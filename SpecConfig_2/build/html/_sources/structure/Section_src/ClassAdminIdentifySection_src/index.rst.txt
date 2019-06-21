===================================
The class AdminIdentifySection_Func
===================================

public:
   - AdminIdentifySection(const string & path, uint8_t nsid, uint8_t cns);
   - virtual ~AdminIdentifySection();

protected:
   - virtual void HandleBitFieldName  (const std::string & name);
   - virtual void HandleBitFieldValue(const JsonObject& val, const std::string & cust, const std::set<std::string>& m_flags);

private:
   - uint8_t m_cns;
   - uint8_t m_nsid;
