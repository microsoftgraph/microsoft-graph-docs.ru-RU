---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Обновление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3eb23e5657794a4ef4062cc8b36cc003055e38c2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260006"
---
# <a name="update-driveitem-properties"></a>Обновление свойств ресурса DriveItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.

Путем обновления также можно [переместить элемент](driveitem-move.md) в другой родительский объект, изменив свойство **parentReference** этого элемента.

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
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`. |

## <a name="request-body"></a>Текст запроса

Укажите в тексте запроса значения обновляемых свойств.

Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.
Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.

## <a name="example"></a>Пример

В этом примере показано, как переименовать ресурс DriveItem и присвоить ему имя new-file-name.docx.

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] в теле ответа.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
