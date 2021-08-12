---
title: тип ресурса appConsentRequest
description: Запрос, представляюща коллекцию объектов userConsentRequest для определенного приложения.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d6fae1c3914f901c24190b5c27b184b4c90aa5e67cfdc54416ec5e6f81703361
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155227"
---
# <a name="appconsentrequest-resource-type"></a>тип ресурса appConsentRequest

Пространство имен: microsoft.graph

Коллекция объектов [userConsentRequest](../resources/userconsentrequest.md) для определенного приложения.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список appConsentRequests](../api/appconsentrequest-list.md)|[коллекция appConsentRequest](../resources/appconsentrequest.md)|Извлечение коллекции [объектов appConsentRequest](appconsentrequest.md) и их свойств.|
|[Get appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)|
|[filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|Ознакомьтесь с свойствами объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние запроса на согласие пользователя `InProgress` . |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|appDisplayName|String|Отображение имени приложения, для которого запрашивается согласие. Обязательный элемент. Поддерживает `$filter` `eq` (только) и `$orderby` . |
|appId|String|Идентификатор приложения. Обязательный элемент. Поддерживает `$filter` `eq` (только) и `$orderby` . |
|id|String|Идентификатор запроса на согласие приложения. Обязательный элемент.|
|pendingScopes|[коллекция appConsentRequestScope](../resources/appconsentrequestscope.md)|Список ожидающих утверждения областей. Обязательный.|

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
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```
