---
title: accessReviewnotificationrecipientqueryscope resource type
description: Указывает список пользователей, которые будут получать уведомления для отзывов о доступе.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82d1cbffd3e51ee8aff5dee3bdefd3196d004243
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562142"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>accessReviewnotificationrecipientqueryscope resource type

Пространство имен: microsoft.graph

Указывает статический список получателей (например, определенных пользователей, владельцев групп или членов группы) для получения уведомлений о просмотре доступа.

Наследует [от accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | Строка | Представляет запрос для получателей. Например, `/groups/{group id}/members` для участников группы и `/users/{user id}` для определенного пользователя. |
| queryType | Строка | Указывает тип запроса. Разрешено значение `MicrosoftGraph` . |
| queryRoot | Строка | В сценарии, в котором рецензенты должны быть указаны динамически, указывается относительный источник запроса. Это свойство требуется только в том случае, если указан относительный запрос (то есть). `./manager` |


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
