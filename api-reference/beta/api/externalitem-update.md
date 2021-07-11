---
title: Обновление externalitem
description: Обновление свойств externalitem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c862a6139f4f24a9207e7387913ec0fc5b04e8e6
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366800"
---
# <a name="update-externalitem"></a>Обновление externalitem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств [externalitem](../resources/externalitem.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Параметры пути

| Параметр     | Тип   | Описание                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | `id`Свойствосодержащего [externalConnection](../resources/externalconnection.md) |
| item-id       | string | Свойство `id` [externalItem,](../resources/externalitem.md)предоставленное разработчиком. |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства (за исключением свойств внутри объекта), не включенные в тело запроса, будут поддерживать прежние значения или пересчитываться на основе изменений других `properties` значений свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. Могут быть обновлены перечисленные ниже свойства.

| Свойство   | Тип                                  | Описание               |
|:-----------|:--------------------------------------|:--------------------------|
| acl        | [коллекция acl](../resources/acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. |
| содержимое    | [externalItemContent](../resources/externalitemcontent.md) | Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. |
| properties | Объект                                | Пакет свойств со свойствами элемента. Свойства должны соответствовать [схеме,](../resources/schema.md) определенной для [externalConnection.](../resources/externalconnection.md) |

### <a name="updating-the-acl-collection"></a>Обновление коллекции acl

Если свойство включено в запрос на обновление, существующая коллекция ACL перезаписывается с коллекцией, `acl` включенной в запрос.

### <a name="updating-the-properties-object"></a>Обновление объекта свойств

Если свойство включено в запрос на обновление, существующий пакет свойств перезаписывается со значением, `properties` включенным в запрос.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект externalItem](../resources/externalitem.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
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


