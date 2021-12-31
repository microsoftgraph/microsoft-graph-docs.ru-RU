---
title: тип ресурса appConsentRequest
description: Запрос, представляюща коллекцию объектов userConsentRequest для определенного приложения.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 36323f32276b609eeda2430c5a71f4bd5855599d
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651304"
---
# <a name="appconsentrequest-resource-type"></a>тип ресурса appConsentRequest

Пространство имен: microsoft.graph

Коллекция объектов [userConsentRequest](../resources/userconsentrequest.md) для определенного приложения.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список appConsentRequests](../api/appconsentapprovalroute-list-appconsentrequests.md)|[коллекция appConsentRequest](../resources/appconsentrequest.md)|Извлечение коллекции [объектов appConsentRequest](appconsentrequest.md) и их свойств.|
|[Get appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)|
|[filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md)|[appConsentRequest](../resources/appconsentrequest.md)|Ознакомьтесь с свойствами объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние запроса на согласие пользователя `InProgress` . |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|appDisplayName|String|Отображение имени приложения, для которого запрашивается согласие. Обязательный. Поддерживает `$filter` `eq` (только) и `$orderby` . |
|appId|String|Идентификатор приложения. Обязательный. Поддерживает `$filter` `eq` (только) и `$orderby` . |
|id|Строка|Идентификатор запроса на согласие приложения. Обязательное.|
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
