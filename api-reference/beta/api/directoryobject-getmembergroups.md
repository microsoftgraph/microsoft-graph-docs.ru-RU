---
title: 'directoryObject: getMemberGroups'
description: Верни все группы, в которые входит указанный пользователь, группа, руководитель службы, организационный контакт, устройство или объект каталога. Это транзитивная функция.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0b282c5f8bb9556c371c40364bb41eb6e4217d3f
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671204"
---
# <a name="directoryobject-getmembergroups"></a>directoryObject: getMemberGroups

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Верни все групповые ID для [групп, в](../resources/user.md)[](../resources/directoryobject.md) которые входит указанный [пользователь, группа](../resources/group.md)[, руководитель](../resources/serviceprincipal.md) службы[, организационный](../resources/orgcontact.md) [контакт, устройство](../resources/device.md) или объект каталога. Это транзитивная функция.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="group-memberships-for-a-directory-object"></a>Членство в группе для объекта каталога

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, Directory.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, Directory.Read.All |

### <a name="group-memberships-for-a-user"></a>Членство в группе для пользователя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, Directory.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, Directory.Read.All |

### <a name="group-memberships-for-a-group"></a>Членство в группе для группы

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                              |
| Для приложений                            | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All                             |

### <a name="group-memberships-for-a-service-principal"></a>Членство в группе для директора службы

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

### <a name="group-memberships-for-an-organizational-contact"></a>Членство в группе для организационного контакта

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

### <a name="group-memberships-for-a-device"></a>Членство в группе для устройства

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Device.Read.All, Directory.Read.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |


<!--
The following table lists the permission types to use for different scenarios.

| Scenario | Permissions |
|:-|:-|
| To get group memberships for the signed-in user | Use one of the following sets of permissions: <br/> <li> **User.Read** and **GroupMember.Read.All** <li>**User.Read** and **Group.Read.All** |
| To get group memberships for any user | Use one of the following sets of permissions: <br/> <li> **User.ReadBasic.All** and **GroupMember.Read.All** <li>**User.Read.All** and **GroupMember.Read.All** <li>**User.ReadBasic.All** and **Group.Read.All** <li>**User.Read.All** and **Group.Read.All** |
| To get group memberships for a group | Use either the **GroupMember.Read.All** or **Group.Read.All** permission. |
| To get group memberships for a service principal | Use one of the following sets of permissions <br/> <li>**Application.ReadWrite.All** and **GroupMember.Read.All** <li>**Application.ReadWrite.All** and **Group.Read.All** |
| To get group memberships for a directory object | Use the **Directory.Read.All** permission. |
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

Членство в группе для устройства.
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/getMemberGroups
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
|securityEnabledOnly|Boolean| `true` чтобы указать, что должны возвращаться только группы безопасности, в которые входит объект; `false` чтобы указать, что все роли групп и каталогов, в которые входит объект, должны быть возвращены. `true` могут быть указаны только для пользователей или директоров служб для возврата групп с поддержкой безопасности. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Пример 1. Проверка членства группы для объекта каталога

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/directoryObjects/0049d944-a805-4680-9f54-3ab292090309/getMemberGroups
Content-type: application/json

{
    "securityEnabledOnly": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-getmembergroups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-getmembergroups-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "a8daa1fb-d24c-47d0-9e9e-c99e83394e3e"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Пример 2. Проверка членства в группе для пользователя, заявив о регистрации

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-getmembergroups-me-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-getmembergroups-me-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "6239671a-0db6-4e8b-9d2f-f280efb5a181",
        "2e2f1227-1586-45ae-bf51-fccc1de72625",
        "f5987b5a-61f6-4c31-9fa2-7bfb845c8d2a"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


