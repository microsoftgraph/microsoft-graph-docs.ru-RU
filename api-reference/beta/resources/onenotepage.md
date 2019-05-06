---
title: Тип ресурса Оненотепаже
description: Страница в записной книжке OneNote.
localization_priority: Normal
ms.openlocfilehash: 04e06fefd0b48a5d794f20733a4755e030cb7e0d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630799"
---
# <a name="onenotepage-resource-type"></a>Тип ресурса Оненотепаже

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Страница в записной книжке OneNote.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|содержимое|Поток|HTML-контент страницы.|
|contentUrl|String|URL-адрес HTML-содержимого страницы.  Только для чтения.|
|Креатедбяппид|String|Уникальный идентификатор приложения, создавшего страницу. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|String|Уникальный идентификатор страницы.  Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|степень|Int32|Уровень отступа страницы. Только для чтения.|
|links|[Пажелинкс](pagelinks.md)|Ссылки для открытия страницы. `oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена. `oneNoteWebUrl` Ссылка открывает страницу в OneNote Online. Только для чтения.|
|порядке|Int32|Порядок страницы в родительском разделе. Только для чтения.|
|Self|String|Конечная точка, в которой можно получить сведения о странице. Только для чтения.|
|title|String|Заголовок страницы. |

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[записной книжки](notebook.md)|Записная книжка, содержащая страницу.  Только для чтения.|
|parentSection|[Оненотесектион](onenotesection.md)|Раздел, содержащий страницу. Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод страницы](../api/page-get.md) | [Оненотепаже](onenotepage.md) |Чтение свойств и связей страницы.|
|[Обновление содержимого страницы](../api/page-update.md) | Нет |Обновление HTML-содержимого страницы. |
|[Удаление страницы](../api/page-delete.md) | Нет |Удаление страницы. |
|[copyToSection](../api/page-copytosection.md)| Нет |Копирует страницу в определенный раздел.|

## <a name="json-representation"></a>Представление в формате JSON

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
