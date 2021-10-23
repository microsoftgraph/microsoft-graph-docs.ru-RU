---
title: Обновление externalItem
description: Обновление свойств externalitem.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d4e53891336c6a32d932cce280605391aeefba92
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558569"
---
# <a name="update-externalitem"></a>Обновление externalItem

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств [externalitem](../resources/externalconnectors-externalitem.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Параметры пути

| Параметр     | Тип   | Описание                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | строка | `id`Свойствосодержащего [externalConnection](../resources/externalconnectors-externalconnection.md) |
| item-id       | string | Свойство `id` [externalItem,](../resources/externalconnectors-externalitem.md)предоставленное разработчиком. |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства (за исключением свойств внутри объекта), не включенные в тело запроса, будут поддерживать прежние значения или пересчитываться на основе изменений других `properties` значений свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. Могут быть обновлены перечисленные ниже свойства.

| Свойство   | Тип                                  | Описание               |
|:-----------|:--------------------------------------|:--------------------------|
| acl        | [коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. |
| содержимое    | [microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md) | Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. |
| properties | Объект                                | Пакет свойств со свойствами элемента. Свойства должны соответствовать [схеме,](../resources/externalconnectors-schema.md) определенной для [externalConnection.](../resources/externalconnectors-externalconnection.md) |

### <a name="updating-the-acl-collection"></a>Обновление коллекции acl

Если свойство включено в запрос на обновление, существующая коллекция ACL перезаписывается с коллекцией, `acl` включенной в запрос.

### <a name="updating-the-properties-object"></a>Обновление объекта свойств

Если свойство включено в запрос на обновление, существующий пакет свойств перезаписывается со значением, `properties` включенным в запрос.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект externalItem](../resources/externalconnectors-externalitem.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "update_externalitem",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}-->

```http
PATCH https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ]
}
```


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent",
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_externalitem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->


