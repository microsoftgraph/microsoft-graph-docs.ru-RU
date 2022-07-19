---
title: Обновление объекта profilephoto
description: Обновите фотографию для любого пользователя в клиенте, включая вошедвшего пользователя, или указанную группу, контакт или команду.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: people
author: kevinbellinger
ms.openlocfilehash: 4e930f96076f37ee39ef578c4f091af75cf9acc6
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855758"
---
# <a name="update-profilephoto"></a>Обновление объекта profilephoto

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите фотографию для указанного контакта, группы, команды или пользователя в клиенте. Размер фотографии, которую можно обновить, не должен быть ниже 8 МБ.

Используйте put только для этой операции.

> **Примечание**. При обновлении **фотографии** пользователя эта операция сначала пытается обновить фотографию в Microsoft 365. В случае сбоя (из-за того, что у пользователя нет почтового ящика) этот API попытается обновить фотографию в Azure Active Directory.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="to-update-the-profile-photo-of-a-contact"></a>Обновление фотографии профиля контакта

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)      |   Contacts.ReadWrite           |
|Делегированные (личная учетная запись Майкрософт)      |   Не поддерживается.            |
|Для приложений      |    Contacts.ReadWrite           |

### <a name="to-update-the-profile-photo-of-a-group"></a>Обновление фотографии профиля группы

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)      |   Group.ReadWrite.All           |
|Делегированные (личная учетная запись Майкрософт)      |   Не поддерживается.            |
|Для приложений      |    Group.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-team"></a>Обновление фотографии профиля команды

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                            |
|:---------------------------------------|:-----------------------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | TeamSettingsReadWriteAll, GroupReadWriteAll **, DirectoryReadWriteAll** |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                         |
| Для приложений                            | Не поддерживается.                                                         |

[!INCLUDE [teamwork-permissions-note](../../../includes/teamwork-permissions-note.md)]

### <a name="to-update-the-profile-photo-of-the-signed-in-user"></a>Обновление фотографии профиля вошедшего в систему пользователя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)      |   User.ReadWrite, User.ReadWrite.All           |
|Делегированные (личная учетная запись Майкрософт)      |   Не поддерживается.            |
|Для приложений      |    User.ReadWrite.All           |

> [!NOTE]
> 1. Чтобы обновить фотографию любого пользователя в организации, ваше приложение должно иметь разрешение *User.ReadWrite.All* и вызывать этот API под собственным удостоверением, а не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service). Для обновления фотографии вошедвшего пользователя требуется только *разрешение User.ReadWrite* .
> 2. В настоящее время существует [известная проблема](/graph/known-issues#groups) c доступом к групповым фотографиям с помощью разрешений приложений.
> 3. Обновление фотографии пользователя с помощью microsoft API Graph в настоящее время не поддерживается в Azure AD B2C.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

Чтобы обновить фотографию для команды:

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{teamId}/photo/$value
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | image/jpeg. Обязательный.  |

## <a name="request-body"></a>Тело запроса
Включите в текст запроса двоичные данные фотографии.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика или `204 No Content` код отклика для обновления фотографии команды.

## <a name="examples"></a>Примеры
### <a name="example-1-update-the-profile-photo-of-the-user"></a>Пример 1. Обновление фотографии профиля пользователя
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

### <a name="example-2-update-the-photo-of-a-team"></a>Пример 2. Обновление фотографии команды

#### <a name="request"></a>Запрос
Ниже приведен пример запроса на обновление фотографии команды.

<!-- {
  "blockType": "request",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8491e/photo/$value
Content-type: image/jpeg

Binary data for the image
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
