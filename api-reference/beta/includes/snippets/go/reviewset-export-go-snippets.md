---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d2c978194f7063017047dbf2f573686ac566578
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090265"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
outputName := "2020-12-06 Contoso investigation export"
requestBody.SetOutputName(&outputName)
description := "Export for the Contoso investigation"
requestBody.SetDescription(&description)
exportOptions := "originalFiles,fileInfo,tags"
requestBody.SetExportOptions(&exportOptions)
exportStructure := "directory"
requestBody.SetExportStructure(&exportStructure)
options := &msgraphsdk.ExportRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).Export().Post(options)


```