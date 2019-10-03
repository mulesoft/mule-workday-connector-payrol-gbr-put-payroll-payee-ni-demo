Workday Anypoint Connector Demo - Payroll GBR-Put Payroll Payee NI
=================================================================

## Introduction

The present demo is an application that provides a **complete workflow** to sequentially invoke some of Workday's standard operations.

## Prerequisites

* Java 8
* Anypoint Studio 7.x
* Mule Runtime 4.1.x EE or higher
* APIKit
* DataWeave
* Access to a Workday account

## Import the project

* Go to **File > Import**.
* Select **Anypoint Studio Project from External Location** (under the parent folder "Anypoint Studio").
* Provide the root **path to the demo** project folder.
* Select **Mule Runtime (4.1.x EE)**.
* Click **Finish**.
* Set credentials inside the file `src/main/resources/mule-app.properties`.

   ```
   workday.username=
   workday.password=
   workday.tenantname=
   workday.hostname=
   ```

* Open the **Global Element Configuration**.

   ![Global Element](images/workday-config.png)

* Click the **Test Connection** button to ensure there is connectivity with the sandbox. A successful message should pop-up.

## Run the demo

* Go to **Run > Run As > Mule Application**. 

## Payroll GBR-Put Payroll Payee NI

* Open a browser and access the URL **http://localhost:8081/**. You should see the **Create Position form**.

   ![Demo Create Position](images/CreatePosition.png)

* Click on **Create Position** button.
* Click on **Put Applicant** button under **Put Applicant form**.

   ![Demo Put Applicant](images/PutApplicant.png)
   
* Click on **Hire Employee** button under **Hire Employee form**.

   ![Demo Hire Employee](images/HireEmployee.png)

* Click on **Put Payee NI** button under **Put Payee NI form**.

   ![Demo Put Payee NI](images/PutPayeeNI.png)

* Click on **Get Payee NI** button under **Get Payee NI form**.

   ![Demo Get Payee NI](images/GetPayeeNI.png)
    
* A successful message with Employee ID value should appear.

   ![Demo Success](images/success.png)

## See more
* For additional technical information on the Workday Connector, visit our [technical reference documentation](https://docs.mulesoft.com/connectors/workday/workday-reference) or refer to the [Workday Documentation Site](https://docs.mulesoft.com/connectors/workday/workday-connector).
* For more information on Workday, go to the [Workday API site](https://community.workday.com/api).
