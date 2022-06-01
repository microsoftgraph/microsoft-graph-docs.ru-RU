---
title: Тип ресурса accessReviewSettings (не рекомендуется)
description: Предоставляет дополнительные параметры при создании проверки доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f197ca69132252a58508aa57b2c192eaae34077f
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821206"
---
# <a name="accessreviewsettings-resource-type-deprecated"></a>Тип ресурса accessReviewSettings (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Предоставляет дополнительные параметры при создании проверки доступа для управления поведением функции при запуске проверки доступа.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Логическое | Указывает, включена ли отправка сообщений рецензентам и создателю проверки. |
| remindersEnabled | Логическое | Указывает, включена ли отправка напоминаний рецензентам. |
| justificationRequiredOnApproval | Логическое | Указывает, требуются ли рецензенты для предоставления обоснования при проверке доступа. |
| activityDurationInDays | Int64 | Количество дней действий пользователей, отображаемые рецензентам. |
| autoReviewEnabled | Логическое | Указывает, должно ли быть задано решение, если рецензент не указал его. Используется, если включено автоматическое применение. Если вы не хотите, чтобы решение о проверке было записано, если рецензент не сделает явный выбор, задайте для него значение `false`.|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | Подробные параметры того, как эта функция должна задавать решение о проверке. Используется, если включено автоматическое применение. |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | Подробные параметры повторения. |
| autoApplyReviewResultsEnabled | Логическое | Указывает, включена ли функция автоматического применения для автоматического изменения ресурса доступа к целевому объекту.  Если этот параметр не включен, пользователь должен после завершения проверки доступа применить проверку доступа. |
| accessRecommendationsEnabled | Логическое | Указывает, включены ли рекомендации для рецензентов. |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
```json
{
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,  
  "justificationRequiredOnApproval": true,
  "activityDurationInDays": 1024,
  "autoReviewEnabled": false,
  "autoReviewSettings": {"@odata.type": "microsoft.graph.autoReviewSettings"},
  "recurrenceSettings": {"@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"},
  "autoApplyReviewResultsEnabled": false,
  "accessRecommendationsEnabled": false
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
