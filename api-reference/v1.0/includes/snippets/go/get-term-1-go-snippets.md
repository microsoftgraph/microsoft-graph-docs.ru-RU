---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f5bbfe5feb893a8ee2e04c75653ed728419086f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093827"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
groupId := "group-id"
setId := "set-id"
termId := "term-id"
result, err := graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).SetsById(&setId).TermsById(&termId).Get(options)


```