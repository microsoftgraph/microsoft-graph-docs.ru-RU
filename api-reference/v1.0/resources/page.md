---
title: Тип ресурса Page
description: Страница в записной книжке OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 69066585c575569da7b355a6c52263843510dcc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447243"
---
# <a name="page-resource-type"></a>Тип ресурса Page

Пространство имен: microsoft.graph

Страница в записной книжке OneNote.

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
|contentUrl|String|URL-адрес HTML-содержимого страницы.  Только для чтения.|
|createdByAppId|String|Уникальный идентификатор приложения, создавшего страницу. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|String|Уникальный идентификатор страницы.  Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|степень|Int32|Уровень отступа страницы. Только для чтения.|
|links|[пажелинкс](pagelinks.md)|Ссылки для открытия страницы. `oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена. `oneNoteWebUrl` Ссылка открывает страницу в OneNote в Интернете. Только для чтения.|
|порядке|Int32|Порядок страницы в родительском разделе. Только для чтения.|
|Self|String|Конечная точка, в которой можно получить сведения о странице. Только для чтения.|
|title|Строка|Заголовок страницы. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Записная книжка, содержащая страницу.  Только для чтения.|
|parentSection|[оненотесектион](section.md)|Раздел, содержащий страницу. Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод страницы](../api/page-get.md) | [Page](page.md) |Чтение свойств и связей страницы.|
|[Обновление содержимого страницы](../api/page-update.md) | Нет |Обновление HTML-содержимого страницы. |
|[Удаление страницы](../api/page-delete.md) | Нет |Удаление страницы. |
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
