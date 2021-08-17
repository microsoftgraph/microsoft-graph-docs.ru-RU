---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8bcb80069f53466bcf19a77277a6dfa8d2cf90362fbdcdf93192c683e608d717
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("hasMembersWithLicenseErrors eq true")
    .Select("id,displayName")
    .GetAsync();

```