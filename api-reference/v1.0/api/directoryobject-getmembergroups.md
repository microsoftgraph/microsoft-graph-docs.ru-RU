---
title: 'directoryObject: getMemberGroups'
description: Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9ccb8db35f8aadf89859afc130377287f4bcce1b
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123560"
---
# <a name="directoryobject-getmembergroups"></a>directoryObject: getMemberGroups

Пространство имен: microsoft.graph

Верни все группы, в которые входит указанный [пользователь,](../resources/user.md) [](../resources/directoryobject.md) [группа,](../resources/group.md)руководитель [службы,](../resources/serviceprincipal.md)организационный контакт [или](../resources/orgcontact.md)объект каталога. Это транзитивная функция.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, Directory.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, Directory.Read.All |

Используйте руководство по следующим сценариям, чтобы определить, какие типы разрешений использовать:

| Сценарий | Разрешения на использование |
|:-|:-|
| Для получения членства в группе для пользователя, вписаного в группу | Используйте один из следующих наборов разрешений: <br/> <li> **User.Read** и **GroupMember.Read.All** <li>**User.Read** и **Group.Read.All** |
| Для получения членства в группе для любого пользователя | Используйте один из следующих наборов разрешений: <br/> <li> **User.ReadBasic.All** и **GroupMember.Read.All** <li>**User.Read.All** и **GroupMember.Read.All** <li>**User.ReadBasic.All** и **Group.Read.All** <li>**User.Read.All** и **Group.Read.All** |
| Чтобы получить членство в группе для группы | Используйте разрешение **GroupMember.Read.All** или **Group.Read.All.** |
| Чтобы получить членство в группе для объекта каталога | Используйте **разрешение Directory.Read.All.** |

<!-- These tables will replace the data in lines 22-36 to help with the tooling that parses permissions tables.
+ Current data is copy-pasted from incorrect files/file names
+ To validate these permissions against lines 32-36

### Group memberships for a directory object

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All |

### Group memberships for a user

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All |

### Group memberships for a group

| Permission type                        | Permissions (from least to most privileged)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Delegated (work or school account)     | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported.                                                                              |
| Application                            | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All                             |

### Group memberships for a service principal

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for an organizational contact

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Directory.Read.All, Directory.ReadWrite.All |

-->

## <a name="http-request"></a>HTTP-запрос

Членство в группах для объекта каталога (пользователя, группы, руководителя службы или организационного контакта).
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/getMemberGroups
```

Членство в группе для подписанного пользователя или других пользователей.
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
```

Членство в группе для группы.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```

Членство в группе для директора службы.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups
```

Членство в группе для организационного контакта.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type   | application/json  |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|securityEnabledOnly|Логическое| `true` чтобы указать, что должны возвращаться только группы безопасности, в которые входит объект; чтобы указать, что все роли групп и каталогов, в которые входит объект, `false` должны быть возвращены. `true` могут быть указаны только для пользователей или директоров служб для возврата групп с поддержкой безопасности. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Пример 1. Проверка членства группы для объекта каталога

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/0049d944-a805-4680-9f54-3ab292090309/getMemberGroups
Content-type: application/json

{
    "securityEnabledOnly": false
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
        "a8daa1fb-d24c-47d0-9e9e-c99e83394e3e"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Пример 2. Проверка членства в группе для пользователя, заявив о регистрации

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

#### <a name="response"></a>Отклик

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
        "6239671a-0db6-4e8b-9d2f-f280efb5a181",
        "2e2f1227-1586-45ae-bf51-fccc1de72625",
        "1dae9306-be75-4c3c-99ec-0316a4342c84",
        "0e2d1bbb-76f8-4140-bda7-2a858b74507e",
        "0049d944-a805-4680-9f54-3ab292090309",
        "a8daa1fb-d24c-47d0-9e9e-c99e83394e3e",
        "6f204729-1b8f-4067-bcc9-98fb6c069ffd",
        "59afd38d-441a-4358-b074-8b9b1e7de52f",
        "64ed3df3-53c7-4d4d-ac5c-5c8dd4dafe33",
        "8b676bab-4b1e-419e-a253-7f5aca97d739",
        "be4ef325-9fa8-40d7-b375-4758853ddf52",
        "f5987b5a-61f6-4c31-9fa2-7bfb845c8d2a"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

