---
author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dd24f0d1fc0a5f5db576f5eea89b8205ff55b2b7
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714258"
---
# <a name="itemreference-resource-type"></a>Тип ресурса ItemReference

Пространство имен: microsoft.graph

Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание
|:--------------|:------------------|:-----------------------------------------
| driveId       | String            | Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.
| driveType     | Строка            | Служит для идентификации типа для объекта drive. Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].
| id            | String            | Уникальный идентификатор элемента на диске. Только для чтения.
| name          | String            | Имя элемента, на который направлена ссылка. Только для чтения.
| path          | String            | Путь, по которому можно перейти к элементу. Только для чтения.
| shareId       | String            | Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].
| sharepointIds | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| siteId        | String            | Для OneDrive для бизнеса и SharePoint это свойство представляет собой ИД сайта, который содержит родительную библиотеку документов ресурса driveItem. Это значение такое же, как свойство id этого [ресурса][] сайта. Это [непрозрачной строки, которая состоит из трех идентификаторов](/graph/api/resources/site#id-property) сайта. <br>В OneDrive это свойство не заполняется.

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md
[site]: ../resources/site.md

## <a name="remarks"></a>Замечания

Чтобы обратиться к элементу **driveItem** из ресурса **itemReference**, составьте URL-адрес в следующем формате:

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.

Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->

