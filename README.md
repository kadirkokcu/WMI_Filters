# Sample WMI_Filters for GPO

# For Windows Desktop OS
select * from Win32_OperatingSystem WHERE (ProductType = "1")

# For Windows Server Domain Controller
select * from Win32_OperatingSystem where (ProductType = "2")

# For Windows Server (Domain Member)
select * from Win32_OperatingSystem where (ProductType = "3")

# For Any Windows – Non-Domain Controller
select * from Win32_OperatingSystem where (ProductType = "1") OR (ProductType = "3")
