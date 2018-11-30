---
title: Обновление объекта profilephoto
description: Обновление фотографий для любого пользователя, в том числе выполнил вход для клиентов пользователя, или указанной группы или контакта. Начиная с него
ms.openlocfilehash: 801ccd58e57cb02c1805f927dc22c9fd593cbae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079534"
---
# <a name="update-profilephoto"></a>Обновление объекта profilephoto

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновление фотографий для любого пользователя, в том числе выполнил вход для клиентов пользователя, или указанной группы или контакта. Поскольку в настоящее время не более 4 МБ на общий размер каждого запроса REST, этот параметр ограничивает размер фотографию, которую можно добавить в разделе 4 МБ.

Используйте только PUT для этой операции в бета-версии.

> **Примечание** Операция обновления фотографий в бета-версии поддерживает только пользователя рабочих или почтовые ящики school и не личные почтовые ящики.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Фотографий профиля выполнившего вход **пользователя**:<br/>User.ReadWrite User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложения                            | Для ресурса **user**:<br/>User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.ReadWrite |

> **Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](/graph/auth-v2-service).

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
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | image/jpeg. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Включите в текст запроса двоичные данные фотографии.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK`.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
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
  "tocPath": ""
}-->
