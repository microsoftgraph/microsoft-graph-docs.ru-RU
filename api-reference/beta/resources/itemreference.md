---
author: JeremyKelley
description: Ресурс ItemReference предоставляет сведения, необходимые для обращения к ресурсу DriveItem через API.
ms.date: 09/10/2017
title: ItemReference
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sharepoint
ms.openlocfilehash: ca111ef38ca8e283294a879f4dfb582c50da80fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068516"
---
# <a name="itemreference-resource-type"></a>Тип ресурса ItemReference

Пространство имен: microsoft.graph

Ресурс **ItemReference предоставляет** сведения, необходимые для решения [проблемы driveItem через](driveitem.md) API.

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
| id            | Строка            | Уникальный идентификатор элемента на диске. Только для чтения.
| name          | String            | Имя элемента, на который направлена ссылка. Только для чтения.
| path          | String            | Путь, по которому можно перейти к элементу. Только для чтения.
| shareId       | String            | Уникальный идентификатор общего ресурса, доступ к которому можно получить с помощью API [Shares][].
| sharepointIds | [sharepointIds][] | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| siteId        | Строка            | Для OneDrive для бизнеса и SharePoint это свойство представляет ID сайта, который содержит родительную библиотеку документов ресурса driveItem. Это значение такое же, как и свойство id этого [ресурса][] сайта. Это [непрозрачной строки, которая состоит из трех идентификаторов](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true#id-property) сайта. <br>Для OneDrive это свойство не заполнено.

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
  "tocPath&quot;: &quot;Resources/ItemReference"
} -->


