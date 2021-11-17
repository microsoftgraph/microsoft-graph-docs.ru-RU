---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96ec87c9d01cfd72cc26b836a4f6a0916d29b53e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025080"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printTaskDefinitionId := "printTaskDefinition-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Tasks().Get(options)


```