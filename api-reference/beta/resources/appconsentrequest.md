---
title: тип ресурса appConsentRequest
description: Запрос, который представляет собой агрегацию userConsentRequests для определенного приложения.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f823f64d4c0324aeca74c3268d6fc95d313e2f00
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965235"
---
# <a name="appconsentrequest-resource-type"></a>тип ресурса appConsentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список appConsentRequests](../api/appconsentrequest-list.md)|[коллекция appConsentRequest](../resources/appconsentrequest.md)|Получите список объектов [appConsentRequest](../resources/appconsentrequest.md) и их свойств.|
|[Get appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)|
|[Список appConsentRequests: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|Список [appConsentRequests,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appDisplayName|String|Отображение имени приложения, для которого запрашивается согласие. Обязательный. Поддерживает `$filter` `eq` (только) и `$orderby` . |
|appId|String|Идентификатор приложения. Обязательный. Поддерживает `$filter` `eq` (только) и `$orderby` . |
|consentType|Строка|Тип согласия запроса. Возможные значения: `Static`   и  `Dynamic` . Они представляют статические и динамические разрешения, соответственно, запрашиваются в рабочего процесса согласия. Поддерживает `$filter` `eq` (только) и `$orderby` . Обязательный.|
|id|Строка|Идентификатор запроса на согласие приложения. Обязательный.|
|pendingScopes|[коллекция appConsentRequestScope](../resources/appconsentrequestscope.md)|Список ожидающих утверждения областей. Это пусто, если consentType `Static` . Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|userConsentRequests|[коллекция userConsentRequest](../resources/userconsentrequest.md)|Список ожидающих запросов на согласие пользователей.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```

