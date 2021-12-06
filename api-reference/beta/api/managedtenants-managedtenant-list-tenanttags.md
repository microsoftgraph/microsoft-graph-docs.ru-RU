---
title: Список tenantTags
description: Получите список объектов tenantTag и их свойств.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 60b35cdef256c4485e89d609b1c02d30e4e7c6ca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020711"
---
# <a name="list-tenanttags"></a>Список tenantTags
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [tenantTag](../resources/managedtenants-tenanttag.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.Read.All, ManagedTenants.WriteRead.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-tenanttag-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags",
    "value": [
        {
            "id": "913391c0-5466-42b4-900d-0a7501399cb0",
            "displayName": "Onboarding",
            "description": "Tenants that we are currently onboarding",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "34298981-4fc8-4974-9486-c8909ed1521b",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:36:31.086644Z",
            "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
            "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
            "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        },
        {
            "id": "bfd883e8-10f3-40ee-994c-111fa1c5d1db",
            "displayName": "ExtendedSupport",
            "description": "Tenants that have purchased extended support.",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:43:31.8917383Z",
            "createdByUserId": "43a2424c-0fa3-446d-bee9-4ab500bb1603",
            "lastActionDateTime": "2021-06-17T03:23:31.3531635Z",
            "lastActionByUserId": "248f617e-a6a7-4d31-922d-726c24074bb6",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        }
    ]
}
```
