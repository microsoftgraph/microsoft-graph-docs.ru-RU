---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3786e287115443bece14d99ff86d841a96fdb12e
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628935"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAgreementFileLocalization()
fileName := "Contoso ToU for guest users (French)"
requestBody.SetFileName(&fileName)
language := "fr-FR"
requestBody.SetLanguage(&language)
isDefault := false
requestBody.SetIsDefault(&isDefault)
isMajorVersion := false
requestBody.SetIsMajorVersion(&isMajorVersion)
displayName := "Contoso ToU for guest users (French)"
requestBody.SetDisplayName(&displayName)
fileData := msgraphsdk.NewAgreementFileData()
requestBody.SetFileData(fileData)
data := []byte("base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data")
fileData.SetData(&data)
agreementId := "agreement-id"
result, err := graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Files().Post(requestBody)


```