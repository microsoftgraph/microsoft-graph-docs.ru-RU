---
title: 'directoryObject: checkMemberGroups'
description: Проверьте членство в указанном списке групп и вернись из этого списка тех групп, участником которых является указанный пользователь, группа, руководитель службы, организационный контакт или объект каталога.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1efadd27c8e3a9cd2100734fc5b2d781fd451542
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61125060"
---
# <a name="directoryobject-checkmembergroups"></a>directoryObject: checkMemberGroups

Пространство имен: microsoft.graph

Проверьте членство в указанном списке групп и вернись из этого списка тех групп, [](../resources/orgcontact.md)членом которых [](../resources/directoryobject.md) является указанный [пользователь,](../resources/user.md) [группа,](../resources/group.md)руководитель службы, [](../resources/serviceprincipal.md)организационный контакт или объект каталога. Это транзитивная функция.

В одном запросе можно проверять до 20 групп. Эта функция поддерживает все группы, которые предусмотрены в Azure AD. Поскольку Microsoft 365 группы не могут содержать другие группы, членство Microsoft 365 группы всегда является прямым.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All, User.Read.All, Directory.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All, Directory.Read.All |

В следующей таблице перечислены типы разрешений, которые можно использовать для различных сценариев.

| Сценарий | Разрешения |
|:-|:-|
| Для получения членства в группе для пользователя, вписаного в группу | Используйте один из следующих наборов разрешений: <br/> <li> **User.Read** и **GroupMember.Read.All** <li>**User.Read** и **Group.Read.All** |
| Для получения членства в группе для любого пользователя | Используйте один из следующих наборов разрешений: <br/> <li> **User.ReadBasic.All** и **GroupMember.Read.All** <li>**User.Read.All** и **GroupMember.Read.All** <li>**User.ReadBasic.All** и **Group.Read.All** <li>**User.Read.All** и **Group.Read.All** |
| Чтобы получить членство в группе для группы | Используйте разрешение **GroupMember.Read.All** или **Group.Read.All.** |
| Чтобы получить членство в группе для директора службы | Используйте один из следующих наборов разрешений <br/> <li>**Application.ReadWrite.All** и **GroupMember.Read.All** <li>**Application.ReadWrite.All** и **Group.Read.All** |
| Чтобы получить членство в группе для объекта каталога | Используйте **разрешение Directory.Read.All.** |

<!-- These tables will replace the data in lines 22-36 to help with the tooling that parses permissions tables.
+ Current data is copy-pasted from incorrect files/file names
+ To validate these permissions against lines 32-36

### Group memberships for a directory object

| Permission type                        | Permissions (from least to most privileged)           |
|:---------------------------------------|:------------------------------------------------------|
| Delegated (work or school account)     | User.ReadBasic.All, User.Read.All, Directory.Read.All |
| Delegated (personal Microsoft account) | Not supported.                                        |
| Application                            | User.Read.All, Directory.Read.All                     |

### Group memberships for a user

| Permission type | Permissions (from least to most privileged) |
|:-|:-|
| Delegated (work or school account) | User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application | User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for a group

| Permission type | Permissions (from least to most privileged) |
|:-|:-|
| Delegated (work or school account) | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for a service principal

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for an organizational contact

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All   |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Directory.Read.All, Directory.ReadWrite.All |

-->

## <a name="http-request"></a>HTTP-запрос

Членство в группах для объекта каталога (пользователя, группы, руководителя службы или организационного контакта).
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/checkMemberGroups
```

Членство в группе для подписанного пользователя или других пользователей.
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
```

Членство в группе для группы.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```

Членство в группе для директора службы.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups
```

Членство в группе для организационного контакта.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|groupIds|Коллекция строк|Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Пример 1. Проверка членства группы для объекта каталога

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e/checkMemberGroups
Content-type: application/json

{
    "groupIds": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

#### <a name="response"></a>Отклик

Ниже приводится пример ответа

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Пример 2. Проверка членства в группе для пользователя, заявив о регистрации

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

#### <a name="response"></a>Отклик

Ниже приводится пример ответа
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

