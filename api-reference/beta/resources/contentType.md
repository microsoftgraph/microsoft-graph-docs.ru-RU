---
author: daspek
description: Ресурс contentType представляет тип контента в SharePoint.
ms.date: 09/12/2017
title: Контент
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a051a8bb31cd138d351321255e77b7fb1517fe3e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507452"
---
# <a name="contenttype-resource-type"></a>Тип ресурса contentType

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **contentType** представляет _тип контента_ в SharePoint.
Типы контента позволяют определить набор столбцов, которые должны присутствовать в каждом элементе [**ListItem**][listItem] в [**списке**][list].

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentType** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

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
| **hidden**        | логический              | Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.
| **id**            | строка               | Уникальный идентификатор типа контента.
| **inheritedFrom** | [itemReference][]    | Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.
| **name**          | string               | Имя типа контента.
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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": []
}
-->
