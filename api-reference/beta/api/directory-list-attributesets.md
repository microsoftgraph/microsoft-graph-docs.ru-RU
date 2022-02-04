---
title: Атрибуты listSets
description: Получите список объектов attributeSet и их свойств.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="list-attributesets"></a>Атрибуты listSets
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [attributeSet](../resources/attributeset.md) и их свойств.

## <a name="permissions"></a>Разрешения:
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CustomSecAttributeDefinition.Read.All, CustomSecAttributeDefinition.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|CustomSecAttributeDefinition.Read.All, CustomSecAttributeDefinition.ReadWrite.All|

Пользователю, заявляемого в каталог, также должна быть назначена одна из следующих [ролей каталога](/azure/active-directory/roles/permissions-reference):

+ Чтение назначений атрибутов
+ Считыватель определения атрибутов
+ Администратор назначения атрибутов
+ Администратор определения атрибутов

По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /directory/attributeSets
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса
Этот метод поддерживает параметры `$select`запроса OData `$top``$orderBy` и OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` отклика и коллекцию объектов [attributeSet](../resources/attributeset.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-all-attribute-sets"></a>Пример 1. Получить все наборы атрибутов

В следующем примере все наборы атрибутов получаются в клиенте.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_attributeset_all"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/attributeSets
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-attributeset-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-attributeset-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-attributeset-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-attributeset-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-attributeset-all-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-attributeset-all-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attributeSet)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/attributeSets",
    "value": [
        {
            "description": "Attributes for engineering team",
            "id": "Engineering",
            "maxAttributesPerSet": 25
        },
        {
            "description": "Attributes for marketing team",
            "id": "Marketing",
            "maxAttributesPerSet": 25
        }
    ]
}
```

### <a name="example-2-get-top-attribute-sets"></a>Пример 2. Получить верхние наборы атрибутов

В следующем примере приводится топ-10 наборов атрибутов с поддержкой для paging.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_attributeset_top"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/attributeSets?$top=10
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-attributeset-top-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-attributeset-top-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-attributeset-top-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-attributeset-top-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-attributeset-top-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-attributeset-top-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attributeSet)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/attributeSets",
    "@odata.nextLink": "https://graph.microsoft.com/beta/directory/attributeSets?$top=10&$skiptoken={skiptoken}",
    "value": [
        {
            "description": "Attributes for engineering team",
            "id": "Engineering",
            "maxAttributesPerSet": 25
        },
        {
            "description": "Attributes for marketing team",
            "id": "Marketing",
            "maxAttributesPerSet": 25
        }
    ]
}
```

### <a name="example-3-get-attribute-sets-in-order"></a>Пример 3. Привести наборы атрибутов в порядок

В следующем примере получает наборы атрибутов, заказать по id.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_attributeset_orderby"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/attributeSets?$orderBy=id
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-attributeset-orderby-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-attributeset-orderby-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-attributeset-orderby-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-attributeset-orderby-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-attributeset-orderby-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-attributeset-orderby-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attributeSet)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/attributeSets",
    "value": [
        {
            "description": "Attributes for applications",
            "id": "Application",
            "maxAttributesPerSet": 25
        },
        {
            "description": "Attributes for engineering team",
            "id": "Engineering",
            "maxAttributesPerSet": 25
        }
    ]
}
```
