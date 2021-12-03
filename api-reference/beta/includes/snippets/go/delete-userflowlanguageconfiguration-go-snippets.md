---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 412a7a46a7791d4a9e19250f9f41bd85f8c9e6b8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).Delete(nil)


```