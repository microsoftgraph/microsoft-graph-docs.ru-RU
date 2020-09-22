---
title: Создание Екстерналитем
description: Создание нового Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6e0ee2ca2eebcca9b912c62242c2606590d9cbc4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192268"
---
# <a name="create-externalitem"></a>Создание Екстерналитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [екстерналитем](../resources/externalitem.md).

Этот API можно использовать для создания настраиваемого элемента. Укажите тип, который вы создаете, включив `@odata.type` свойство в текст JSON. В содержащем [екстерналконнектион](../resources/externalconnection.md) должна быть зарегистрирована [схема](../resources/schema.md) соответствующего типа.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Параметры пути

| Параметр     | Тип   | Описание                                         |
|:--------------|:-------|:----------------------------------------------------|
| ИД подключения | string | `id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md) |
| item-id       | string | Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md). Если такой элемент уже не существует `id` , создается новый элемент. Если такой элемент уже существует `id` , он перезаписывается объектом, отправленным в теле. |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [екстерналитем](../resources/externalitem.md) в формате JSON. Размер полезных данных не может превышать 4 МБ.

### <a name="creating-an-externalitem"></a>Создание Екстерналитем

При создании `externalItem` необходимо указать следующие поля: `@odata.type` , `acl` , и `properties` . `properties`Объект должен содержать по крайней мере одно свойство.

Все `DateTime` свойства типа должны быть в формате ISO 8601.

Свойства в `externalItem` полезных данных должны использовать описатели типов в следующих сценариях:

- Для `String` свойств Type, если значение содержит символы, не входящие в набор ASCII.

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- Для всех типов коллекций.

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > При включении свойства типа `Collection(DateTime)` необходимо использовать описатель типа `Collection(DateTimeOffset)` .

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры

### <a name="example-create-a-custom-item"></a>Пример: Создание настраиваемого элемента

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    },
    {
      "type": "group",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
      "identitySource": "external"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
