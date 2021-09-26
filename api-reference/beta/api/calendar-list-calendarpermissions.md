---
title: Список calendarPermissions
description: 'Получите коллекцию ресурсов calendarPermission, описывающих удостоверения и роли пользователей, с которыми указанный календарь был общим или делегирован. '
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 21b7beec7e6fbd74a2021dbb3a8d8db8939064a6
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777385"
---
# <a name="list-calendarpermissions"></a>Список calendarPermissions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите коллекцию [ресурсов calendarPermission,](../resources/calendarpermission.md) описывающих удостоверения и роли пользователей, с которыми указанный календарь был общим или делегирован. Здесь календарь может быть календарем пользователя или групповым календарем.

## <a name="permissions"></a>Разрешения

В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Календарь | Делегированные (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Приложение |
|:-----|:-----|:-----|:-----|
| календарь пользователя | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite |
| календарь группы | Group.Read.All, Group.ReadWrite.All | Не поддерживается. | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Список указанных разрешений основного календаря пользователя:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions
```

Список указанных разрешений группового календаря:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions
```

Список указанных разрешений пользовательского календаря, который содержит указанное событие:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` **calendarPermission** в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions
```
### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('458d4c95-124e-49da-ba9d-1dd0387e682e')/calendar/calendarPermissions",
    "value": [
        {
            "id": "RXhjaGFuZ2VQdWJsaXNoZWRVc2VyLmFkbWluQE0zNjVCODc3NzE5Lm9ubWljcm9zb2Z0LmNvbQ==",
            "isRemovable": true,
            "isInsideOrganization": false,
            "role": "read",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read"
            ],
            "emailAddress": {
                "name": "admin@M365B877719.onmicrosoft.com",
                "address": "admin@M365B877719.onmicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->