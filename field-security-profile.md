# Field Security Profiles in Dynamics 365 

## Lesson Overview :pencil2:

This lesson will cover the fundamentals of Field Security Profiles in Dynamics 365. Field Security Profiles in Dynamics 365 allow administrators to control access to specific fields within an entity, protecting sensitive data by restricting user permissions. These profiles let you define who can read, create, or update field data, providing more granular control over security. By enabling field security on a field, organizations can ensure compliance with data privacy regulations and restrict information based on roles. Users or teams can be assigned to specific Field Security Profiles to enforce these restrictions. The lesson will cover creating, configuring, and testing Field Security Profiles. 


<br>

## Learning Objectives :notebook:

By the end of this lesson, you will be able to:

- Understand the purpose and function of Field Security Profiles. 
- Configure and manage Field Security Profiles in Dynamics 365. 
- Apply field-level security to control user access to sensitive data. 
- Test and troubleshoot field security settings. 


<br>

## Key Definitions and Examples :key:

### Field Security Profile 

Field Security Profiles in Dynamics 365 allow administrators to control access to specific fields in an entity for certain users or teams. They help protect sensitive data by providing the ability to define who can read, create, or update field data. This is important for ensuring compliance with privacy regulations and safeguarding confidential information, such as personal details or financial data. 


<u><i>Some real-life examples:</i></u>

- Your organization uses Dynamics 365 to manage employee records and you may want to restrict access to the "Salary" field in an employee record so that only HR staff can view or update it while other users from IT and Operations cannot view or update it. 

- In a healthcare application, patient records contain sensitive personal information, such as "Social Security Number" and "Date of Birth". Only authorized personnel from the HR department should be allowed to view and edit these fields. 

- You are working for a company that handles customer financial data. Only finance managers should have access to view and edit the "Annual Revenue" field in the Account entity. 

### Enabling Field Security on Fields

Field security can be enabled on individual fields within an entity. This process involves marking specific fields, like "Credit Limit" or "Social Security Number," as secure, so that access can be controlled through Field Security Profiles. Once field security is enabled, only users assigned to the relevant profile can view or modify the field. 


<u><i>Example:</i></u>

Suppose you're storing the "Social Security Number (SSN)" field in a contact record. After enabling field security for this field, you configure the profile to allow only Finance users to access it. Users without the profile would see a blank or restricted view of the "Social Security Number" field, depending on the permissions set. 

### Assigning Users and Teams 

Assigning users or teams to a Field Security Profile determines who has access to the restricted fields. This can be done by navigating to the profile and adding the necessary users or entire teams who require access. Teams allow for easier management when you need to apply the same permissions across multiple users with the same role. 

<u><i>Example:</i></u>

For example, if you have created a "ConfidentialInfoProfile" for financial fields, you can assign the Finance team to this profile. This will grant all Finance team members the ability to read or update fields like "Annual Revenue" or "Credit Limit" without needing to individually assign each user. 

### Testing and Troubleshooting Field Security 

Testing field security involves logging in as different users to verify their permissions on the secured fields. You should check that users who have been assigned to the Field Security Profile can access the protected fields, while those without access should see restricted or hidden data. Troubleshooting may involve ensuring field security is enabled and that users/teams are correctly assigned. 

<u><i>Example:</i></u>

After setting up a "HRAccessProfile" for the "Salary" field, log in as an HR employee and confirm that they can view and update the "Salary" field. Next, log in as a non-HR user, such as a Sales representative, and verify that they cannot see or edit the "Salary" field, confirming the profile is working as intended. 

<br>

## Additional Resources :clipboard:

If you would like to study these concepts before the class or would benefit from some remedial studying, please utilize the resources below:

- [Field level security to control access ](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/admin/field-level-security?view=op-9-1)
