---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b581edc8c87eb61574a482700e5d969fdc93fdbe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganizationalBrandingLocalization()
signInPageText := "Welcome to Contoso France."
requestBody.SetSignInPageText(&signInPageText)
usernameHintText := " "
requestBody.SetUsernameHintText(&usernameHintText)
organizationId := "organization-id"
organizationalBrandingLocalizationId := "organizationalBrandingLocalization-id"
graphClient.OrganizationById(&organizationId).Branding().LocalizationsById(&organizationalBrandingLocalizationId).Patch(requestBody)


```