---
title: Тип ресурса notebook
description: Записная книжка OneNote.
ms.openlocfilehash: 1c92ea22cdd6f368fbc84ee5a70c62272609b58c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075911"
---
# <a name="notebook-resource-type"></a>Тип ресурса notebook

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Записная книжка OneNote.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
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
|id|String|Уникальный идентификатор записной книжки. Только для чтения.|
|isDefault|Логический|Указывает, является ли эта записная книжка записной книжкой пользователя по умолчанию. Только для чтения.|
|IsShared|Логический|Указывает, является ли записная книжка общей. Если вы укажете значение true, содержимое записной книжки сможет видеть не только владелец. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[NotebookLinks](notebooklinks.md)|Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.|
|displayName|String|Имя записной книжки.|
|sectionGroupsUrl|Строка|URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в записной книжке. Только для чтения.|
|sectionsUrl|Строка|URL-адрес для свойства навигации `sections`, который возвращает все разделы в записной книжке. Только для чтения.|
|self|String|Конечная точка, в которой можно получить сведения о записной книжке. Только для чтения.|
|userRole|Строка|Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Owner — доступ к записной книжке на уровне владельца. Contributor — доступ к записной книжке для чтения и записи. Reader — доступ к записной книжке только для чтения. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|sectionGroups|Коллекция объектов [SectionGroup](sectiongroup.md)|Группы разделов в записной книжке. Только для чтения. Допускает значение null.|
|sections|Коллекция объектов [Section](section.md)|Разделы в записной книжке. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение записной книжки](../api/notebook-get.md) | [Notebook](notebook.md) |Считывание свойств и связей записной книжки.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | Коллекция [recentNotebook](recentnotebook.md) | Получение коллекции недавно открывавшихся записных книжек для пользователя. |
|[Создание группы разделов](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной записной книжке.|
|[Перечисление групп разделов](../api/notebook-list-sectiongroups.md) |Коллекция объектов [SectionGroup](sectiongroup.md)| Получение коллекции групп разделов в указанной записной книжке.|
|[Создание раздела](../api/notebook-post-sections.md) |[Section](section.md)| Создайте раздел, отправив запрос POST в коллекцию sections в указанной записной книжке.|
|[Перечисление разделов](../api/notebook-list-sections.md) |Коллекция объектов [Section](section.md)| Получение коллекции разделов в указанной записной книжке.|
|[copyNotebook](../api/notebook-copynotebook.md)| Нет | Копирование записной книжки.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
