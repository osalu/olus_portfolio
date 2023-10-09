--A QUERY TO EXTRACT ALL THE EMPLOYEES PRESENTLY WORKING IN THE COMPANY
SELECT*
FROM [HumanResources].[Employee]

-- A QUERY TO EXTRACT SINGLE MALE EMPLOYEES 
SELECT[BusinessEntityID],
      [OrganizationLevel],
	  [JobTitle],
      [MaritalStatus],
      [Gender],
      [HireDate]
FROM [HumanResources].[Employee]
WHERE [Gender]='M' AND [MaritalStatus]='S';

--A QUERY TO EXTRACT MALE EMPLOYEE
SELECT [BusinessEntityID],
       [OrganizationLevel],
	   [JobTitle],
       [MaritalStatus],
       [Gender],
       [HireDate]
FROM [HumanResources].[Employee]
WHERE [Gender]<> 'M';
