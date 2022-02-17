---
title: Список участников
description: Используйте этот API, чтобы получить список участников (пользователей, групп и устройств) в административном подразделении.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a3e591e164f92557c1661a3f3c3318508d054e7
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878633"
---
# <a name="list-members"></a>Список участников

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API, чтобы получить список участников (пользователей, групп и устройств) в административном подразделении.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

> Примечание. Чтобы перечислить членов скрытого членства в административном подразделении, требуется разрешение Member.Read.Hidden.

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод (если используется без `$ref`) поддерживает параметры [запроса OData](/graph/query-parameters) , чтобы помочь настроить ответ, `$search`в том числе , `$count`и `$filter`. Также включена литье OData, например, чтобы получить только пользователей, которые являются членом административного подразделения. 

`$search` поддерживается только **в свойствах displayName** **и description** . Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Заголовки запросов
| Заголовок      |Значение|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |
| ConsistencyLevel  | необязательный. Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы `200 OK` этот метод возвращает код отклика и коллекцию объектов [пользователя, группы](../resources/user.md) или [](../resources/device.md) устройств в тексте ответа. [](../resources/group.md) Добавление `$ref` в конце запроса возвращает коллекцию `@odata.id` только URL-адресов участников.

## <a name="examples"></a>Примеры
### <a name="example-1-list-member-objects"></a>Пример 1. Объекты участников списка

#### <a name="request"></a>Запрос
В следующем запросе будут перечисляться члены административного подразделения, возвращающие коллекцию пользователей и/или групп.

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
 
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

### <a name="example-2-list-member-references"></a>Пример 2. Ссылки на членов списка

#### <a name="request"></a>Запрос

Следующий запрос будет перечислять ссылки членов административного подразделения, `@odata.id` возвращая коллекцию ссылок на членов.

```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```


