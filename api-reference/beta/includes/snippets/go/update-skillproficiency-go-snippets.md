---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 224c6b4cc657553bb98d260b6890a7a97701279e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340832"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSkillProficiency()
requestBody.SetCategories( []String {
    "Professional",
}
proficiency := "advancedProfessional"
requestBody.SetProficiency(&proficiency)
skillProficiencyId := "skillProficiency-id"
graphClient.Me().Profile().SkillsById(&skillProficiencyId).Patch(requestBody)


```