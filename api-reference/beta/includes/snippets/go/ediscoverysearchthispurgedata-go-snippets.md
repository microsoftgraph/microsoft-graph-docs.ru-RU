---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: acf05f269f7b5c89081e4fbafeca91231ee5b7fe
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095420"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoverySearchId := "ediscoverySearch-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).SearchesById(&ediscoverySearchId).PurgeData(ediscoveryCase-id, ediscoverySearch-id).Post()


```