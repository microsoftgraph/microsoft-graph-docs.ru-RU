---
title: 'разрешение: Ревокегрантс'
description: Обновление разрешений на общий доступ к элементу
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a6ac5f1aacc068ef092f3881d67f6c121d84b400
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582371"
---
# <a name="permission-revokegrants"></a>разрешение: Ревокегрантс
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отмените доступ к элементу [ListItem][] или [driveItem][] , предоставленному через ссылку для общего доступа, удалив указанного [получателя][] из ссылки.

>**Примечание:** Эта функция доступна только для ссылок для общего доступа, ограниченных пользователями.

[listItem]: ../resources/listitem.md
[driveItem]: ../resources/driveitem.md
[recipient]: ../resources/driverecipient.md

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Files.ReadWrite.All, Sites.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/lists/{list-id}/items/{listItem-id}/permissions/{perm-id}/revokeGrants
POST /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|получателей|Коллекция [driveRecipient](../resources/driverecipient.md)|Коллекция получателей, которые будут отзывать доступ к ссылке для общего доступа.|

## <a name="response"></a>Отклик

При успешном выполнении это действие возвращает `200 OK` код отклика и [разрешение](../resources/permission.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "permission-revokegrants"
}
-->
``` http
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants

Content-Type: application/json
Content-length: 95

{
  "grantees": [
    {
      "email": "ryan@contoso.com"
    }
  ]
}
```


### <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает ресурс [Permission](../resources/permission.md) в тексте отклика, представляющий обновленное состояние ссылки для общего доступа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "users",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
