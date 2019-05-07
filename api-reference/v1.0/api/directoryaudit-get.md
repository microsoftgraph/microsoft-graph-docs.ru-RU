---
title: Получение directoryAudit
description: Описывает метод Get ресурса Директоряудит (Entity) из API Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: df4b64f616cc902daaa764b74be4a16bea84b9fd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630155"
---
# <a name="get-directoryaudit"></a>Получение directoryAudit

Получение конкретного элемента журнала аудита Azure Active Directory. Сюда входит элемент журнала аудита, созданный различными службами в Azure Active Directory, такими как пользователь, приложение, Управление устройствами и группами, управление правами на доступ к данным, обзоры доступа, условия использования, защита удостоверений, управление паролями ( самообслуживания и сброс паролей администратора), самостоятельное управление группами и т. д.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Аудитлог. Read. ALL и Directory. Read. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Для приложений | AuditLog.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки отклика. Сведения о том, как использовать эти параметры, представлены в разделе [Параметры запроса OData](/graph/query_parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директоряудит](../resources/directoryaudit.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits/{id}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryaudit"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218
```

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditlogs/directoryaudits",
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
                "id": "728309ae-1a37-4937-9afe-e35d964db09b",
                "displayName": "Audry Oliver",
                "userPrincipalName": "bob@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResource": [{
            "id": "ef7e527d-6c92-4234-8c6d-cf6fdfb57f95",
            "displayName": "Example.com",
            "Type": "Group",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync" }],
            "groupType": "unifiedGroups"
            }],
        }, {
            "id": "1f0e98f5-3161-4c6b-9b50-d488572f2bb7",
            "displayName": null,
            "Type": "User",
            "modifiedProperties": [],
            "userPrincipalName": "example@contoso.com"
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
  "description": "Get directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
