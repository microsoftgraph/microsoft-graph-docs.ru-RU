---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb90ec671916a73366ce9d58e7471df1881b371e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445727"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Stop-MgPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -GovernanceRoleAssignmentRequestId $governanceRoleAssignmentRequestId

```