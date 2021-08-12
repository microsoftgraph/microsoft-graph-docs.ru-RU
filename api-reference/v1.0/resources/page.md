---
title: Тип ресурса страницы
description: Страница в записной OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77cadf00585c18a5ab0c8d87a09861c7806676fcad55beac033bc0a5a6d3b255
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180574"
---
# <a name="page-resource-type"></a>Тип ресурса страницы

Пространство имен: microsoft.graph

Страница в записной OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|содержимое|Поток|HTML-контент страницы.|
|contentUrl|String|URL-адрес HTML-контента страницы.  Только для чтения.|
|createdByAppId|String|Уникальный идентификатор приложения, создавшего страницу. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String|Уникальный идентификатор страницы.  Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|уровень|Int32|Уровень отступа страницы. Только для чтения.|
|links|[PageLinks](pagelinks.md)|Ссылки для открытия страницы. Ссылка `oneNoteClientURL` открывает страницу в родном клиенте OneNote, если она установлена. Ссылка `oneNoteWebUrl` открывает страницу в OneNote в Интернете. Только для чтения.|
|порядок|Int32|Порядок страницы в родительском разделе. Только для чтения.|
|self|String|Конечная точка, в которой можно получить сведения о странице. Только для чтения.|
|title|String|Заголовок страницы. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Блокнот, содержащий страницу.  Только для чтения.|
|parentSection|[OnenoteSection](section.md)|Раздел, содержащий страницу. Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод страницы](../api/page-get.md) | [Page](page.md) |Ознакомьтесь с свойствами и отношениями страницы.|
|[Обновление содержимого страницы](../api/page-update.md) | Нет |Обновление HTML-контента страницы. |
|[Удаление страницы](../api/page-delete.md) | Нет |Удалите страницу. |
|[copyToSection](../api/page-copytosection.md)| Нет |Копирует страницу в определенный раздел.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

