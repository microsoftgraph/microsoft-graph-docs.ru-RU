---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ae7cc863fbf740e0cb6d915ff4c491408fbbe1c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091582"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamsAppId := "teamsApp-id"
teamsAppDefinitionId := "teamsAppDefinition-id"
graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).AppDefinitionsById(&teamsAppDefinitionId).OutlineIcon().HostedContent().$value().Get(options)


```