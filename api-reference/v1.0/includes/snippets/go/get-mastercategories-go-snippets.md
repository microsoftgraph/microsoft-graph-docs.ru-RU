---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8d0379c74a50e069ec7331c2f5e9a38031dae123
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61296169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().MasterCategories().Get(nil)


```