---
title: Тип ресурса section
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
ms.openlocfilehash: e0e2d650993ff3c8bcda688be305cf296a2dfdb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028225"
---
# <a name="section-resource-type"></a>Тип ресурса section

Раздел в записной книжке OneNote. Разделы могут содержать страницы.

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
|createdDateTime|DateTimeOffset|Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|String|Уникальный идентификатор раздела.  Только для чтения.|
|isDefault|Логический|Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[SectionLinks](sectionlinks.md)|Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote Online.|
|displayName|Строка|Имя раздела. |
|pagesUrl|Строка|`pages` — конечная точка, в которой можно получить сведения обо всех страницах в разделе. Только для чтения.|
|self|String|Конечная точка, в которой можно получить сведения о разделе. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|pages|[OnenotePage](page.md) коллекции|Коллекция страниц в разделе.  Только для чтения. Допускает значение null.|
|parentNotebook|[Notebook](notebook.md)|Записная книжка, содержащая раздел.  Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа объектов, содержащая раздел.  Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение раздела](../api/section-get.md) | [OnenoteSection](section.md) |Чтение свойств и отношений раздела.|
|[Создание страницы](../api/section-post-pages.md) |[Page](page.md)| Создайте страницу, отправив запрос POST в коллекцию pages в указанном разделе.|
|[Перечисление страниц](../api/section-list-pages.md) |Коллекция объектов [Page](page.md)| Получение коллекции страниц в указанном разделе.|
|[copyToNotebook](../api/section-copytonotebook.md)|Нет|Копирование раздела в указанную записную книжку.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Нет|Копирование раздела в указанную группу разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
