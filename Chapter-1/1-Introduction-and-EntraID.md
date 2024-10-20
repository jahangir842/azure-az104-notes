# AZ-104, Introduction:

AZ-104 is the **Microsoft Azure Administrator** certification exam. It is designed for IT professionals who manage cloud services, including storage, networking, security, and compute capabilities within Microsoft Azure.

### Key Responsibilities for Azure Administrators:
- **Manage Azure Subscriptions and Resources**: Monitor usage and billing, manage resource groups, and administer Azure policies.
- **Implement and Manage Storage**: Secure and manage storage accounts, configure Azure files, and implement backup and restore capabilities.
- **Manage and Configure Virtual Networks**: Set up virtual networks, implement network security groups, and configure load balancing.
- **Manage Azure Identities and Governance**: Control access using role-based access control (RBAC), manage identities, and configure multi-factor authentication (MFA) and Azure EntraID.
- **Deploy and Manage Compute Resources**: Create and configure virtual machines (VMs), manage VM backups, and monitor the health of VMs.
- **Monitor and Maintain Azure Resources**: Set up monitoring, analyze alerts, and implement Azure backup solutions.

### Target Audience
- IT professionals looking to manage cloud resources in Azure environments.
- Administrators managing day-to-day tasks such as deployment, monitoring, and security in Azure.

### Related Certifications
- **Prerequisite**: No formal prerequisites, though experience in Azure is recommended.
- **Related Certifications**: Azure Fundamentals (AZ-900), Azure Solutions Architect (AZ-305), Azure DevOps Engineer (AZ-400).

AZ-104 is a critical certification for professionals aiming to manage Azure services and is essential for cloud administrators.

#### **1. Signing Up on the Azure Portal**
- **URL**: [https://portal.azure.com](https://portal.azure.com)
- **Steps to Sign Up**:
   1. Go to the URL above.
   2. Use your **email address** and **password** to log in. If you don’t have an account, sign up with a new one.
   3. After login, you will be redirected to the Azure portal dashboard.

---

### 2. EntraID 
**Entra ID**, previously known as **Azure Active Directory (Azure AD)**, is Microsoft’s cloud-based identity and access management service. It provides secure sign-in, authentication, and access control for users and applications within the Azure ecosystem and beyond. 

- Unlike AD DS, Microsoft Entra ID is multi-tenant by design and is implemented specifically to ensure isolation between its individual directory instances.
- At any given time, an Azure subscription must be associated with one, and only one, Microsoft Entra tenant.
- You can associate the same Microsoft Entra tenant with multiple Azure subscriptions. This allows you to use the same users, groups, and applications to manage resources across multiple Azure subscriptions.

### Key Features:
1. **User Authentication**: Manages user identities and grants access to apps and services.
2. **Single Sign-On (SSO)**: Allows users to access multiple apps with one set of credentials.
3. **Multi-Factor Authentication (MFA)**: Adds an extra layer of security by requiring a second form of verification.
4. **Conditional Access**: Controls how and when users can access resources based on location, device, and risk level.
5. **Role-Based Access Control (RBAC)**: Assigns permissions to users based on their roles in the organization.
   
#### **EntraID Licensing Options**: https://learn.microsoft.com/en-us/entra/fundamentals/licensing
1. **Free Tier**: 
   - 55,000 free identities, ideal for testing and development.

2. **P1 License (Premium 1)**:
   - Advanced security and identity management for hybrid setups.

3. **P2 License (Premium 2)**:
   - Includes P1 features, plus enhanced identity protection for large enterprises.

4. **Suite License**: 
   - Combines **Microsoft 365** with Azure for integrated productivity and security.


Entra ID is crucial for managing identities and securing access in cloud and hybrid environments.

---

### What is Microsoft Entra? https://learn.microsoft.com/en-us/entra/fundamentals/what-is-entra

**Microsoft Entra** is a suite of identity and network access solutions designed to help organizations adopt a Zero Trust security strategy. It establishes a trust fabric that verifies identities, validates access conditions, checks permissions, encrypts connection channels, and continuously monitors for potential compromises.

### **Microsoft Entra Product Family**

The Microsoft Entra product family encompasses four maturity stages of secure end-to-end access for reliable identities. These stages include:
- Implementing Zero Trust access controls
- Securing access for employees
- Securing access for customers and partners
- Protecting any cloud environment


---

#### **3. Azure Directories and Tenants**
- **Default Directory**: Each Azure account is automatically assigned a **default directory**, which is also called a **tenant**.
- **Directory = Tenant**: In Azure, a **directory** and a **tenant** are essentially the same thing. They are used to manage identities and resources within the Azure ecosystem.
- **Multiple Tenants**: You can create multiple tenants (directories) if needed. Each tenant can be used for different environments or organizations.

   > **Note**: Only paid customers can create a new Workforce tenant in Microsoft Entra ID. Customers using a free tenant, or a trial subscription won't be able to create additional tenants from the Microsoft Entra admin center..

---

#### **4. Working with Entra ID**
   - **Entra ID**: This is the new name for Azure Active Directory (Azure AD).
   - **Tenant Overview**: In Entra ID, you can go to the **Overview** section and select **Manage Tenants**. Here, you will see:
     - **Your Tenants**: These are the tenants created by you or your organization.
     - **Guest/External Tenants**: These are the tenants you've been added to as a guest or external user.

   - **Switching Between Tenants**: 
     - Select a tenant and switch between them using the **tenant switch** feature. 
     - The tenant you are currently using is visible in the top-right corner of the portal, under your email.
     - You can also switch tenants by clicking the **gear icon** (⚙) near your profile image.

   > **Note**: Only a **Super Admin** can create new tenants. **Global Admins** do not have this privilege by default.

---

#### **Choosing a License**
Before signing up, decide which subscription to use:
- **Azure/Microsoft 365** subscription.
- **Enterprise Mobility + Security (EMS)** plan.
- **Microsoft Volume Licensing**.


---

#### **5. Managing Users in Azure**
   - **Default Users**: Initially, the only user in a tenant is the one who created the account.
   - **Groups**: There are no default groups when you first log in.
   
   - **Creating New Users**: 
     - There are two ways to add users in Entra ID: 
       1. **Create a New User**.
       2. **Invite an External User** (guest).
     - **Principal Name**: This becomes the **login ID**.
     - **Domain Selection**: If the user is only for Office 365, select the appropriate email domain.
     - **User Type**: You can choose **Member** or **Guest**. For internal users, select **Member**.

   - **Review and Create**:
     - After entering the required details, review and create the user.
     - Copy the **login name** and **password** for the newly created user.
   
   - **Identity of the User**: The identity of a user is tied to the **tenant** they belong to.
   - You can then **log in** using the new user's credentials.

---

#### **6. Entra ID Role vs Service Role**
   - **Entra ID Roles**:
     - These roles control access to resources within the directory (tenant).
     - Examples include **User Admin**, **Global Admin**, and **Directory Readers**.
   
   - **Service Roles**:
     - Service roles provide access to specific services within Azure (e.g., Virtual Machines, Storage, etc.).
     - Examples include **Virtual Machine Contributor** or **Storage Account Reader**.

---

#### **7. Azure AZ-401 (Advanced)** 
   - **AZ-401 Certification**: This certification is focused on advanced DevOps practices in Azure.
   - **Price**: The classroom price for this certification is approximately **$2500**.
   - **Scenarios**: This training includes scenario-based learning, which is critical for real-world application.
   - **Free Courses**: Note that free courses typically do not include scenario-based training.

---
