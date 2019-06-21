==============================
The class AdminGetLogPage_Func 
==============================

public:
   - AdminGetLogPageSection(const std::string & file,uint8_t nsid,uint32_t size);
   
   - virtual ~AdminGetLogPageSection();

protected:
   - virtual void HandleByteFieldName (const std::string & name);
   
   - virtual void HandleBitFieldName  (const std::string & name);

   - virtual void HandleBitFieldValue(const JsonObject& val, const std::string & cust, const std::set<std::string>& m_flags);

private:
   - uint8_t m_lpid;
   
   - uint8_t m_nsid;
   
   - uint32_t m_size;


   
   
   
   
