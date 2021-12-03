---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 00e79227eb285039adfb79386cd83a309d163f3d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294846"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

connectedOrganizationId := "connectedOrganization-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).InternalSponsors().Get(nil)


```