---
title: Перечисление directoryAudits
description: Описывает метод списка ресурса directoryAudit (сущности) из microsoft API Graph (бета-версия).
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: dd8fe4c8923dac46cd9e9d7854d64015a5319390
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437411"
---
# <a name="list-directoryaudits"></a>Перечисление directoryAudits

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка журналов аудита, созданных Azure Active Directory. К ним относятся журналы аудита, созданные различными службами в Azure AD, включая управление пользователями, приложениями, устройствами и группой, управление привилегированными пользователями (PIM), проверки доступа, условия использования, защиту идентификации, управление паролями (сброс пароля SSPR и администратора) и управление группой самообслуживания.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AuditLog.Read.All и Directory.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Приложение | AuditLog.Read.All и Directory.Read.All | 

> [!IMPORTANT]
> Этот API имеет известная проблема и в настоящее время требует согласия на разрешения **AuditLog.Read.All** и **Directory.Read.All**.[](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports)

Кроме того, приложения должны быть [правильно зарегистрированы](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает следующие параметры запроса OData для настройки ответа. Дополнительные сведения об использовании этих параметров см. в разделе параметров [запроса OData](/graph/query-parameters).

|Параметр     |Описание                            |Пример|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Фильтрует результаты (строки). |`/auditLogs/directoryAudits?$filter=activityDateTime le 2018-01-24`<br>`/auditLogs/directoryAudits?$filter=targetResources/any(x: startswith(x/displayName, 'def'))` |
|[$top](/graph/query-parameters#top-parameter)|Задает размер страницы результатов.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.|`/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a>Атрибуты, поддерживаемые $filter параметра

|Атрибут        |Поддерживаемые операторы|
|:----------------|:------|
|activityDisplayName| eq, startswith|
|activityDateTime| eq, ge, le|
|loggedByService|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq, startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/displayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| eq, startswith|

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryAudit](../resources/directoryaudit.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryaudits-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryaudits-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Directory_504a302a-8f2d-418d-b7df-bf77de6ed831_M1N6X_27777783",
    "category": "UserManagement",
    "correlationId": "504a302a-8f2d-418d-b7df-bf77de6ed831",
    "result": "success",
    "resultReason": "",
    "activityDisplayName": "Update user",
    "activityDateTime": "2022-06-21T23:25:00.1458248Z",
    "loggedByService": "Core Directory",
    "operationType": "Update",
    "userAgent": null,
    "initiatedBy": {
        "app": null,
        "user": {
            "id": "2c940657-1026-4386-bcfd-3176637ba01f",
            "displayName": "Test Admin",
            "userPrincipalName": "tadmin@contoso.com",
            "ipAddress": "",
            "userType": "Member",
            "homeTenantId": null,
            "homeTenantName": null
        }
    },
    "targetResources": [
        {
            "id": "2c940657-1026-4386-bcfd-3176637ba01f",
            "displayName": "Test User",
            "type": "User",
            "userPrincipalName": "tuser@contoso.com",
            "groupType": null,
            "modifiedProperties": [
                {
                    "displayName": "StrongAuthenticationMethod",
                    "oldValue": "[{\"MethodType\":6,\"Default\":true},{\"MethodType\":7,\"Default\":false}]",
                    "newValue": "[{\"MethodType\":7,\"Default\":false},{\"MethodType\":6,\"Default\":true},{\"MethodType\":0,\"Default\":false},{\"MethodType\":5,\"Default\":false}]"
                },
                {
                    "displayName": "Included Updated Properties",
                    "oldValue": null,
                    "newValue": "\"StrongAuthenticationMethod\""
                },
                {
                    "displayName": "TargetId.UserType",
                    "oldValue": null,
                    "newValue": "\"Member\""
                }
            ]
        }
    ],
    "additionalDetails": [
        {
            "key": "UserType",
            "value": "Member"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
