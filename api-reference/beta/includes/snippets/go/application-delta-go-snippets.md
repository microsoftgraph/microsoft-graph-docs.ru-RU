---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b4739805e3cf6198d3c3c4acbb1c653cd963de9a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294586"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).Get(nil)


```