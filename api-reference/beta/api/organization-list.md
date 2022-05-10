---
title: Список организаций
description: Получение списка объектов организаций.
ms.localizationpriority: medium
author: KuiGithui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4da11a8c4a8db104d3909183f15c3fa68e733aec
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2022
ms.locfileid: "65294049"
---
# <a name="list-organization"></a>Список организаций

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов организаций.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organization-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-organization-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
    "value": [
        {
            "id": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "deletedDateTime": null,
            "businessPhones": [
                "425-555-0100"
            ],
            "city": null,
            "country": null,
            "countryLetterCode": "NL",
            "createdDateTime": "2021-08-02T10:30:06Z",
            "displayName": "Contoso",
            "isMultipleDataLocationsForServicesEnabled": null,
            "marketingNotificationEmails": [],
            "onPremisesLastSyncDateTime": null,
            "onPremisesSyncEnabled": null,
            "postalCode": null,
            "preferredLanguage": "en",
            "securityComplianceNotificationMails": [],
            "securityComplianceNotificationPhones": [],
            "state": null,
            "street": null,
            "technicalNotificationMails": [
                "admin@contoso.com"
            ],
            "tenantType": "AAD",
            "directorySizeQuota": {
                "used": 698,
                "total": 50000
            },
            "assignedPlans": [
                {
                    "assignedDateTime": "2022-04-03T02:46:42Z",
                    "capabilityStatus": "Deleted",
                    "service": "Adallom",
                    "servicePlanId": "932ad362-64a8-4783-9106-97849a1a30b9"
                },
                {
                    "assignedDateTime": "2022-04-03T02:46:42Z",
                    "capabilityStatus": "Deleted",
                    "service": "MultiFactorService",
                    "servicePlanId": "8a256a2b-b617-496d-b51b-e76466e88db0"
                },
                {
                    "assignedDateTime": "2021-08-02T10:36:57Z",
                    "capabilityStatus": "Enabled",
                    "service": "exchange",
                    "servicePlanId": "113feb6c-3fe4-4440-bddc-54d774bf0318"
                },
                {
                    "assignedDateTime": "2021-08-02T10:36:02Z",
                    "capabilityStatus": "Deleted",
                    "service": "SCO",
                    "servicePlanId": "882e1d05-acd1-4ccb-8708-6ee03664b117"
                }
            ],
            "privacyProfile": {
                "contactEmail": "",
                "statementUrl": ""
            },
            "provisionedPlans": [
                {
                    "capabilityStatus": "Deleted",
                    "provisioningStatus": "Success",
                    "service": "Adallom"
                },
                {
                    "capabilityStatus": "Enabled",
                    "provisioningStatus": "Success",
                    "service": "exchange"
                }
            ],
            "verifiedDomains": [
                {
                    "capabilities": "Email, OfficeCommunicationsOnline",
                    "isDefault": true,
                    "isInitial": true,
                    "name": "Contoso.com",
                    "type": "Managed"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
