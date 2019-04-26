---
title: Обновление объекта profilephoto
description: Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта. Так как
localization_priority: Normal
ms.openlocfilehash: 1cf4d99f55768a6fad868d91d526fc5fd0b7b5ca
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332066"
---
# <a name="update-profilephoto"></a>Обновление объекта profilephoto

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление фотографии для любого пользователя в клиенте, в том числе пользователя, выполнившего вход, или указанной группы или контакта. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемой фотографии не может превышать 4 МБ.

Используйте только PUT для этой операции в бета-версии.

> **Note (Примечание** ) Операция обновления фотографий в бета-версии поддерживает только рабочие и учебные почтовые ящики пользователей, а не личные почтовые ящики.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Фотография профиля вошедшего **пользователя**:<br/>User. ReadWrite, User. ReadWrite. ALL<br /><br />Для ресурса **group**:<br />Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Для ресурса **user**:<br/>User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.ReadWrite |

> **Note (Примечание** ) Чтобы обновить фотографию любого пользователя в Организации, ваше приложение должно иметь разрешение User. ReadWrite. ALL Application и вызывать этот API с собственным идентификатором, а не от имени пользователя. Чтобы узнать больше, ознакомьтесь [со статьей получение доступа без вошедшего пользователя](/graph/auth-v2-service).

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
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
