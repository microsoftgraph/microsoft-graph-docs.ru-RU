---
title: Получение объекта servicePrincipal
description: Получение свойств и связей объекта serviceprincipal.
author: sureshja
ms.localizationpriority: high
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 933a7cd6f4cee0fdb0abdc78296eaac949824948
ms.sourcegitcommit: 7deb4fad6acc69fd6bc02cd4e2f6774de5784c97
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2022
ms.locfileid: "62894700"
---
# <a name="get-serviceprincipal"></a>Получение объекта servicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей объекта [servicePrincipal](../resources/serviceprincipal.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

> [!NOTE]
> Субъект-служба может получить сведения о собственном приложении и субъекте-службе без предоставления разрешений приложения.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика. Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

По умолчанию этот API не возвращает значение открытого ключа **key** в свойстве **keyCredentials**, если в запросе `$select` не указан параметр **keyCredentials**.
Например, `$select=id,appId,keyCredentials`.

При использовании `$select` с целью получения **keyCredentials** для субъектов-служб применяется ограничение регулирования в количестве 150 запросов в минуту для каждого клиента.

## <a name="request-headers"></a>Заголовки запросов
| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-properties-of-the-specified-service-principal"></a>Пример 1. Получение свойств указанного субъекта-службы

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-serviceprincipal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-serviceprincipal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
        "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appDisplayName": "My App",
        "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
        "applicationTemplateId": null,
        "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
        "appRoleAssignmentRequired": false,
        "disabledByMicrosoftStatus": null,
        "displayName": "foo",
        "errorUrl": null,
        "homepage": null,
        "loginUrl": null,
        "logoutUrl": null,
        "notificationEmailAddresses": [],
        "preferredSingleSignOnMode": null,
        "preferredTokenSigningKeyEndDateTime": null,
        "preferredTokenSigningKeyThumbprint": null,
        "publisherName": "Contoso",
        "replyUrls": [],
        "samlMetadataUrl": null,
        "samlSingleSignOnSettings": null,
        "servicePrincipalNames": [
            "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
        ],
        "signInAudience": "AzureADandPersonalMicrosoftAccount",
        "tags": [],
        "verifiedPublisher": {
            "displayName": "publisher_contoso",
            "verifiedPublisherId": "9999999",
             "addedDateTime": "2021-04-24T17:49:44Z"
        },
        "addIns": [],
        "api": {
            "resourceSpecificApplicationPermissions": []
        },
        "appRoles": [],
        "info": {
            "termsOfServiceUrl": null,
            "supportUrl": null,
            "privacyStatementUrl": null,
            "marketingUrl": null,
            "logoUrl": null
        },
        "keyCredentials": [],
        "publishedPermissionScopes": [],
        "passwordCredentials": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

### <a name="example-2-get-the-custom-security-attribute-assignments-of-the-specified-service-principal"></a>Пример 2. Получение назначений настраиваемых атрибутов безопасности указанного субъекта-службы

В следующем примере выполняется получение настраиваемых атрибутов безопасности указанного субъекта-службы.

Атрибут №1

+ Набор атрибутов: `Engineering`
+ Атрибут: `Project`
+ Тип данных атрибута: коллекция строк
+ Значение атрибута: `["Baker","Cascade"]`

Атрибут №2

+ Набор атрибутов: `Engineering`
+ Атрибут: `CostCenter`
+ Тип данных атрибута: коллекция целых чисел
+ Значение атрибута: `[1001]`

Атрибут №3

+ Набор атрибутов: `Engineering`
+ Атрибут: `Certification`
+ Тип данных атрибута: логический
+ Значение атрибута: `true`

Атрибут №4

+ Набор атрибутов: `Marketing`
+ Атрибут: `Level`
+ Тип данных атрибута: строка
+ Значение атрибута: `"Public"`

Чтобы получить назначения настраиваемых атрибутов безопасности, вызывающему субъекту должна быть назначена роль читателя назначения атрибутов или администратора назначения атрибутов, а также должно быть предоставлено разрешение *CustomSecAttributeAssignment.Read.All* или *CustomSecAttributeAssignment.ReadWrite.All*.

#### <a name="request"></a>Запрос




# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_customsecurityattributes"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}?$select=customSecurityAttributes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-customsecurityattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-customsecurityattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-customsecurityattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-customsecurityattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-serviceprincipal-customsecurityattributes-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-serviceprincipal-customsecurityattributes-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(customSecurityAttributes)/$entity",
    "customSecurityAttributes": {
        "Engineering": {
            "@odata.type": "#microsoft.graph.customSecurityAttributeValue",
            "Project@odata.type": "#Collection(String)",
            "Project": [
                "Baker",
                "Cascade"
            ],
            "CostCenter@odata.type": "#Collection(Int32)",
            "CostCenter": [
                1001
            ],
            "Certification": true
        },
        "Marketing": {
            "@odata.type": "#microsoft.graph.customSecurityAttributeValue",
            "Level": "Public"
        }
    }
}
```

Если субъекту-службе не назначены настраиваемые атрибуты безопасности или у вызывающего субъекта нет прав доступа, отклик будет выглядеть указанным ниже образом.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(customSecurityAttributes)/$entity",
    "customSecurityAttributes": null
}
```
