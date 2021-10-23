---
title: Создание externalItem
description: Создание нового externalItem.
author: snlraju-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e0d7bb9066ba09dfb6b133a64d796e89f4b195a9
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560837"
---
# <a name="create-externalitem"></a>Создание externalItem

Пространство имен: microsoft.graph.externalConnectors

Создайте [новый объект externalItem.](../resources/externalconnectors-externalitem.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Неприменимо|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Application| ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections/{connectionsId}/items
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [externalItem.](../resources/externalconnectors-externalitem.md)

При создании [externalItem](../resources/externalconnectors-externalitem.md)можно указать следующие свойства.

|Свойство|Тип| Описание|
|:---|:---|:---|
|id|Строка|ID элемента. Обязательный.|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|Свойства элемента. Объект `properties` должен содержать по крайней мере одно свойство. Все `DateTime` свойства типа должны быть в формате ISO 8601. Обязательно.|
|содержимое|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|Внешний контент элемента. Необязательный параметр.|
|acl|[коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)|Список управления доступом. Обязательный.|

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

В случае успешного выполнения этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры

### <a name="example-create-a-custom-item"></a>Пример: Создание настраиваемой номенклатуры

### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
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



### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

