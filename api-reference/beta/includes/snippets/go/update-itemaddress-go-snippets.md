---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46cde7b4cf3176c932bfa8b6d6c66d21aa0cff69
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294469"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemAddressId := "itemAddress-id"
graphClient.UsersById(&userId).Profile().AddressesById(&itemAddressId).Patch(nil)


```