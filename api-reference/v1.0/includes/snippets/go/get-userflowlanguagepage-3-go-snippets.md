---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 073b481e79e3a22e8ea223def709865f0f140ef6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63416881"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
userFlowLanguagePageId := "userFlowLanguagePage-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).DefaultPagesById(&userFlowLanguagePageId).$value().Get(nil)


```