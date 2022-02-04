---
title: Get attributeSet
description: Ознакомьтесь с свойствами и отношениями объекта attributeSet.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="get-attributeset"></a>Get attributeSet
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [attributeSet](../resources/attributeset.md) .

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

По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на определение, чтение или назначение настраиваемой атрибуты безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /directory/attributeSets/{attributeSetId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса
Этот метод поддерживает параметры `$select` запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` отклика и [объект attributeSet](../resources/attributeset.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-get-an-attribute-set"></a>Пример. Получить набор атрибутов

В следующем примере получается один набор атрибутов с именем `Engineering`.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attributeset_single"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/attributeSets/Engineering
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attributeset-single-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attributeset-single-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attributeset-single-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attributeset-single-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-attributeset-single-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-attributeset-single-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeSet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/attributeSets/$entity",
    "description": "Attributes for engineering team",
    "id": "Engineering",
    "maxAttributesPerSet": 25
}
```
