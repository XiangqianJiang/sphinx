======================
The class Section_Func 
======================

public:
   - Section(const std::string & file);
   
   - virtual ~Section();

   - void Load(const std::string & cust, const std::map<std::string, std::string> & m_flags);

protected:
   - virtual void HandleByteFieldName (const std::string & name);
   
   - virtual void HandleByteFieldRange(uint32_t s, uint32_t e);
   
   - virtual void HandleBitFieldName  (const std::string & name);
	
   - virtual void HandleBitFieldRange (uint32_t s, uint32_t e);

   - virtual std::string HandleCustomer (const std::string & enable, const std::string & cust);
	
   - virtual std::set<std::string> HanleSplitValue(const std::string & enable, const std::map<std::string, std::string>& m_flags);

   - virtual void HandleBitFieldValue(const JsonObject& val, const std::string & cust, const std::set<std::string>& m_flags);

   - virtual std::string GetSplitFlag(const std::map<std::string, std::string> & m_flags) { return ""; }

   - void   LoadData (const JsonArray  & data,  const std::string & cust, const std::map<std::string, std::string> & m_flags);

protected:
   - std::string ReadFile();

protected:
   - std::string m_path;
   
   - c_Attribute m_attr;
   
   - std::vector<c_Attribute> m_attrs;


   



   
   
   
   
