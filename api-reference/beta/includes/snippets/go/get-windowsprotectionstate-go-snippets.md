---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05157028741973d85b208e33016748b5e3a0f5fe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343007"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

windowsProtectionStateId := "windowsProtectionState-id"
result, err := graphClient.TenantRelationships().ManagedTenants().WindowsProtectionStatesById(&windowsProtectionStateId).Get()


```