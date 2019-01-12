---
title: Получение directoryAudit
description: Предоставляет (или получает) определенного элемента журнала аудита Azure Active Directory. Включает в себя журналы аудита, созданных функцией различных служб в Azure Active Directory пользователя, приложения, устройств и управление группами, привилегированной управления удостоверениями, обзоры доступа, условия использования, защиту, управление паролями (SSPR и администрирования сброс пароля ), Самообслуживания и т.д группы управления...
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 43b478aed8ac6beb28d9db53d0c97c01b34f173a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956320"
---
# <a name="get-directoryaudit"></a>Получение directoryAudit
Предоставляет (или получает) определенного элемента журнала аудита Azure Active Directory. Включает в себя журналы аудита, созданных функцией различных служб в Azure Active Directory пользователя, приложения, устройств и управление группами, привилегированной управления удостоверениями, обзоры доступа, условия использования, защиту, управление паролями (SSPR и администрирования сброс пароля ), Самообслуживания и т.д группы управления...

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
GET /auditLogs/directoryAudits/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает следующие параметры запроса OData для настройки ответа. Проверьте [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для порядок использования этих параметров.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` объект [directoryAudit](../resources/directoryaudit.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits/{id}
```
##### <a name="response"></a>Ответ
Ниже приведен пример отклика. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "dax59xfb-5xfa-4x92-8x38-6e1fx7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "72xx09ae-1x37-49x7-9xfe-e3xx964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6xx2-4xx4-8xxd-cxxfdxx5xx95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
            "id": "1x0exxf5-3xx1-4xxb-9xx0-d4xx572xxbb7",
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
