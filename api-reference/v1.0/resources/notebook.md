---
title: тип ресурса записной книжки
description: Блокнот OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ac3a433e3fa0e13beefb83a4525cb5975c9dfbe56d1c668c7bd8931982e84425
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189452"
---
# <a name="notebook-resource-type"></a>тип ресурса записной книжки

Пространство имен: microsoft.graph

Блокнот OneNote.

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
|createdDateTime|DateTimeOffset|Дата и время создания записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String|Уникальный идентификатор записной книжки. Только для чтения.|
|isDefault|Boolean|Указывает, является ли это ноутбук пользователя по умолчанию. Только для чтения.|
|IsShared|Boolean|Указывает, является ли записная книжка общей. Если да, ее содержимое, кроме владельца, могут видеть другие люди. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|links|[NotebookLinks](notebooklinks.md)|Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в OneNote, если она установлена. Ссылка `oneNoteWebURL` открывает записную книжку в OneNote в Интернете.|
|displayName|String|Имя записной книжки.|
|sectionGroupsUrl|String|URL-адрес `sectionGroups` свойства навигации, который возвращает все группы разделов в записной книжке. Только для чтения.|
|sectionsUrl|String|URL-адрес `sections` свойства навигации, который возвращает все разделы в записной книжке. Только для чтения.|
|self|String|Конечная точка, где можно получить сведения о записной книжке. Только для чтения.|
|userRole|onenoteUserRole|Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Владелец представляет доступ к записной книжке на уровне владельца. Автор представляет доступ к записной книжке для чтения и записи. Reader представляет доступ только для чтения к записной книжке. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|sectionGroups|Коллекция [SectionGroup](sectiongroup.md)|Группы разделов в записной книжке. Только для чтения. Допускает значение null.|
|sections|Коллекция [OnenoteSection](section.md)|Разделы в записной книжке. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод записной книжки](../api/notebook-get.md) | [Notebook](notebook.md) |Ознакомьтесь с свойствами и отношениями записной книжки.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [recentNotebook](recentnotebook.md) collection | Получите коллекцию записных книжек, которые недавно открывал пользователь. |
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md) | [Notebook](notebook.md) | Извлечение свойств и связей объекта записной книжки с помощью url-адреса. |
|[Создание группы разделов](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создайте группу разделов, разместив в разделеGroups коллекцию в указанной записной книжке.|
|[Перечисление групп разделов](../api/notebook-list-sectiongroups.md) |Коллекция [SectionGroup](sectiongroup.md)| Получите коллекцию групп разделов в указанной записной книжке.|
|[Создание раздела](../api/notebook-post-sections.md) |[OnenoteSection](section.md)| Создайте раздел, разместив в коллекции разделов в указанной записной книжке.|
|[Перечисление разделов](../api/notebook-list-sections.md) |Коллекция [OnenoteSection](section.md)| Получите коллекцию разделов в указанной записной книжке.|
|[copyNotebook](../api/notebook-copynotebook.md)| Нет | Копирует записную книжку.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

