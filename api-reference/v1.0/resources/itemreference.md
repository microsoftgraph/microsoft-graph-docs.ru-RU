---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
ms.openlocfilehash: e83b0a18725d587094a00e9cc84a51b030d83340
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268468"
---
# <a name="itemreference-resource-type"></a>Тип ресурса ItemReference

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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание
|:--------------|:------------------|:-----------------------------------------
| driveId       | String            | Уникальный идентификатор экземпляра диска, содержащего элемент. Только для чтения.
| driveType     | String            | Служит для идентификации типа для объекта drive. Сведения о возможных значениях см. в статье, посвященной ресурсу [drive][].
| id            | String            | Уникальный идентификатор элемента на диске. Только для чтения.
| name          | String            | Имя элемента, на который направлена ссылка. Только для чтения.
| path          | String            | Путь, по которому можно перейти к элементу. Только для чтения.
| shareId       | String            | Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].
| sharepointIds | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares_get.md

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
