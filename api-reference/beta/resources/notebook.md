---
title: тип ресурса записной книжки
description: Блокнот OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 35c6ab2136f8a04be7edbc6170b4e7e0328b314c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722107"
---
# <a name="notebook-resource-type"></a>тип ресурса записной книжки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Блокнот OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
|links|[notebookLinks](notebooklinks.md)|Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в родном клиенте OneNote, если она установлена. Ссылка `oneNoteWebURL` открывает записную книжку в OneNote в Интернете.|
|displayName|String|Имя записной книжки.|
|sectionGroupsUrl|String|URL-адрес `sectionGroups` свойства навигации, который возвращает все группы разделов в записной книжке. Только для чтения.|
|sectionsUrl|String|URL-адрес `sections` свойства навигации, который возвращает все разделы в записной книжке. Только для чтения.|
|self|String|Конечная точка, где можно получить сведения о записной книжке. Только для чтения.|
|userRole|String|Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Владелец представляет доступ к записной книжке на уровне владельца. Автор представляет доступ к записной книжке для чтения и записи. Reader представляет доступ только для чтения к записной книжке. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|sectionGroups|[коллекция sectionGroup](sectiongroup.md)|Группы разделов в записной книжке. Только для чтения. Допускает значение null.|
|sections|[коллекция onenoteSection](onenotesection.md)|Разделы в записной книжке. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод записной книжки](../api/notebook-get.md) | [notebook](notebook.md) |Ознакомьтесь с свойствами и отношениями записной книжки.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [recentNotebook](recentnotebook.md) collection | Получите коллекцию записных книжек, которые недавно открывал пользователь. |
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md) | [notebook](notebook.md) | Извлечение свойств и связей объекта записной книжки с помощью url-адреса. |
|[Создание группы разделов](../api/notebook-post-sectiongroups.md) |[sectionGroup](sectiongroup.md)| Создайте группу разделов, разместив в разделеGroups коллекцию в указанной записной книжке.|
|[Перечисление групп разделов](../api/notebook-list-sectiongroups.md) |[коллекция sectionGroup](sectiongroup.md)| Получите коллекцию групп разделов в указанной записной книжке.|
|[Создание раздела](../api/notebook-post-sections.md) |[onenoteSection](onenotesection.md)| Создайте раздел, разместив в коллекции разделов в указанной записной книжке.|
|[Перечисление разделов](../api/notebook-list-sections.md) |[коллекция onenoteSection](onenotesection.md)| Получите коллекцию разделов в указанной записной книжке.|
|[copyNotebook](../api/notebook-copynotebook.md)| Нет | Копирует записную книжку.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


