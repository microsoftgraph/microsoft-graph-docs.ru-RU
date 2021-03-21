---
title: тип ресурса userConsentRequest
description: Запрос, созданный пользователем на использование приложения, требующее доступа к организационным данным, несанкционированный для предоставления согласия для себя.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d3d91688a0a385ea319dee6df90b45c52bd4ec89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965189"
---
# <a name="userconsentrequest-resource-type"></a>тип ресурса userConsentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[UserConsentRequest](../resources/userconsentrequest.md) создается пользователем при запросе доступа к приложению, к которому требуется авторизация администратора. 

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список userConsentRequests](../api/userconsentrequest-list.md)|[коллекция userConsentRequest](../resources/userconsentrequest.md)|Получите список объектов [userConsentRequest](../resources/userconsentrequest.md) и их свойств.|
|[Get userConsentRequest](../api/userconsentrequest-get.md)|[userConsentRequest](../resources/userconsentrequest.md)|Ознакомьтесь с свойствами и отношениями [объекта userConsentRequest.](../resources/userconsentrequest.md)|
|[Список userConsentRequests: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md)|[коллекция userConsentRequest](../resources/userconsentrequest.md)|Получите список объектов [userConsentRequest](../resources/userconsentrequest.md) и их свойств.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalId|Строка|Id утверждения. Это значение равно значению `id` .|
|completedDateTime|DateTimeOffset|Дата и время, когда **состояние** запроса было отмечено как `Completed` . Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший запрос.|
|createdDateTime|DateTimeOffset|Дата и время создания запроса. Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$filter` `eq` (только) и `$orderby` .|
|customData|Строка|Свободное текстовое поле для определения настраиваемой информации для запроса согласия пользователя. Не используется.|
|id|Строка|Идентификатор запроса. |
|reason|Строка|Обоснование пользователем необходимости доступа к приложению. Поддерживает `$filter` `eq` (только) и `$orderby` .  |
|status|String|Состояние запроса на согласие приложения пользователя. Возможные значения: `Initializing` , `InProgress` и `Completed` . Поддерживает `$filter` `eq` (только) и `$orderby` . |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|утверждение|[утверждение](../resources/approval.md)|Решения об утверждении, связанные с запросом.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "reason": "String"
}
```

