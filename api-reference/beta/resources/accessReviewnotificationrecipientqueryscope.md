---
title: accessReviewnotificationrecipientqueryscope resource type
description: Представляет пользователей, которые получат уведомления для отзывов о доступе.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b619b7479212e5fc055f5ab19b025d8d512dc1
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896747"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>accessReviewnotificationrecipientqueryscope resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Указывает статический список получателей (например, определенных пользователей, владельцев групп или членов группы) для получения уведомлений о просмотре доступа.

Наследует [от accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | String | Это представляет запрос для получателей. Например, `/groups/{group id}/members` для участников группы и `/users/{user id}` для определенного пользователя. |
| queryType | String | Указывает тип запроса. Разрешено значение `MicrosoftGraph` . |
| queryRoot | String | В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство требуется только в том случае, если указан относительный запрос. `./manager` |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
