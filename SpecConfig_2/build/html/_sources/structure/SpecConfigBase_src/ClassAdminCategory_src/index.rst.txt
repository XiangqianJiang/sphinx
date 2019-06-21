=============================
The class AdminCategory_Func
=============================

public:
   - AdminCategory(int instance, const std::string & folder,const std::string & customer,const std::string & capacity,const std::string & security,const std::string & formfactor);

   - int WriteIdentifyCsv(const NVMeAdminCommand &adminCmd,const vector<struct Attribute>& attributes);
   
   - int WriteFeatureCsv(const NVMeAdminCommand &adminCmd,const vector<struct Attribute>& attributes);
   
   - int WriteLogPageCsv(const NVMeAdminCommand &adminCmd,const vector<struct Attribute>& attributes);

   - int WriteCsV(const NVMeAdminCommand &adminCmd,const vector<struct Attribute>& attributes);
   
   - string Replace(string temp,char delim);

   - virtual int Execute();




private:
   - int m_instance;
   
   - std::string m_folder;
  
   - std::string m_customer;
   
   - std::string m_capacity;
   
   - std::string m_security;
   
   - std::string m_formfactor;

   - std::string cust;
   
   - map<std::string, std::string> m_flags;

private:
   - std::map<NVMeAdminCommand, std::vector<struct c_Attribute >> m_cmds;


   
   
   
   
