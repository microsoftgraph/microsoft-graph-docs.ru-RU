---
title: 'accessPackageAssignment: additionalAccess'
description: Получение списка объектов accessPackageAssignment, указывающих на возможное разделение конфликтов обязанностей или доступ к несовместимым пакетам доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6aac3e2ac4ecb3c539a24bf8fa730641e2fa09e1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203795"
---
# <a name="accesspackageassignment-additionalaccess"></a>accessPackageAssignment: additionalAccess
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](../resources/entitlementmanagement-overview.md) получите коллекцию объектов [accessPackageAssignment](../resources/accesspackageassignment.md), указывающих, что целевой пользователь имеет назначение указанному пакету доступа, а также назначение другому, потенциально несовместимого пакета доступа.  Это можно использовать для подготовки к настройке несовместимых пакетов доступа для определенного пакета доступа.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='parameterValue',incompatibleAccessPackageId='parameterValue')
```

## <a name="function-parameters"></a>Параметры функции
В следующей таблице показаны параметры, которые должны быть предоставлены этой функцией.  Два идентификатора пакета доступа должны быть разными.

|Параметр|Тип|Описание|
|:---|:---|:---|
| accessPackageId | Строка |  Указывает идентификатор пакета доступа, для которого вызывающий объект должен получить назначения. Обязательно. |
| incompatibleAccessPackageId | Строка | Конкретный несовместимый пакет доступа, для которого вызывающий объект должен получить только те назначения, в которых пользователь также имеет назначение этому несовместимым пакету доступа. Обязательно. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры `$select``$filter`запроса OData `$expand` и , чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [accessPackageAssignment](../resources/accesspackageassignment.md) в теле отклика.

Если результирующий набор занимает несколько страниц, Microsoft Graph `@odata.nextLink` возвращает эту страницу со свойством в ответе, содержащее URL-адрес следующей страницы результатов. Если это свойство присутствует, продолжайте делать дополнительные `@odata.nextLink` запросы с URL-адресом в каждом ответе, пока не будут возвращены все результаты. Дополнительные сведения см. в статье о [разбиении данных microsoft Graph в приложении](/graph/paging).

## <a name="examples"></a>Примеры

В следующем примере показано, как получить назначения пакетов доступа для пользователей, имеющих назначения обоим пакетам доступа.

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_additionalaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='2506aef1-3929-4d24-a61e-7c8b83d95e6f',incompatibleAccessPackageId='d5d99728-8c0b-4ede-83d2-cf9b0e8dabfb')?$expand=target
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignment-additionalaccess-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignment-additionalaccess-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignment-additionalaccess-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignment-additionalaccess-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackageassignment-additionalaccess-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackageassignment-additionalaccess-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "a61f7889-ae61-4e97-a4dc-e4fa525f5b33",
            "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
            "accessPackageId": "2506aef1-3929-4d24-a61e-7c8b83d95e6f",
            "assignmentPolicyId": "07c7c99d-6cf3-4527-bd05-5fc2ac8e96e7",
            "targetId": "cdbdf152-82ce-479c-b5b8-df90f561d5c7",
            "target": {
                "id": "ebaf071e-c647-42c6-b86f-fbe3625b4b63",
                "objectId": "cdbdf152-82ce-479c-b5b8-df90f561d5c7",
                "displayName": "user1"
            }
        },
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "a7284263-8233-44de-8095-0ee3ff5a1716",
            "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
            "accessPackageId": "2506aef1-3929-4d24-a61e-7c8b83d95e6f",
            "assignmentPolicyId": "07c7c99d-6cf3-4527-bd05-5fc2ac8e96e7",
            "targetId": "79a8f0b6-61dc-41db-b49e-470c278e05b6",
            "target": {
                "id": "9865b0f8-868f-42c6-a49b-3067eb4b2da1",
                "objectId": "79a8f0b6-61dc-41db-b49e-470c278e05b6",
                "displayName": "user2"
            }
        }
  ]
}

```

