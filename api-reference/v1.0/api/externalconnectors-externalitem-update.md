---
title: Обновление externalItem
description: Обновление свойств объекта externalItem.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 91dedc0c061a4469092ea4e4525398c2126dc3ca
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439312"
---
# <a name="update-externalitem"></a>Обновление externalItem
Пространство имен: microsoft.graph.externalConnectors



Обновление свойств объекта [externalItem](../resources/externalconnectors-externalitem.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
| Делегированные (рабочая или учебная учетная запись)     | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Параметры пути

| Параметр     | Тип   | Описание                                         |
|:--------------|:-------|:----------------------------------------------------|
| идентификатор подключения | string | Свойство `id` содержащего [externalConnection](../resources/externalconnectors-externalconnection.md) |
| item-id       | string | Предоставленное разработчиком `id` свойство [externalItem](../resources/externalconnectors-externalitem.md). |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства ( `properties` за исключением свойств внутри объекта), которые не включены в текст запроса, сохраняют предыдущие значения или пересчитываются на основе изменений других значений свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. Могут быть обновлены перечисленные ниже свойства.

| Свойство   | Тип                                  | Описание               |
|:-----------|:--------------------------------------|:--------------------------|
| Acl        | [Коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) | Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. |
| содержимое    | [microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md) | Текстовое представление содержимого элемента. Текст в этом свойстве является полнотекстовой индексированной. |
| properties | Объект                              | Контейнер свойств со свойствами элемента. Свойства должны соответствовать [схеме](../resources/externalconnectors-schema.md) , определенной для [внешнего соединения](../resources/externalconnectors-externalconnection.md). |

### <a name="updating-the-acl-collection"></a>Обновление коллекции ACL

Если свойство `acl` включено в запрос на обновление, существующая коллекция ACL перезаписывается коллекцией, включенной в запрос.

### <a name="updating-the-properties-object"></a>Обновление объекта свойств

Если свойство `properties` включено в запрос на обновление, существующий контейнер свойств перезаписывается значением, включенным в запрос.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный [объект externalItem](../resources/externalconnectors-externalitem.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/external/connections/contosohr/items/TSP228082938
Content-Type: application/json

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-externalitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-externalitem-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Отклик
Ниже приведен пример отклика.

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
      "accessType": "grant"
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
