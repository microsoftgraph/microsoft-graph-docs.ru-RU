---
title: Тип ресурса "раздел"
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: faecf31ad09f3ea3b5614480fc051ad1054d442b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562951"
---
# <a name="section-resource-type"></a>Тип ресурса "раздел"

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
|id|String|Уникальный идентификатор раздела.  Только для чтения.|
|isDefault|Boolean|Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[Сектионлинкс](sectionlinks.md)|Ссылки для открытия раздела. `oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен. `oneNoteWebURL` Ссылка открывает раздел в OneNote Online.|
|displayName|String|Имя раздела. |
|Ссылки pagesurl|String|Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе. Только для чтения.|
|Self|String|Конечная точка, где можно получить сведения о разделе. Только для чтения.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|pages|Коллекция [страниц](page.md)|Коллекция страниц в разделе.  Только для чтения. Допускается значение null.|
|parentNotebook|[Notebook](notebook.md)|Записная книжка, содержащая раздел.  Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа разделов, содержащая раздел.  Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение раздела](../api/section-get.md) | [Section](section.md) |Прочитайте свойства и связи раздела.|
|[Создание страницы](../api/section-post-pages.md) |[Page](page.md)| Создание страницы путем публикации в коллекции страниц в указанном разделе.|
|[Перечисление страниц](../api/section-list-pages.md) |Коллекция [страниц](page.md)| Получение коллекции страниц в указанном разделе.|
|[copyToNotebook](../api/section-copytonotebook.md)|Нет|Скопируйте раздел в указанную записную книжку.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Нет|Скопируйте раздел в определенную группу разделов.|

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
