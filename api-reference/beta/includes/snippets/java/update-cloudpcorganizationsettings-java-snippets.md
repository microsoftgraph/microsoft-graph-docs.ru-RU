---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b402d71cadbf148eed24a8cda6b24317d13a92e4
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225029"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOrganizationSettings cloudPcOrganizationSettings = new CloudPcOrganizationSettings();
cloudPcOrganizationSettings.userAccountType = CloudPcUserAccountType.STANDARD_USER;
cloudPcOrganizationSettings.osVersion = CloudPcOperatingSystem.WINDOWS11;

graphClient.deviceManagement().virtualEndpoint().organizationSettings()
    .buildRequest()
    .patch(cloudPcOrganizationSettings);

```