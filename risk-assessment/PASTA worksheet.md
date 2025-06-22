## PASTA worksheet

---

| Stages | Sneaker company |
| :---- | :---- |
| **I. Define business and security objectives** | Make **2-3 notes** of specific business requirements that will be analyzed. *A secure and safe app for transactions and customer data stored in the database should be protected.THis app connects many people from different places to the sellers and shoppers , there data privacy concern is prioritised.* |
| **II. Define the technical scope** | List of technologies used by the application: *Application programming interface (API) Public key infrastructure (PKI) SHA-256 SQL* I would prioritize evaluating the **API** because it is the main channel through which the app exchanges data with external systems. APIs are often targeted by attackers due to potential vulnerabilities like weak authentication, data exposure, or injection flaws. Securing the API is critical to protecting user data and overall app integrity. |
| **III. Decompose application** | [Sample data flow diagram](https://docs.google.com/presentation/d/1ol7y79popTFfNHM-90ES-H-i1Lpd0YNvPShxBlXozjg/template/preview?resourcekey=0-DZAkf7Vzh2PXsP-j3oXV-g) |
| **IV. Threat analysis** | List **2 types of threats** in the PASTA worksheet that are risks to the information being handled by the application. *Two key threats to the sneaker app are **API exploitation** and **social engineering attacks**. Injection Session hijacking* |
| **V. Vulnerability analysis** |  Two vulnerabilities that could be exploited are **insecure API endpoints** and **insufficient employee security awareness**. APIs without proper authentication or input validation can be targeted with injection attacks or credential stuffing to gain access to user data. Additionally, if employees aren’t trained to recognize phishing or social engineering attempts, they may unknowingly expose credentials or internal system access. These weaknesses create opportunities for attackers to compromise the app and its sensitive information. |
| **VI. Attack modeling** | [Sample attack tree diagram](https://docs.google.com/presentation/d/1FmWLyHgmq9XQoVuMxOym2PHO8IuedCkan4moYnI-EJ0/template/preview?usp=sharing&resourcekey=0-zYPY7AhPJdcClXamlAfOag) |
| **VII. Risk analysis and impact** | List **4 security controls** that can reduce risk. *SHA-256, incident response procedures, password policy, principle of least privilege* |

---

