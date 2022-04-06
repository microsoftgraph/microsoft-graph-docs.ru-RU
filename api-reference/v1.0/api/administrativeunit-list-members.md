---
title: Список участников
description: Используйте этот API для получения списка участников (пользователя и группы) в административном подразделении.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4a87d88bbd69a9a9a93b80968b1719780d2f032e
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672499"
---
# <a name="list-members"></a>Список участников

Пространство имен: microsoft.graph

Используйте этот API для получения списка участников (пользователя и группы) в административном подразделении.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

> Примечание. Чтобы перечислить членов скрытого членства в административном подразделении, требуется разрешение Member.Read.Hidden.

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и коллекцию объектов [](../resources/user.md) пользователей и[/или групп](../resources/group.md) в тексте отклика.  Вместо этого, если вы поместите `$ref` в конце запроса, ответ будет содержать коллекцию `@odata.id` ссылок и URL-адресов для участников.

## <a name="examples"></a>Примеры
##### <a name="list-member-objects"></a>Объекты участников списка
В следующем запросе будут перечисляться члены административного подразделения, возвращающие коллекцию пользователей и/или групп.

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members
```

Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.
 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a>Ссылки на членов списка
Следующий запрос будет перечислять ссылки членов административного подразделения, `@odata.id` возвращая коллекцию ссылок на членов.
```
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```
Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.
 
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
