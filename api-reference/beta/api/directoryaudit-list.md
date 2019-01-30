---
title: Перечисление directoryAudits
description: Представляет список журналов аудита, созданный Azure Active Directory. Включает журналы аудита, созданные различными службами Azure Active Directory, например службой управления пользователями, приложениями, устройствами и группами, управления привилегированными пользователями, проверки доступа, условий использования, защиты идентификации, управления паролями (SSPR и сброс паролей администраторов), самостоятельного управления группами и т. д.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: df6a737696c855cd60e396c6571169f8c46b3952
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642039"
---
# <a name="list-directoryaudits"></a>Перечисление directoryAudits

Представляет список журналов аудита, созданный Azure Active Directory. Включает журналы аудита, созданные различными службами Azure Active Directory, например службой управления пользователями, приложениями, устройствами и группами, управления привилегированными пользователями, проверки доступа, условий использования, защиты идентификации, управления паролями (SSPR и сброс паролей администраторов), самостоятельного управления группами и т. д.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AuditLog.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Для приложений | AuditLog.Read.All | 

Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).

|Имя     |Описание                            |Пример|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Фильтрует результаты (строки). |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|Задает размер страницы результатов.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Список атрибутов, поддерживаемых параметром $filter
|Имя атрибута |Поддерживаемые операторы|
|:----------------|:------|
|activityDisplayName| eq, startswith|
|activityDateTime| eq, ge, le|
|loggedByService|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq, startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/appDisplayName| eq|
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
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "7283X9ae-1a37-4937-9aex-e35d964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6x92-42x4-8x6d-cfxfdfx57f95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
            "id": "1f0ex8f5-3x61-4x6b-9x50-d4xx572f2bb7",
            "displayName": null,
            "modifiedProperties": [],
            "userPrincipalName": "jdoe@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
