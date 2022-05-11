---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e182a31fa1b8b255db377e339f95f96a929acf26
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343460"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedAccessId := "privilegedAccess-id"
governanceRoleSettingId := "governanceRoleSetting-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleSettingsById(&governanceRoleSettingId).Get()


```