---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1119c8d6e8b424a3857be6dd5aa5af9af696024c69b7f6ac30a8cf339cfb4612
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "de9315c1-272b-4905-924b-cc112ca180c7";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.displayName = "Community Outreach";
accessPackageResource.description = "https://contoso.sharepoint.com/sites/CSR";
accessPackageResource.resourceType = "SharePoint Online Site";
accessPackageResource.originId = "https://contoso.sharepoint.com/sites/CSR";
accessPackageResource.originSystem = "SharePointOnline";
AccessPackageResourceEnvironment accessPackageResourceEnvironment = new AccessPackageResourceEnvironment();
accessPackageResourceEnvironment.originId = "https://contoso-admin.sharepoint.com/";
accessPackageResource.accessPackageResourceEnvironment = accessPackageResourceEnvironment;
accessPackageResourceRequest.accessPackageResource = accessPackageResource;
accessPackageResourceRequest.requestType = "AdminAdd";

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```