============================
The class TDD_LogPage3E_Func 
============================

public:
   - TDD_LogPage3E(int instance,const string & folder,const string & customer,const string & capacity,const string & security,const string & formfactor);

   - int WriteLogPage3ECsv(vector<struct Attribute>& attributes);
   
   - virtual int Execute();

private:
   - int m_instance;
   
   - std::string m_folder;
   
   - std::string m_customer;
   
   - std::string m_capacity;
   
   - std::string m_security;
   
   - std::string m_formfactor;

   



   
   
   
   
