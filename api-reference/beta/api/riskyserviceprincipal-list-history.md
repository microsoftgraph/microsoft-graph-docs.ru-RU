---
title: История списка (история рисков riskyServicePrincipal)
description: Получите историю рисков объекта riskyServicePrincipal.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e05c7babbea8f51f849e574d687ebde88c284d94
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334592"
---
# <a name="list-history-risk-history-of-riskyserviceprincipal"></a>История списка (история рисков riskyServicePrincipal)
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите историю рисков объекта [riskyServicePrincipal](../resources/riskyServicePrincipal.md) .

>**Примечание:** Для использования API riskyServicePrincipal требуется лицензия Azure AD Premium P2.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|IdentityRiskyServicePrincipal.Read.All, IdentityRiskyServicePrincipal.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|IdentityRiskyServicePrincipal.Read.All, IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyServicePrincipals/{riskyServicePrincipalId}/history 
```
## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот `200 OK` метод возвращает код отклика и коллекцию объектов [riskyServicePrincipalHistoryItem](../resources/riskyserviceprincipalhistoryitem.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyserviceprincipalhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/riskyServicePrincipals/{riskyServicePrincipalId}/history
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyserviceprincipalhistoryitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyserviceprincipalhistoryitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyserviceprincipalhistoryitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyserviceprincipalhistoryitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-riskyserviceprincipalhistoryitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.riskyServicePrincipalHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyServicePrincipalHistoryItem",
  "value": [
    {
       "id": "0fbef39d-9e8c-460b-444e-8ae5abcdffd7",
       "accountEnabled": true,
       "isProcessing": false,
       "riskLastUpdatedDateTime": "2021-10-20T01:14:37.7214159Z",
       "riskState": "atRisk",
       "riskDetail": "none",
       "riskLevel": "high",
       "displayName": "Contoso App",
       "appId": "ede08db0-9492-4a0c-8ae3-8ggg056c5d75",
       "servicePrincipalType": "Application",
       "servicePrincipalId": "0fbef39d-9e8c-777b-860e-8ae5abcdffd7",
       "initiatedBy": null,
       "activity": null
     }
  ]
}
```
