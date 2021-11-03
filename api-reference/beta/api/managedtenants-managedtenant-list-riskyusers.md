---
title: Список riskyUsers
description: Получите список объектов riskyUser и их свойств.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 77dfc21112d921469d92e63c7706aeca83af0c7c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "60730531"
---
# <a name="list-riskyusers"></a>Список riskyUsers
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [riskyUser](../resources/managedtenants-riskyuser.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/riskyUsers
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [riskyUser](../resources/managedtenants-riskyuser.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/riskyUsers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.riskyUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_ae8d3a3f-be95-429c-8063-635ccc16e899",
      "userId": "ae8d3a3f-be95-429c-8063-635ccc16e899",
      "userDisplayName": "Cynthia Becker",
      "userPrincipalName": "cynthia@fourthcoffee002.onmicrosoft.com",
      "riskState": "atRisk",
      "riskLevel": "hidden",
      "riskDetail": "hidden",
      "isDeleted": false,
      "riskLastUpdatedDateTime": "2021-06-10T13:58:34.5171907Z",
      "lastRefreshedDateTime": "2021-07-11T11:32:55.2168558Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_05ec33c0-471d-4b1a-901c-093fc65c6401",
      "userId": "05ec33c0-471d-4b1a-901c-093fc65c6401",
      "userDisplayName": "Ina Anthony",
      "userPrincipalName": "ianthony@consolidatedmessenger001.onmicrosoft.com",
      "riskState": "atRisk",
      "riskLevel": "hidden",
      "riskDetail": "hidden",
      "isDeleted": false,
      "riskLastUpdatedDateTime": "2021-06-11T14:35:29.8061797Z",
      "lastRefreshedDateTime": "2021-07-11T14:42:10.8700665Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
