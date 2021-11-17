---
title: Перечисление типов ресурсов claimsMappingPolicy
description: Получите список объектов claimsMappingPolicy.
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cbc6b65631db29e228e248d6abb67c620a7ff86b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975712"
---
# <a name="list-claimsmappingpolicies"></a>Перечисление типов ресурсов claimsMappingPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [claimsMappingPolicy.](../resources/claimsmappingpolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |

> [!IMPORTANT]
> Этот метод имеет [известные проблемы разрешений и](/graph/known-issues#claims-mapping-policy) может требовать согласия на оба разрешения.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры `$expand` `$filter` запроса `$select` OData и OData для настройки `$top` ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters). При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [claimsMappingPolicy](../resources/claimsmappingpolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-claimsmappingpolicies-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/claimsMappingPolicies",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/cb7e01e0-06e7-4636-a3f5-0aa994f9d164/Microsoft.DirectoryServices.ClaimsMappingPolicy",
            "id": "cb7e01e0-06e7-4636-a3f5-0aa994f9d164",
            "deletedDateTime": null,
            "definition": [
                "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"},{\"Source\":\"user\",\"ID\":\"givenname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname\"},{\"Source\":\"user\",\"ID\":\"displayname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\"},{\"Source\":\"user\",\"ID\":\"surname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname\"},{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"username\"}],\"ClaimsTransformation\":[{\"ID\":\"CreateTermsOfService\",\"TransformationMethod\":\"CreateStringClaim\",\"InputParameters\": [{\"ID\":\"value\",\"DataType\":\"string\", \"Value\":\"sandbox\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"TOS\",\"TransformationClaimType\":\"createdClaim\"}]}]}}"
            ],
            "displayName": "Test1234",
            "isOrganizationDefault": false
        },
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/3bf1b5b2-5fb3-4a5a-80f3-bb0f1e246977/Microsoft.DirectoryServices.ClaimsMappingPolicy",
            "id": "3bf1b5b2-5fb3-4a5a-80f3-bb0f1e246977",
            "deletedDateTime": null,
            "definition": [
                "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\":[{\"Source\":\"user\",\"ID\":\"extensionattribute1\"},{\"Source\":\"transformation\",\"ID\":\"DataJoin\",\"TransformationId\":\"JoinTheData\",\"JwtClaimType\":\"JoinedData\"}],\"ClaimsTransformations\":[{\"ID\":\"JoinTheData\",\"TransformationMethod\":\"Join\",\"InputClaims\":[{\"ClaimTypeReferenceId\":\"extensionattribute1\",\"TransformationClaimType\":\"string1\"}], \"InputParameters\": [{\"ID\":\"string2\",\"Value\":\"sandbox\"},{\"ID\":\"separator\",\"Value\":\".\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"DataJoin\",\"TransformationClaimType\":\"outputClaim\"}]}]}}"
            ],
            "displayName": "TestclaimsPolicy",
            "isOrganizationDefault": false
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List claimsMappingPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


