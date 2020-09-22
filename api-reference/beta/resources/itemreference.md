---
author: JeremyKelley
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a02a33bed5875e6e97f41e534274adb0355333fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039337"
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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
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

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

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
  "tocPath": "Resources/ItemReference"
} -->


