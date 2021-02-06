---
title: Тип ресурса accessReviewSettings
description: Предоставляет дополнительные параметры при создании проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18af2ef86c33650129934f43d2212222e98448fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133429"
---
# <a name="accessreviewsettings-resource-type"></a>Тип ресурса accessReviewSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дополнительные параметры при создании проверки доступа для управления поведением функций при запуске проверки доступа.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Boolean | Указывает, включена ли отправка сообщений рецензентам и создателю отзывов. |
| remindersEnabled | Boolean | Указывает, включена ли отправка напоминаний рецензентам. |
| justificationRequiredOnApproval | Boolean | Указывает, должны ли проверяющие предоставлять обоснование при проверке доступа. |
| activityDurationInDays | Int64 | Количество дней действий пользователей, которые будут показываться рецензентам. |
| autoReviewEnabled | Boolean | Указывает, следует ли принимать решение, если рецензент не указал его. Используется, если включено автоматическое применение. Если вы не хотите, чтобы решение о проверке было записано, если рецензент не сделал явного выбора, установите для него такое же. `false`|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | Подробные параметры настройки функции для принятия решения об отзыве. Используется, если включено автоматическое применение. |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | Подробные параметры повторения. |
| autoApplyReviewResultsEnabled | Boolean | Указывает, включена ли возможность автоматического применения для автоматического изменения ресурса доступа к целевому объекту.  Если этот запрет не включен, пользователь должен после завершения проверки доступа применить проверку доступа. |
| accessRecommendationsEnabled | Boolean | Указывает, включены ли рекомендации для проверяющих. |

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
