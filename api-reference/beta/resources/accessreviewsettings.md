---
title: Тип ресурса accessReviewSettings
description: Предоставляет дополнительные параметры при создании проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdc8d22639d098619ef7183ebe22fc9da7bc0287
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293087"
---
# <a name="accessreviewsettings-resource-type"></a>Тип ресурса accessReviewSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Предоставляет дополнительные параметры при создании проверки доступа для управления поведением функций при запуске проверки доступа.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Логический | Указывает, включена ли отправка сообщений рецензентам и создателю отзывов. |
| remindersEnabled | Логический | Указывает, включена ли отправка напоминаний рецензентам. |
| justificationRequiredOnApproval | Логический | Указывает, должны ли проверяющие предоставлять обоснование при проверке доступа. |
| activityDurationInDays | Int64 | Количество дней действий пользователей, которые будут показываться рецензентам. |
| autoReviewEnabled | Логический | Указывает, следует ли принимать решение, если рецензент не указал его. Используется, если включено автоматическое применение. Если вы не хотите, чтобы решение о проверке было записано, если рецензент не сделал явного выбора, установите для него такое же. `false`|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | Подробные параметры настройки функции для принятия решения об отзыве. Используется, если включено автоматическое применение. |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | Подробные параметры повторения. |
| autoApplyReviewResultsEnabled | Логический | Указывает, включена ли возможность автоматического применения для автоматического изменения ресурса доступа к целевому объекту.  Если этот запрет не включен, пользователь должен после завершения проверки доступа применить проверку доступа. |
| accessRecommendationsEnabled | Логический | Указывает, включены ли рекомендации для проверяющих. |

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
