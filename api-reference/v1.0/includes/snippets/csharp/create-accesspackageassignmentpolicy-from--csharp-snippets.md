---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e7c4cffa828590547e73e515d552992e97dea9cd
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    DisplayName = "New Policy",
    Description = "policy for assignment",
    AllowedTargetScope = AllowedTargetScope.NotSpecified,
    SpecificAllowedTargets = new List<SubjectSet>()
    {
    },
    Expiration = new ExpirationPattern
    {
        EndDateTime = null,
        Duration = null,
        Type = ExpirationPatternType.NoExpiration
    },
    RequestorSettings = new AccessPackageAssignmentRequestorSettings
    {
        EnableTargetsToSelfAddAccess = false,
        EnableTargetsToSelfUpdateAccess = false,
        EnableTargetsToSelfRemoveAccess = false,
        AllowCustomAssignmentSchedule = true,
        EnableOnBehalfRequestorsToAddAccess = false,
        EnableOnBehalfRequestorsToUpdateAccess = false,
        EnableOnBehalfRequestorsToRemoveAccess = false,
        OnBehalfRequestors = new List<SubjectSet>()
        {
        }
    },
    RequestApprovalSettings = new AccessPackageAssignmentApprovalSettings
    {
        IsApprovalRequiredForAdd = false,
        IsApprovalRequiredForUpdate = false,
        Stages = new List<AccessPackageApprovalStage>()
        {
        }
    },
    AccessPackage = new AccessPackage
    {
        Id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentPolicies
    .Request()
    .AddAsync(accessPackageAssignmentPolicy);

```