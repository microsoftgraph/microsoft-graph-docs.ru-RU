---
title: Обновление profilePhoto
description: Обновление фотографии вошедшего пользователя либо указанной группы или контакта.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fb3ccef7898305dbd76f891ff85019da853187dc
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645478"
---
# <a name="update-profilephoto"></a>Обновление profilePhoto

Пространство имен: microsoft.graph

Обновление фотографии вошедшего **пользователя** либо указанной **группы** или **контакта**.

Из-за текущего ограничения в 4 МБ на общий размер каждого запроса REST размер фотографии, которую можно добавить, также ограничен 4 МБ. Ниже приведены поддерживаемые измерения для фотографий HD на Exchange Online: `48x48`, , , `96x96`, `120x120`, `240x240`, `360x360`, и `648x648``432x432``504x504`. `64x64`

В версии 1.0 для этой операции можно использовать запросы PATCH и PUT.

> **Примечание:** Эта операция поддерживает только рабочие или учебные почтовые ящики пользователя, а не личные почтовые ящики.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="to-update-the-profile-photo-of-the-signed-in-user"></a>Обновление фотографии профиля вошедшего в систему пользователя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)      |   User.ReadWrite, User.ReadWrite.All           |
|Делегированные (личная учетная запись Майкрософт)      |   Не поддерживается.            |
|Для приложений      |    User.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-group"></a>Обновление фотографии профиля группы

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)      |   Group.ReadWrite.All           |
|Делегированные (личная учетная запись Майкрософт)      |   Не поддерживается.            |
|Для приложений      |    Group.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-contact"></a>Обновление фотографии профиля контакта

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)      |   Contacts.ReadWrite           |
|Делегированные (личная учетная запись Майкрософт)      |   Не поддерживается.            |
|Для приложений      |    Contacts.ReadWrite           |

> [!NOTE]
> 1. Чтобы обновить фотографию любого пользователя в организации, ваше приложение должно иметь разрешение *User.ReadWrite.All* и вызывать этот API под собственным удостоверением, а не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service). Для обновления фотографии вошедвшего пользователя требуется только *разрешение User.ReadWrite* .
> 2. В настоящее время существует [известная проблема](/graph/known-issues#groups) c доступом к групповым фотографиям с помощью разрешений приложений.
> 3. Обновление фотографии пользователя с помощью microsoft API Graph в настоящее время не поддерживается в Azure AD B2C.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | image/jpeg. Обязательный.  |

## <a name="request-body"></a>Тело запроса
Включите в текст запроса двоичные данные фотографии.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK`.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
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

### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

