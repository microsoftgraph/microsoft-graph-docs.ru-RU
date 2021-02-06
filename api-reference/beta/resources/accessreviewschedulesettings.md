---
title: Тип ресурса accessReviewScheduleSettings
description: В функции проверки доступа Azure AD параметры, связанные с ряду отзывов `accessReviewScheduleSettings` о доступе.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a58ba9a682e443efbc159befaea61b15e3fdc81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133450"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Тип ресурса accessReviewScheduleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) 

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | Флаг, который указывает, включены ли или отключены сообщения электронной почты.                |
| reminderNotificationsEnabled|Boolean  | Флаг, который указывает, включены или отключены напоминания.   |
| justificationRequiredOnApproval|Boolean | Флаг, который указывает, требуются ли проверяющих для обоснования своего решения. |
| defaultDecisionEnabled|Boolean | Флаг, который указывает, включено ли решение по умолчанию, если рецензенты не отвечают. |
| defaultDecision|Строка | Решение, выбранное, `defaultDecisionEnabled` если включено. Может иметь одно из двух ок: "Утвердить", "Запретить" или "Рекомендация". |
| instanceDurationInDays|Int32 | Длительность каждого повторения проверки `accessReviewInstance` () в днях. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Подробные параметры повторения. Использование стандартного объекта повторения Outlook.  |
| autoApplyDecisionsEnabled|Boolean | Флаг, который указывает, включена ли функция автоматического применения. |
| applyActions|[Коллекция accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Необязательное поле. Описывает действия, которые необходимо выполнить после проверки. В настоящее время поддерживаются два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` . Поле должно быть указано только в случае с `disableAndDeleteUserApplyAction` . См. [accessReviewApplyAction.](accessreviewapplyaction.md) |
| recommendationsEnabled|Boolean | Флаг, который указывает, включены ли рекомендации по принятию решений. |

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
