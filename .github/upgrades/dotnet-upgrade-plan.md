# .NET10.0 Upgrade Plan

## Execution Steps

Execute steps below sequentially one by one in the order they are listed.

1. Validate that an .NET10.0 SDK required for this upgrade is installed on the machine and if not, help to get it installed.
2. Ensure that the SDK version specified in global.json files is compatible with the .NET10.0 upgrade.
3. Upgrade eShop.csproj

## Settings

This section contains settings and data used by execution steps.

### Excluded projects

| Project name | Description |
|:-----------------------------------------------|:---------------------------:|

### Aggregate NuGet packages modifications across all projects

NuGet packages used across all selected projects or their dependencies that need version update in projects that reference them.

| Package Name | Current Version | New Version | Description |
|:------------------------------------|:---------------:|:-----------:|:----------------------------------------------|
| Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore |9.0.3 |10.0.0 | Recommended for .NET10.0 |
| Microsoft.AspNetCore.Identity.EntityFrameworkCore |9.0.3 |10.0.0 | Recommended for .NET10.0 |
| Microsoft.AspNetCore.Identity.UI |9.0.3 |10.0.0 | Recommended for .NET10.0 |
| Microsoft.EntityFrameworkCore.SqlServer |9.0.3 |10.0.0 | Recommended for .NET10.0 |
| Microsoft.EntityFrameworkCore.Tools |9.0.3 |10.0.0 | Recommended for .NET10.0 |
| Microsoft.VisualStudio.Web.CodeGeneration.Design |9.0.0 |10.0.0-rc.1.25458.5 | Recommended for .NET10.0 |

### Project upgrade details

#### eShop.csproj modifications

Project properties changes:
 - Target framework should be changed from `net9.0` to `net10.0`

NuGet packages changes:
 - Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore should be updated from `9.0.3` to `10.0.0` (recommended for .NET10.0)
 - Microsoft.AspNetCore.Identity.EntityFrameworkCore should be updated from `9.0.3` to `10.0.0` (recommended for .NET10.0)
 - Microsoft.AspNetCore.Identity.UI should be updated from `9.0.3` to `10.0.0` (recommended for .NET10.0)
 - Microsoft.EntityFrameworkCore.SqlServer should be updated from `9.0.3` to `10.0.0` (recommended for .NET10.0)
 - Microsoft.EntityFrameworkCore.Tools should be updated from `9.0.3` to `10.0.0` (recommended for .NET10.0)
 - Microsoft.VisualStudio.Web.CodeGeneration.Design should be updated from `9.0.0` to `10.0.0-rc.1.25458.5` (recommended for .NET10.0)
