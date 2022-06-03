---
title: Список участников
description: Используйте этот API для получения списка участников (пользователей, групп или устройств) в административной единице.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4de66a36c8399a233b5dabdd65041415c2abfe42
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884299"
---
# <a name="list-members"></a>Список участников

Пространство имен: microsoft.graph

Используйте этот API для получения списка участников (пользователей, групп или устройств) в административной единице.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

> Примечание. Чтобы получить список членов скрытого членства в административной единице, требуется разрешение Member.Read.Hidden.

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод (при использовании без `$ref`) поддерживает параметры [запроса OData](/graph/query-parameters) для настройки ответа, `$search`включая , `$count`и `$filter`. Приведение OData также включено. Например, можно выполнить приведение, чтобы получить только пользователей, которые являются членами административной единицы. 

`$search` поддерживается только **для свойств displayName** **и** description. Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |
| ConsistencyLevel  | необязательный. Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пользователя](../resources/user.md), [группы](../resources/group.md) [или устройства в](../resources/device.md) тексте отклика. При `$ref` добавлении в конце запроса возвращается коллекция только `@odata.id` URL-адресов элементов.

## <a name="examples"></a>Примеры

### <a name="example-1-list-member-objects"></a>Пример 1. Перечисление объектов-членов

#### <a name="request"></a>Запрос
Следующий запрос выводит список членов административной единицы, возвращая коллекцию пользователей, групп и устройств.

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit_members"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
        {
            "@odata.type": "#microsoft.graph.device",
            "id": "7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac",
            "accountEnabled": true,
            "deviceId": "6fa60d52-01e7-4b18-8055-4759461fc16b",
            "displayName": "Test Windows device",
            "operatingSystem": "Windows"
        },
        {
            "@odata.type": "#microsoft.graph.device",
            "id": "c530e1f6-7b4c-4313-840e-cf1a99ec3b38",
            "accountEnabled": false,
            "deviceId": "4c299165-6e8f-4b45-a5ba-c5d250a707ff",
            "displayName": "Test Linux device",
            "operatingSystem": "linux"
        }
    ]
}
```

### <a name="example-2-list-member-references"></a>Пример 2. Ссылки на элементы списка

#### <a name="request"></a>Запрос
Следующий запрос выводит список ссылок на элементы административной единицы, `@odata.id` возвращая коллекцию ссылок на члены.

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit_member_refs"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
