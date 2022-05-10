---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
ms.localizationpriority: medium
author: KuiGithui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 32db80ebdd5a559acf79976916aeb39f7d941ece
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2022
ms.locfileid: "65294021"
---
# <a name="get-organization"></a>Получение организации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей организации, прошедшей проверку подлинности.

Так как ресурс **organization** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете получить настраиваемые свойства и данные расширения в экземпляре **организации**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложения | Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All |

> **Примечание.** Приложения с разрешением User.Read могут считывать только такие свойства организации, как **id**, **displayName** и **verifiedDomains**.  Для всех остальных свойств возвращается значение `null`. Считать все свойства можно с помощью Organization.Read.All.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает только [параметр запросов OData](/graph/query-parameters) `$select` для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию из одного объекта [organization](../resources/organization.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/84841066-274d-4ec0-a5c1-276be684bdd3
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organization-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-organization-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
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
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
