---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3f5bfc75f0a6924c2f71fe082f1f30f974726ea7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342814"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganizationalBrandingLocalization()
backgroundColor := "#00000F"
requestBody.SetBackgroundColor(&backgroundColor)
id := "fr-FR"
requestBody.SetId(&id)
signInPageText := " "
requestBody.SetSignInPageText(&signInPageText)
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().Localizations().Post(requestBody)


```