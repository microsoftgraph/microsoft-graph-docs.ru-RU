---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dd7546f077fcf16d0add4beca9f2b777b95d3681
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629314"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().Snapshots().GetSubscriptions()().Get()


```