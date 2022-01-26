---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ced2e0435dce72bb43db8da5f1c4b0fe7b5186f8
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOrganizationSettings = new CloudPcOrganizationSettings
{
    UserAccountType = CloudPcUserAccountType.StandardUser,
    OsVersion = CloudPcOperatingSystem.Windows11
};

await graphClient.DeviceManagement.VirtualEndpoint.OrganizationSettings
    .Request()
    .UpdateAsync(cloudPcOrganizationSettings);

```