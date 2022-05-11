---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 941dbf636a49e3c3c41f48ac57f4a9585a9886d3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341070"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Resume(educationSynchronizationProfile-id).Post()


```