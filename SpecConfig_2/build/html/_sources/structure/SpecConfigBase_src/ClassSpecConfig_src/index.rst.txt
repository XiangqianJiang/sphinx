=============================
The class SpecConfigBase_Func
=============================

public:
   - SpecConfigBase();
   
   - ~SpecConfigBase();

   - virtual int Execute() = 0;

   - void InitAttributes(const std::string& path, const struct property & flags, std::vector<struct Attribute>& attributes);
   
   - void ExtractAttribute(uint8_t * buf, uint32_t size, std::vector<Attribute> & attributes);

   - void DecodeAttributes(std::vector<Attribute> & attributes);
   
   - int ScreenAttributes(std::vector<Attribute> & attributes);
	
private:
   - uint32_t StringToUint32(std::string str);
   
   - std::string GetExpectValue(const JsonObject& valueObj, const struct property & flags, bool ignoreCustomer);

protected:
   - std::vector<std::string> m_stringField;


   
   
   
