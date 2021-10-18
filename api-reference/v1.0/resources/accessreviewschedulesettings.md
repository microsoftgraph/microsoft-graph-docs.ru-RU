---
title: тип ресурса accessReviewScheduleSettings
description: Представляет параметры, связанные с серией обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 322e6b0dee9f2a66465096bd5e0f38a20a482483
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452041"
---
# <a name="accessreviewschedulesettings-resource-type"></a>тип ресурса accessReviewScheduleSettings

Пространство имен: microsoft.graph

**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| mailNotificationsEnabled|Логический | Указывает, включена ли электронная почта или отключена. Значение по умолчанию — `false`.               |
| reminderNotificationsEnabled|Логический  | Указывает, включены или отключены напоминания. Значение по умолчанию — `false`.  |
| justificationRequiredOnApproval|Логический | Указывает, требуются ли рецензенты для обоснования своего решения. Значение по умолчанию — `false`. |
| defaultDecisionEnabled|Логический | Указывает, включено или отключено решение по умолчанию, если рецензенты не отвечают. Значение по умолчанию — `false`. |
| defaultDecision|String | Решение, **выбранное, если значение defaultDecisionEnabled** `true` является . Может быть одним из `Approve` `Deny` , или `Recommendation` . |
| instanceDurationInDays|Int32 | Продолжительность каждого повторения обзора **(accessReviewInstance)** в количестве дней. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры для повторения с помощью стандартного объекта Outlook повторения. Поддерживаются `weekly` `absoluteMonthly` только и при **повторном повтореPattern.** Используйте свойство **startDate на** **recurrenceRange,** чтобы определить день начала проверки. |
| autoApplyDecisionsEnabled|Логический | Указывает, применяются ли решения автоматически. Если установлено, администратор должен применять решения вручную, как только рецензент завершит `false` обзор доступа. При наборе решения применяются автоматически после окончания срока действия экземпляра проверки доступа независимо от того, откликнулись ли `true` рецензенты. Значение по умолчанию — `false`. |
| applyActions|[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после завершения проверки. В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` . Поле должно быть указано только в случае `disableAndDeleteUserApplyAction` . |
| recommendationsEnabled|Логический | Указывает, включены или отключены рекомендации по принятию решений. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```
