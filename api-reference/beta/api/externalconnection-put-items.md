---
title: Создание externalItem
description: Создание нового externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 170c3fb87903e6f2f66fe910d80ca8f4a6e87b50
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366807"
---
# <a name="create-externalitem"></a>Создание externalItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [externalItem](../resources/externalitem.md).

Этот API можно использовать для создания настраиваемой номенклатуры. Укажите тип, который вы создаете, включив `@odata.type` свойство в тело JSON. Содержащая [externalConnection](../resources/externalconnection.md) должна иметь [схему,](../resources/schema.md) зарегистрированную соответствующего типа.

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
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Параметры пути

| Параметр     | Тип   | Описание                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | `id`Свойствосодержащего [externalConnection](../resources/externalconnection.md) |
| item-id       | string | Свойство `id` [externalItem,](../resources/externalitem.md)предоставленное разработчиком. Если с этим элементом уже не `id` существует, создается новый элемент. Если элемент уже существует с этим, он `id` перезаписывается объектом, отправленным в тело. |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [externalItem.](../resources/externalitem.md) Нагрузка ограничена 4 МБ.

### <a name="creating-an-externalitem"></a>Создание externalItem

При создании поля требуются следующие `externalItem` поля: `@odata.type` и `acl` `properties` . Объект `properties` должен содержать по крайней мере одно свойство.

Все `DateTime` свойства типа должны быть в формате ISO 8601.

Свойства на объекте должны использовать указанные типы в полезной `externalItem` нагрузке в следующих сценариях:

- Для `String` свойств типа, если значение содержит символы, не относимые к ASCII.

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
    > При включаем свойстве типа `Collection(DateTime)` необходимо использовать указанный `Collection(DateTimeOffset)` тип.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры

### <a name="example-create-a-custom-item"></a>Пример: Создание настраиваемой номенклатуры

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
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
