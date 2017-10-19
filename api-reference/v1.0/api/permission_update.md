---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Изменение разрешений на общий доступ"
ms.openlocfilehash: ead6babf88b7efc578ef8be6d11cc9fb59dd5fdd
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="update-sharing-permission"></a>Изменение разрешений на общий доступ

В этой статье рассказывается, как изменить свойства разрешения на общий доступ путем обновления ресурса разрешения.

Таким способом можно изменить только свойство **roles**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | string | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.

Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.
Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   | Описание                   |
|:-------------|:-------|:------------------------------|
| **roles**    | String | Массив типов разрешений. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.

## <a name="example"></a>Пример

В примере ниже показан запрос, изменяющий роль в разрешении на общий доступ на роль "только чтение".

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md), представляющий обновленное состояние разрешения, в теле ответа.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
