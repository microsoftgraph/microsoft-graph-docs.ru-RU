---
title: Тип ресурса onenotePage
description: Страница в OneNote записной книжке.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: 4f4b556b048d535236d40259bc9736de4e3e5ee4
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176728"
---
# <a name="onenotepage-resource-type"></a>Тип ресурса onenotePage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Страница в OneNote записной книжке.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|содержимое|Поток|HTML-содержимое страницы.|
|contentUrl|Строка|URL-адрес HTML-содержимого страницы.  Только для чтения.|
|createdByAppId|String|Уникальный идентификатор приложения, создавшего страницу. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String|Уникальный идентификатор страницы.  Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|Уровень|Int32|Уровень отступа страницы. Только для чтения.|
|links|[pageLinks](pagelinks.md)|Ссылки для открытия страницы. Ссылка `oneNoteClientURL` открывает страницу в собственном OneNote, если она установлена. Ссылка `oneNoteWebUrl` откроет страницу в OneNote в Интернете. Только для чтения.|
|Заказ|Int32|Порядок страницы в родительском разделе. Только для чтения.|
|Самостоятельно|String|Конечная точка, в которой можно получить сведения о странице. Только для чтения.|
|title|Строка|Заголовок страницы. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[notebook](notebook.md)|Записная книжка, содержащая страницу.  Только для чтения.|
|parentSection|[onenoteSection](onenotesection.md)|Раздел, содержащий страницу. Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод страницы](../api/page-get.md) | [onenotePage](onenotepage.md) |Чтение свойств и связей страницы.|
|[Обновление содержимого страницы](../api/page-update.md) | Нет |Обновите HTML-содержимое страницы. |
|[Удаление страницы](../api/page-delete.md) | Нет |Удалите страницу. |
|[copyToSection](../api/page-copytosection.md)| Нет |Копирует страницу в определенный раздел.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


