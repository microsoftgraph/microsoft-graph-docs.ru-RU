---
title: Тип ресурса для записной книжки
description: Записная книжка OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 2259a8d84c3c784c5c6af5ffda08a863a818be1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086510"
---
# <a name="notebook-resource-type"></a>Тип ресурса для записной книжки

Пространство имен: microsoft.graph

Записная книжка OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|Строка|Уникальный идентификатор записной книжки. Только для чтения.|
|isDefault|Boolean|Указывает, является ли Записная книжка пользователя по умолчанию. Только для чтения.|
|IsShared|Boolean|Указывает, является ли записная книжка общей. Если да, ее содержимое, кроме владельца, могут видеть другие люди. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[нотебуклинкс](notebooklinks.md)|Ссылки для открытия записной книжки. `oneNoteClientURL`Ссылка открывает записную книжку в собственном клиенте OneNote, если она установлена. `oneNoteWebURL`Ссылка открывает записную книжку в OneNote в Интернете.|
|displayName|Строка|Имя записной книжки.|
|сектионграупсурл|Строка|URL-адрес для `sectionGroups` Свойства навигации, который возвращает все группы разделов в записной книжке. Только для чтения.|
|сектионсурл|Строка|URL-адрес для `sections` Свойства навигации, который возвращает все разделы записной книжки. Только для чтения.|
|Self|Строка|Конечная точка, где можно получить сведения о записной книжке. Только для чтения.|
|userRole|оненотеусерроле|Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Owner — это доступ к записной книжке на уровне владельца. Участник представляет доступ к записной книжке для чтения и записи. Читатель предоставляет доступ только для чтения к записной книжке. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|sectionGroups|Коллекция [SectionGroup](sectiongroup.md)|Группы разделов в записной книжке. Только для чтения. Допускает значение null.|
|sections|Коллекция [OnenoteSection](section.md)|Разделы записной книжки. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод записной книжки](../api/notebook-get.md) | [Notebook](notebook.md) |Прочитайте свойства и связи записной книжки.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | Коллекция [recentNotebook](recentnotebook.md) | Получите коллекцию записных книжек, которые недавно открывал пользователь. |
|[жетнотебукфромвебурл](../api/notebook-getnotebookfromweburl.md) | [Notebook](notebook.md) | Получение свойств и связей объекта записной книжки с помощью URL-пути. |
|[Создание группы разделов](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создание группы разделов путем отправки в коллекцию sectionGroups в указанной записной книжке.|
|[Перечисление групп разделов](../api/notebook-list-sectiongroups.md) |Коллекция [SectionGroup](sectiongroup.md)| Получение коллекции групп разделов в указанной записной книжке.|
|[Создание раздела](../api/notebook-post-sections.md) |[оненотесектион](section.md)| Создание раздела путем публикации в коллекции разделов в указанной записной книжке.|
|[Перечисление разделов](../api/notebook-list-sections.md) |Коллекция [OnenoteSection](section.md)| Получение коллекции разделов в указанной записной книжке.|
|[Включеныcopynotebook](../api/notebook-copynotebook.md)| Нет | Копирует записную книжку.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

