---
title: Обновление объекта profilephoto
description: Обновление фотографии любого пользователя в клиенте, в том числе пользователя, выполнившего вход, либо указанной группы или контакта. Так как
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: e6ccd0fe70f2e48c890df074c6a7865cbf502f83
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787592"
---
# <a name="update-profilephoto"></a>Обновление объекта profilephoto

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновим фотографию для любого пользователя в клиенте, включая пользователя, включаемого в нее, или указанной группы или контакта. Так как в настоящее время существует ограничение в 8 МБ на общий размер каждого запроса REST, размер фотографии, которая можно добавить, ограничен до 8 МБ.

Только используйте PUT для этой операции.

> **Примечание.** При обновлении **фотографии** пользователя эта операция сначала пытается обновить фотографию в Microsoft 365. Если это не удается (из-за того, что у пользователя нет почтового ящика), этот API попытается обновить фотографию в Azure Active Directory.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Фотография профиля подписанного **пользователя:**<br/>User.ReadWrite, User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложения                            | Для ресурса **user**:<br/>User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.ReadWrite |

> **Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service). Обновление фотографии подписанного пользователя требует только разрешения User.ReadWrite.

> **Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы при помощи разрешений для приложений.

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

Обновление фотографии для группы:

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
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

### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
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


