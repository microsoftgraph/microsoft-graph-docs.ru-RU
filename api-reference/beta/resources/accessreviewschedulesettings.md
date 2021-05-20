---
title: тип ресурса accessReviewScheduleSettings
description: В функции обзоров доступа Azure AD представлены параметры, связанные `accessReviewScheduleSettings` с серией обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b354ebfc2b5e6c8093f65c8712516421f0b1d332
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579734"
---
# <a name="accessreviewschedulesettings-resource-type"></a>тип ресурса accessReviewScheduleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) 

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | Указывает, включена ли электронная почта или отключена. Значение по умолчанию — `false`.               |
| reminderNotificationsEnabled|Boolean  | Указывает, включены или отключены напоминания. Значение по умолчанию — `false`.  |
| justificationRequiredOnApproval|Boolean | Указывает, требуются ли рецензенты для обоснования своего решения. Значение по умолчанию — `false`. |
| defaultDecisionEnabled|Boolean | Указывает, включено или отключено решение по умолчанию, если рецензенты не отвечают. Значение по умолчанию — `false`. |
| defaultDecision|Строка | Решение, `defaultDecisionEnabled` выбранное, если включено. Может быть одним из `Approve` `Deny` , или `Recommendation` . |
| instanceDurationInDays|Int32 | Продолжительность каждого повторения обзора `accessReviewInstance` () в количестве дней. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры для повторения с помощью стандартного объекта Outlook повторения. Поддерживаются `weekly` `absoluteMonthly` только и при **повторном повтореPattern.** Используйте свойство **startDate на** **recurrenceRange,** чтобы определить день начала проверки. |
| autoApplyDecisionsEnabled|Boolean | Указывает, применяются ли решения автоматически. Если установлено, пользователь должен применять решения вручную, как только рецензент завершит `false` обзор доступа. При наборе решения применяются автоматически после окончания срока действия экземпляра проверки доступа независимо от того, откликнулись ли `true` рецензенты. Значение по умолчанию — `false`. |
| applyActions|[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после завершения проверки. В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` . Поле должно быть указано только в случае `disableAndDeleteUserApplyAction` . См. [accessReviewApplyAction](accessreviewapplyaction.md). |
| recommendationsEnabled|Boolean | Указывает, включены ли рекомендации по принятию решений или отключены. |

## <a name="relationships"></a>Отношения
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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
