# NIM-System-REST-Campus-Nexus

# Create Application Key
The purpose of this is to provide steps on generating and using key based authentication for Student Rest APIs

* Introduction 
The Application API Keys configuration is enhanced to be used when authenticating to the entire Student REST API set instead of only being used for the Campuslink APIs. 

This enhancement:
    * Limits the integrating partners to only access the modules to which they have permissions. Appropriate audits will be recorded in the database. 
    * Allows the integrating partner to generate their own application key, associated to a user in the Staff entity. 

* Steps
    * Location - Select Settings > System > Application API Keys.
  
    ![image](https://github.com/Tools4ever-NIM/NIM-System-REST-Campus-Nexus/assets/24281600/049b9163-5b3e-487c-9a08-bb5168c6303c)
    ![image](https://github.com/Tools4ever-NIM/NIM-System-REST-Campus-Nexus/assets/24281600/396c515a-bc96-401e-beda-996512ebd939)

    * Product Help Link      
    https://help.campusmanagement.com/CNS/23.0/WebClient/Content/SU/System/ApplicationAPIK

    * Encode the Application with Base 64
    https://www.base64encode.org/ 
 
    `{"CallingAppName":"DualEnrollAPI","KeyValue":"YsIQkq2Hj/viKSM5Lzn07Q=="} `

        * CallingAppName: Calling Application Name 
        * KeyValue: Application Key 

    Encode the value and share it with client/vendor
    
    ![image](https://github.com/Tools4ever-NIM/NIM-System-REST-Campus-Nexus/assets/24281600/faf2abed-b9ed-4826-a573-a1e2ddb11b6c)

    Client/Vendor can use the encoded value with “ApplicationKey encoded value

    ![image](https://github.com/Tools4ever-NIM/NIM-System-REST-Campus-Nexus/assets/24281600/2d65f251-d756-4fcc-82d5-8b20bf315712)



