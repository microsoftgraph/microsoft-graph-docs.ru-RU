---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Копирование файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 17c45f33425f77e6f4304360b6d52a0170752f4c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946296"
---
# <a name="copy-a-driveitem"></a>Копирование ресурса DriveItem

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Асинхронно создает копию элемента [driveItem][item-resource] (включая все дочерние элементы) в новом родительском элементе или с новым именем.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.


| Имя            | Значение                                          | Описание                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | Необязательный. Отсылает к родительскому элементу, в котором будет создана копия.                                         |
| name            | строка                                         | Необязательный. Новое имя копии. Если оно не предоставлено, будет использовано такое же имя, как в оригинале.    |

**Примечание.** Элемент _parentReference_ должен включать параметры `driveId` и `id` для целевой папки.

## <a name="example"></a>Пример

В этом примере показано, как копировать файл с идентификатором `{item-id}` в папку с идентификатором `driveId` и значением `id`.
У новой копии файла будет имя `contoso plan (copy).txt`.

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```

## <a name="response"></a>Отклик

Возвращает сведения о том, как [отслеживать ход](/graph/long-running-actions-overview) копирования после принятия запроса.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

В значении заголовка `Location` имеется URL-адрес службы, которая возвращает сведения о текущем состоянии операции копирования.
Вы можете использовать эти сведения, чтобы [определить, когда копирование будет завершено](/graph/long-running-actions-overview).

### <a name="remarks"></a>Примечания

Во многих случаях копирование выполняется асинхронно. Отклик API указывает, что операция копирования принята или отклонена, например из-за использования имени конечного файла.

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
