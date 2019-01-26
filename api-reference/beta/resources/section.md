---
title: Тип ресурса section
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: ea33cfae128a7ea796f3f14bd165210cbfec121d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574140"
---
# <a name="section-resource-type"></a>Тип ресурса section

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Раздел в записной книжке OneNote. Разделы могут содержать страницы.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|Строка|Уникальный идентификатор раздела.  Только для чтения.|
|isDefault|Логический|Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[sectionLinks](sectionlinks.md)|Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote Online.|
|displayName|Строка|Имя раздела. |
|pagesUrl|Строка|`pages` — конечная точка, в которой можно получить сведения обо всех страницах в разделе. Только для чтения.|
|self|Строка|Конечная точка, в которой можно получить сведения о разделе. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|pages|[onenotePage](onenotepage.md) коллекции|Коллекция страниц в разделе.  Только для чтения. Допускает значение null.|
|parentNotebook|[записная книжка](notebook.md)|Записная книжка, содержащая раздел.  Только для чтения.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|Группа объектов, содержащая раздел.  Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение раздела](../api/section-get.md) | [onenoteSection](section.md) |Чтение свойств и отношений раздела.|
|[Создание страницы](../api/section-post-pages.md) |[onenotePage](onenotepage.md)| Создайте страницу, отправив запрос POST в коллекцию pages в указанном разделе.|
|[Перечисление страниц](../api/section-list-pages.md) |[onenotePage](onenotepage.md) коллекции| Получение коллекции страниц в указанном разделе.|
|[copyToNotebook](../api/section-copytonotebook.md)|Нет|Копирование раздела в указанную записную книжку.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Нет|Копирование раздела в указанную группу разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
