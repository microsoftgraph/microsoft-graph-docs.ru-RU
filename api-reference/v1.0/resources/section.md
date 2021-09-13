---
title: Тип ресурса раздела
description: Раздел в OneNote блокноте. Разделы могут содержать страницы.
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8cbabaaae4ee1452cbce2e5c01859a50d0679358
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123092"
---
# <a name="section-resource-type"></a>Тип ресурса раздела

Пространство имен: microsoft.graph

Раздел в OneNote блокноте. Разделы могут содержать страницы.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
|createdDateTime|DateTimeOffset|Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|Строка|Уникальный идентификатор раздела.  Только для чтения.|
|isDefault|Boolean|Указывает, является ли это разделом по умолчанию пользователя. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|links|[SectionLinks](sectionlinks.md)|Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в родной OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote в Интернете.|
|displayName|Строка|Имя раздела. |
|pagesUrl|Строка|Конечная точка, где можно получить сведения `pages` для всех страниц в разделе. Только для чтения.|
|self|Строка|Конечная точка, где можно получить сведения о разделе. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|pages|Коллекция [OnenotePage](page.md)|Коллекция страниц в разделе.  Только для чтения. Допускается значение null.|
|parentNotebook|[Notebook](notebook.md)|Блокнот, содержащий раздел.  Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа разделов, которая содержит раздел.  Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение раздела](../api/section-get.md) | [OnenoteSection](section.md) |Ознакомьтесь с свойствами и отношениями раздела.|
|[Создание страницы](../api/section-post-pages.md) |[Page](page.md)| Создайте страницу, выложив ее в коллекцию страниц в указанном разделе.|
|[Перечисление страниц](../api/section-list-pages.md) |Коллекция [Page](page.md)| Получите коллекцию страниц в указанном разделе.|
|[copyToNotebook](../api/section-copytonotebook.md)|Нет|Скопируйте раздел в определенный блокнот.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Нет|Скопируйте раздел в определенную группу разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

