---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cd3b97e55280783a0e4514dc16e29ca02512cb5e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

organizationId := "organization-id"
organizationalBrandingLocalizationId := "organizationalBrandingLocalization-id"
graphClient.OrganizationById(&organizationId).Branding().LocalizationsById(&organizationalBrandingLocalizationId).BannerLogo().Get(nil)


```