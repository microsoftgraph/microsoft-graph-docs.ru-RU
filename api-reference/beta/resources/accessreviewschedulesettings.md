---
title: тип ресурса accessReviewScheduleSettings
description: В функции обзоров доступа Azure AD представлены параметры, связанные `accessReviewScheduleSettings` с серией обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77ea7d8601df36525aad7a3448aa3b6f031d98d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469327"
---
# <a name="accessreviewschedulesettings-resource-type"></a>тип ресурса accessReviewScheduleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) 

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Логический | Флаг, чтобы указать, включены ли или отключены сообщения электронной почты.                |
| reminderNotificationsEnabled|Логический  | Флаг, чтобы указать, включены ли или отключены напоминания.   |
| justificationRequiredOnApproval|Логический | Флаг, чтобы указать, требуются ли рецензенты для обоснования своего решения. |
| defaultDecisionEnabled|Логический | Флаг, чтобы указать, включено или отключено решение по умолчанию, если рецензенты не отвечают. |
| defaultDecision|String | Решение, `defaultDecisionEnabled` выбранное, если включено. Может быть одним из "Утверждение", "Отказ" или "Рекомендация". |
| instanceDurationInDays|Int32 | Продолжительность каждого повторения обзора `accessReviewInstance` () в количестве дней. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры для повторения. Использование стандартного объекта повторения Outlook. Обратите внимание, что dayOfMonth не поддерживается — используйте свойство startDate на recurrenceRange, чтобы определить день начала проверки. |
| autoApplyDecisionsEnabled|Логический | Флаг, чтобы указать, включена ли функция автоматического применения. |
| applyActions|[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после завершения проверки. В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` . Поле должно быть указано только в случае `disableAndDeleteUserApplyAction` . См. [accessReviewApplyAction](accessreviewapplyaction.md). |
| recommendationsEnabled|Логический | Флаг, чтобы указать, включены или отключены рекомендации по принятию решений. |

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
