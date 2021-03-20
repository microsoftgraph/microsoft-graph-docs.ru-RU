---
title: Список использования устройствRights
description: Извлечение списка объектов useRights для устройства.
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a855ebf34d8e97a7a5fad00df2a022779ff2bc0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946830"
---
# <a name="list-device-usagerights"></a>Список использования устройствRights
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка [объектов useRight](../resources/usageright.md) для данного устройства.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот API поддерживает параметр $filter [OData.](/graph/query-parameters) Поддерживаются следующие шаблоны $filter:

- $filter = значение состояния eq
- $filter = serviceIdentifier eq 'value'
- $filter = состояние eq 'value' и serviceIdentifier eq 'value'
- $filter = состояние в ('value1', 'value2')
- $filter = serviceIdentifier в ('value1', 'value2')
- $filter = состояние в ('value1', 'value2') и serviceIdentifier в ('value1', 'value2')

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|odata.maxpagesize|Установите переоценку размера страницы максимального результата. Необязательный параметр.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного использования этот метод возвращает код отклика и коллекцию `200 OK` [объектов useRight](../resources/usageright.md) в тексте отклика.

Кроме того, если в ответе больше страниц, возвращается @odata.nextLink.

## <a name="examples"></a>Примеры

### <a name="example-1-get-all-usage-rights-for-a-device"></a>Пример 1. Получить все права использования для устройства
 
#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/devices/fead5c35-ebc5-47c4-a909-c43b4faf2160/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "99f828b9-09f2-445d-a758-b6727316dbe1",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a>Пример 2. Получить права использования для устройства с определенными идентификаторами и состояниями службы

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "value": [
    {
      "id": "9905e6b1-9040-4926-b028-fdb748c359d6",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
