- 👋 Hi, I’m @chrisdoveiress
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
chrisdoveiress/chrisdoveiress is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
```mermaid
C4Context
  title System Context diagram for LCBTL
  Person(pBroker, "Broker", "broker")
  Boundary(b0, "MSO") {
  
      System(sysCM, "Case Management")
      System(sysDip, "DIP")
      System(sysFma, "FMA")
      System(sysLCBTL, "Limited Company BTL")
  }


  System_Ext(sysBankValidation, "Bank Validation", "Allows users .")
  System_Ext(sysCompanyHouse, "Company House", "Allow users to look up company house data.")


Rel(pBroker, sysCM, "Creates a new case in case management")
Rel(sysCM, sysCompanyHouse, "Retrives Company information from")
Rel(sysCM, sysDip, "Retrives Company information from")
```
