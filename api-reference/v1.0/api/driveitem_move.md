---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Перемещение файла или папки"
ms.openlocfilehash: ebffe8451c6cf5ce7f025b70225054cfb8080cf6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="move-a-driveitem-to-a-new-folder"></a>Перемещение ресурса DriveItem в новую папку

Чтобы переместить ресурс DriveItem в новый родительский элемент, вашему приложению требуется изменить элемент **parentReference** ресурса DriveItem, который необходимо переместить.

Это особый случай метода [Update](driveitem_update.md).
Ваше приложение может совмещать процедуры перемещения элемента в новый контейнер и изменения других свойств элемента в одном запросе.

С помощью этого запроса не удастся переместить элементы между объектами [Drive](../resources/drive.md).

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
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте новое значение для поля свойства **parentReference**. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в другие значения свойств. Чтобы производительность была максимальной, не следует включать существующие значения, которые не изменились.

**Примечание.** При перемещении элементов в корневую папку диска вашему приложению не удастся использовать синтаксис `"id:" "root"`.
Приложению потребуется предоставить фактический идентификатор корневой папки для ссылки на родительский элемент.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.

## <a name="example"></a>Пример

В этом примере показано, как переместить элемент, указанный с помощью идентификатора {item-id}, в папку с идентификатором `new-parent-folder-id` на диске пользователя.

<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "new-parent-folder-id"
  },
  "name": "new-item-name.txt"
}
```

### <a name="response"></a>Ответ

В примере ниже показан ответ для этого запроса на перемещение.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "new-item-name.txt",
  "parentReference":
  {
    "driveId": "11231001",
    "path": "/drive/root:/Documents",
    "id": "1231203102!1011"
  }
}
```

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move"
} -->
