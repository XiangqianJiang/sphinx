=====================================
The class AdminGetFeatureSection_Func 
=====================================

public:
   - AdminGetFeatureSection(const std::string & file)
   
   - virtual ~AdminGetFeatureSection();

protected:
   - virtual void HandleByteFieldName(const std::string & name)
   
   - virtual void HandleBitFieldName (const std::string & name)

   - virtual std::set<std::string> HanleSplitValue(const std::string & enable, const std::map<std::string, std::string>& m_flags)

   - virtual void HandleBitFieldValue(const JsonObject& val, const std::string & cust, const std::set<std::string>& m_flags)

private:
   - NVMeGetFeatureCommand m_cmd




   
   
   
   
