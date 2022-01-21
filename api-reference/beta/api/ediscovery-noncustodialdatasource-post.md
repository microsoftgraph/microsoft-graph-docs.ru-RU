---
title: Создание noncustodialDataSource
description: Создайте новый объект noncustodialDataSource.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f8082aa0b4413c804d250b74bb2ad5220d42fbcd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100218"
---
# <a name="create-noncustodialdatasource"></a>Создание noncustodialDataSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса подарят представление JSON объекта [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)

В следующей таблице показаны свойства, необходимые при создании [noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|applyHoldToSource|Логический|Указывает, применяется ли удержание к источнику данных без хранения (например, к почтовому ящику или сайту).|
|datasource|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Либо userSource, либо siteSource.  Для userSource используйте "dataSource": { "@odata.type": "microsoft.graph.ediscovery.userSource", "email" : "SMTP address"}.  Для источника сайта используйте "dataSource": { "@odata.type": "microsoft.graph.ediscovery.siteSource", "site@odata.bind": "siteId" }, где siteId можно извлечь из URL-адреса сайта, например, запрос Microsoft Graph будет `https://contoso.sharepoint.com/sites/HumanResources` `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` . ID — это первый GUID, указанный в поле ID.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-add-a-non-custodial-data-source-user-or-group-mailbox-with-an-email"></a>Пример 1. Добавление пользователя источника данных или группового почтового ящика без хранения с помощью электронной почты

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_email"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
Content-Type: application/json

{
    "applyHoldToSource" : true,
    "dataSource" : {
        "@odata.type" : "microsoft.graph.ediscovery.userSource",
        "email" : "adelev@contoso.com"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-noncustodialdatasource-from-email-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-noncustodialdatasource-from-email-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-noncustodialdatasource-from-email-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-noncustodialdatasource-from-email-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-noncustodialdatasource-from-email-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-noncustodialdatasource-from-email-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "0",
    "lastModifiedDateTime": "2021-02-19T07:02:45.7732516Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "39374346363831303741353341373443",
    "displayName": null,
    "createdDateTime": "2021-02-19T07:02:45.4863718Z",
    "applyHoldToSource": true
}
```

### <a name="example-2-add-a-non-custodial-data-source-site-with-a-url"></a>Пример 2. Добавление источника данных без хранения с URL-адресом

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_siteurl"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/noncustodialdatasources
Content-Type: application/json

{
    "applyHoldToSource": false,
    "dataSource": {
        "@odata.type": "microsoft.graph.ediscovery.siteSource",
        "site": {
            "webUrl": "https://contoso.sharepoint.com/sites/SecretSite"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-noncustodialdatasource-from-siteurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-noncustodialdatasource-from-siteurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-noncustodialdatasource-from-siteurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-noncustodialdatasource-from-siteurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-noncustodialdatasource-from-siteurl-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-noncustodialdatasource-from-siteurl-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('15d80234-8320-4f10-96d0-d98d53ffdfc9')/noncustodialDataSources/$entity",
    "status": "Active",
    "lastModifiedDateTime": "2021-08-11T22:43:45.1079425Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "35393843394546413031353146334134",
    "displayName": "Secret Site",
    "createdDateTime": "2021-08-11T22:43:45.0189955Z",
    "applyHoldToSource": false
}
```
