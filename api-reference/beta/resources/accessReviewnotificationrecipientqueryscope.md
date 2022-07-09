---
title: Тип ресурса accessReviewnotificationrecipientqueryscope
description: Представляет пользователей, которые будут получать уведомления для проверок доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fae6a904f06424f79ea96ce4750efa67f6cf1cd4
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697955"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>Тип ресурса accessReviewnotificationrecipientqueryscope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Указывает статический список получателей (например, конкретных пользователей, владельцев групп или участников группы) для получения уведомлений о проверке доступа.

Наследуется [от accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | Строка | Это представляет запрос для получателей. Например, для `/groups/{group id}/members` участников группы и `/users/{user id}` для определенного пользователя. |
| queryType | Строка | Указывает тип запроса. Допустимое значение: `MicrosoftGraph`. |
| queryRoot | String | В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для определения относительного источника запроса. Это свойство требуется только в том случае, если указан относительный запрос, `./manager`то есть ). |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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
