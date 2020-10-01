---
title: Тип ресурса Акцессревиевсеттингс
description: Предоставляет дополнительные параметры при создании проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4de925ecb2fac65e3ab339ba8d4e602fcdc2af3
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330356"
---
# <a name="accessreviewsettings-resource-type"></a>Тип ресурса Акцессревиевсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дополнительные параметры при создании проверки доступа, чтобы управлять поведением компонента при запуске проверки доступа.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| маилнотификатионсенаблед | Boolean | Указывает, включена ли отправка почты рецензентам и создателю рецензирования. |
| реминдерсенаблед | Boolean | Указывает, включено ли отправку сообщений напоминания рецензентам. |
| жустификатионрекуиредонаппровал | Boolean | Указывает, требуются ли проверяющие для предоставления обоснования при проверке доступа. |
| активитидуратиониндайс | Int64 | Количество дней, в течение которых действия пользователей отображаются для рецензентов. |
| ауторевиевенаблед | Boolean | Указывает, следует ли задать решение, если проверяющий не предоставил его. Для использования при включенном автоматическом применении. Если вы не хотите, чтобы решение для проверки было записано, пока проверяющий не выйдет явный выбор, задайте для него значение `false` .|
| ауторевиевсеттингс | [ауторевиевсеттингс](autoreviewsettings.md) | Подробные параметры, определяющие, как компонент должен устанавливать решение по проверке. Для использования при включенном автоматическом применении. |
| рекурренцесеттингс | [акцессревиеврекурренцесеттингс](accessreviewrecurrencesettings.md) | Подробные параметры для периодичности. |
| аутоапплиревиевресултсенаблед | Boolean | Указывает, включена ли функция автоматического применения, чтобы автоматически изменить целевой ресурс доступа к объектам.  Если этот параметр не включен, пользователь должен, после завершения проверки, применить проверку доступа. |
| акцессрекоммендатионсенаблед | Boolean | Указывает, включены ли рекомендации для рецензентов. |

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