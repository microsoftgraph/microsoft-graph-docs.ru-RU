---
title: Тип ресурса onenoteSection
description: Раздел в OneNote записной книжке. Разделы могут содержать страницы.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: fecac214a7d6a56b5f7f8cef4f9b798f3b790aa9
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176704"
---
# <a name="onenotesection-resource-type"></a>Тип ресурса onenoteSection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Раздел в OneNote записной книжке. Разделы могут содержать страницы.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|Строка|Уникальный идентификатор раздела.  Только для чтения.|
|isDefault|Boolean|Указывает, является ли это разделом пользователя по умолчанию. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|links|[sectionLinks](sectionlinks.md)|Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в OneNote клиенте, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote в Интернете.|
|displayName|Строка|Имя раздела. |
|pagesUrl|Строка|`pages` Конечная точка, в которой можно получить сведения для всех страниц в разделе. Только для чтения.|
|Самостоятельно|Строка|Конечная точка, где можно получить сведения о разделе. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|pages|[Коллекция onenotePage](onenotepage.md)|Коллекция страниц в разделе.  Только для чтения. Допускается значение null.|
|parentNotebook|[notebook](notebook.md)|Записная книжка, содержащая раздел.  Только для чтения.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|Группа разделов, содержащая раздел.  Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение раздела](../api/section-get.md) | [onenoteSection](onenotesection.md) |Чтение свойств и связей раздела.|
|[Создание страницы](../api/section-post-pages.md) |[onenotePage](onenotepage.md)| Создайте страницу, выполнив публикацию в коллекции страниц в указанном разделе.|
|[Перечисление страниц](../api/section-list-pages.md) |[Коллекция onenotePage](onenotepage.md)| Получение коллекции страниц в указанном разделе.|
|[copyToNotebook](../api/section-copytonotebook.md)|Нет|Скопируйте раздел в определенную записную книжку.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Нет|Скопируйте раздел в определенную группу разделов.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


