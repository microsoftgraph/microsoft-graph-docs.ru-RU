---
title: Список directoryAudits
description: Список журналов аудита, созданных функцией Azure Active Directory. Включает в себя журналы аудита, созданных функцией различных служб в Azure Active Directory пользователя, приложения, устройств и управление группами, привилегированной управления удостоверениями, обзоры доступа, условия использования, защиту, управление паролями (SSPR и администрирования сброс пароля ), Самообслуживания и т.д группы управления...
localization_priority: Priority
ms.openlocfilehash: 08b9cd5ded6771883a6d0f1129cf44a808515f8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829339"
---
# <a name="list-directoryaudits"></a>Список directoryAudits

Список журналов аудита, созданных функцией Azure Active Directory. Включает в себя журналы аудита, созданных функцией различных служб в Azure Active Directory пользователя, приложения, устройств и управление группами, привилегированной управления удостоверениями, обзоры доступа, условия использования, защиту, управление паролями (SSPR и администрирования сброс пароля ), Самообслуживания и т.д группы управления...

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AuditLog.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Для приложений | AuditLog.Read.All | 

Кроме того приложения должны быть [правильно зарегистрирован](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) для Azure AD.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает следующие параметры запроса OData для настройки ответа. Проверьте [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для порядок использования этих параметров.

|Имя     |Описание                            |Пример|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Фильтрует результаты (строки). |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|Задает размер страницы результатов.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Извлекает следующую страницу результатов из результатов наборы данных, которые охватывают несколько страниц.|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Список атрибутов, поддерживаемых $filter параметром
|Имя атрибута |Поддерживаемые операторы|
|:----------------|:------|
|activityDisplayName| EQ, startswith|
|activityDateTime| le EQ, ge,|
|loggedByService|eq|
|initiatedBy/пользователь|eq|
|initiatedBy/пользователей/displayName| eq|
|initiatedBy/пользователей/userPrincipalName| EQ, startswith|
|initiatedBy/приложение/appId| eq|
|initiatedBy/приложение/appDisplayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| EQ, startswith|
## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [directoryAudit](../resources/directoryaudit.md) в теле ответа.
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
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
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
