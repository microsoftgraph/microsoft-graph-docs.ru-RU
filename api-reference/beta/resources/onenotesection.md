---
title: Тип ресурса Оненотесектион
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f23017506208c1c0ff4f5a190eafe12079626d23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522318"
---
# <a name="onenotesection-resource-type"></a>Тип ресурса Оненотесектион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Раздел в записной книжке OneNote. Разделы могут содержать страницы.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|String|Уникальный идентификатор раздела.  Только для чтения.|
|isDefault|Boolean|Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[сектионлинкс](sectionlinks.md)|Ссылки для открытия раздела. `oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен. `oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.|
|displayName|Строка|Имя раздела. |
|Ссылки pagesurl|String|Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе. Только для чтения.|
|Self|String|Конечная точка, где можно получить сведения о разделе. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|pages|Коллекция [оненотепаже](onenotepage.md)|Коллекция страниц в разделе.  Только для чтения. Допускается значение null.|
|parentNotebook|[notebook](notebook.md)|Записная книжка, содержащая раздел.  Только для чтения.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|Группа разделов, содержащая раздел.  Только для чтения.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение раздела](../api/section-get.md) | [оненотесектион](onenotesection.md) |Прочитайте свойства и связи раздела.|
|[Создание страницы](../api/section-post-pages.md) |[оненотепаже](onenotepage.md)| Создание страницы путем публикации в коллекции страниц в указанном разделе.|
|[Перечисление страниц](../api/section-list-pages.md) |Коллекция [оненотепаже](onenotepage.md)| Получение коллекции страниц в указанном разделе.|
|[copyToNotebook](../api/section-copytonotebook.md)|Нет|Скопируйте раздел в указанную записную книжку.|
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
