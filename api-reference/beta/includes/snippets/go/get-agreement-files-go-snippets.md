---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe4822374b0114b87943a41ab0c2da66456cf528
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340393"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AgreementRequestBuilderGetQueryParameters{
    Expand: "files",
}
options := &msgraphsdk.AgreementRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
agreementId := "agreement-id"
result, err := graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```