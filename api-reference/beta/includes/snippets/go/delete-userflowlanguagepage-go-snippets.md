---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eddf41ae0a07c581180a6c1ce91c1db269235dcc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988770"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
userFlowLanguagePageId := "userFlowLanguagePage-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).OverridesPagesById(&userFlowLanguagePageId).$value().Delete(options)


```