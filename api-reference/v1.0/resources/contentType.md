---
author: daspek
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: Ресурс contentType представляет тип контента в SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1b307fb0b11b0608c15c46b618775dcef431815c4302a092e7e89f9cb7cb5942
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229292"
---
# <a name="contenttype-resource-type"></a>Тип ресурса contentType

Пространство имен: microsoft.graph

Ресурс **contentType** представляет _тип контента_ в SharePoint.
Типы контента позволяют определить набор столбцов, которые должны присутствовать на каждом [**listItem**][listItem] в [**списке.**][list]

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentType** в формате JSON.
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a>Свойства

| Имя свойства     | Тип                 | Описание
|:------------------|:---------------------|:----------------------------------
| **description**   | строка               | Текст с описанием элемента.
| **group**         | string               | Имя группы, которой принадлежит этот тип контента. Позволяет упорядочить связанные типы контента.
| **hidden**        | boolean              | Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.
| **id**            | строка               | Уникальный идентификатор типа контента.
| **inheritedFrom** | [itemReference][]    | Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.
| **name**          | строка               | Имя типа контента.
| **order**         | [contentTypeOrder][] | Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.
| **parentId**      | string               | Уникальный идентификатор типа контента.
| **readOnly**      | boolean              | Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.
| **sealed**        | boolean              | Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз. Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.

## <a name="relationships"></a>Связи

| Имя свойства   | Тип                      | Описание
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | Коллекция [columnLink][] | Коллекция столбцов, необходимых для этого типа контента

Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/ContentType"
} -->

