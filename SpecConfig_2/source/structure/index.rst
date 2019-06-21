=================
Program Structure
=================

The source files for the test program are organized into a component hierarchy.

The Input and Output
>>>>>>>>>>>>>>>>>>>>
:Input: Json File

#. configspec_NVMeCommandSetSpecific
#. ...
#. onfigspec_GET_FEATURES
#. configspec_GET LOG PAG
#. ...
	
:Output: print out and CSV File
   
.. toctree::
   :maxdepth: 1

   Print out log <log>
   CSV File <csv>
   
   
      
	
	

The whole Program Framework
>>>>>>>>>>>>>>>>>>>>>>>>>>>

::

  #. class SpecConfigBase for all spec config
  #. class Section and AminSection for Admin only
  
 ┌───────+───<Start> - class TmSpecConfig : public TMBase
 ├    
 ├───────+───<Father Class> - class SpecConfigBase
 ├       ├─ class AdminCategory        : public SpecConfigBase   ==> m_cmds
 ├       ├─ class TDD_LogPage3E        : public SpecConfigBase
 ├       ├─ class NvmeRegSpecConfig    : public SpecConfigBase
 ├       └─ class PcieSpecConfig       : public SpecConfigBase
 ├    
 └──────────+───<Father Class 1> - class Section.
            │───<Father Class 2> - class AdminSection: public Section ==> use m_cmds  
            │                                                         friend class AdminCategory
            ├─ class AdminIdentifySection	: public AdminSection ==> fill m_cmds
            ├─ class AdminGetFeatureSection	: public AdminSection ==> fill m_cmds
            └─ class AdminGetLogPageSection	: public AdminSection ==> fill m_cmds


   

AdminSection Framework
>>>>>>>>>>>>>>>>>>>>>>

- map_cmd
   - 64 byte Nvme cmd
   - Attribute
 
- Attribute 
   - std::string jsonName;
   - std::string name;
   - uint32_t offset;	
   - uint32_t length;
   - std::string actualValue;
   - std::string expectValue;

.. note::
   We start from **int TmSpecConfig::Execute()** where the ``AdminSection`` and ``TDD_LogPage3E`` obj will be created.
   Then we execute ``int AdminCategory::Execute()`` and ``int TDD_LogPage3E::Execute()``.
   
   In the **AdminCategory::Execute()** 
   the ``AdminIdentifySection`` ``AdminGetLogPageSection`` and ``AdminGetFeatureSection`` obj will be created.
   We will load the json file and prepare the cmd setting and attribute for the **<m_cmds>** which is the member from the AdminSection.
   Once **<m_cmds>** map is done, we will loop it and do the flow of  ``SendCommand()`` , ``ExtractAttribute()`` , ``DecodeAttributes``
   ``ScreenAttributes`` and  ``WriteCsV`` .
   
   In the **TDD_LogPage3E::Execute()** 
   We just run the flow of ``SendTDDcmd()`` , ``InitAttributes`` , ``ExtractAttribute()`` , ``DecodeAttributes``
   ``ScreenAttributes`` and  ``WriteCsV`` .
   



**Contents:**

.. toctree::
   :maxdepth: 2

   About Class SpecConfigBase <SpecConfigBase_src/index>
  

.. toctree::
   :maxdepth: 2

   About Class Section <Section_src/index>
   
   
   

   