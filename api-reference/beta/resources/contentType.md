---
author: daspek
description: Ресурс contentType представляет тип контента в SharePoint.
title: contentType
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: f4585cad71f4d893c7034f3a346771d96cfd3e8d
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720872"
---
# <a name="contenttype-resource-type"></a>тип ресурса contentType

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип контента в SharePoint.
Типы контента позволяют определить набор столбцов, которые должны присутствовать на каждом [**listItem**][listItem] в [**списке**][list].

## <a name="properties"></a>Свойства

| Свойство          | Тип                 | Описание|
|:------------------|:---------------------|:----------------------------------|
|   associatedHubsUrls         | Коллекция (строка) | Список канонических URL-адресов для сайтов-концентраторов, с которыми связан этот тип контента. Это будет содержать все концентраторы, где этот тип контента находится в очереди для принудительного или уже принудительного. Применение типа контента означает, что тип контента будет применяться к спискам на принудительном сайте.|
|   documentSet         | [documentSet][]      | [Метаданные набора](/sharepoint/governance/document-set-planning#about-document-sets) документов.|
|   documentTemplate    | [documentSetContent][] | Метаданные шаблона документов. Чтобы убедиться, что документы имеют согласованное содержимое на сайте и его подмышках, можно связать шаблон Word, Excel или PowerPoint с типом контента сайта.|
|   description     | строка               | Текст с описанием элемента.|
|   group;           | string               | Имя группы, которой принадлежит этот тип контента. Позволяет упорядочить связанные типы контента.|
|   hidden          | Boolean              | Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.|
|   id              | строка               | Уникальный идентификатор типа контента.|
|   inheritedFrom   | [itemReference][]    | Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.|
|   isBuiltIn              | Boolean| Указывает, является ли тип контента встроенным типом контента. |
|   name            | string               | Имя типа контента.|
|   порядок           | [contentTypeOrder][] | Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.|
|   parentId        | string               | Уникальный идентификатор типа контента.|
|   propagateChanges     | Boolean              | Если `true`какие-либо изменения, внесенные в тип контента, будут нажаты на унаследованные типы контента и списки, которые реализуют тип контента.|
|   readOnly        | Boolean              | Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.|
|   sealed          | Boolean              | Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз. Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.|

| Свойство               | Тип                   | Описание                                                                                                                                                                                                                                                                                          |
| :--------------------- | :--------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **description**        | строка                 | Текст с описанием элемента.                                                                                                                                                                                                                                                                   |
| **group**              | string                 | Имя группы, которой принадлежит этот тип контента. Позволяет упорядочить связанные типы контента.                                                                                                                                                                                                            |
| **hidden**             | Boolean                | Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.                                                                                                                                                                                                                               |
| **id**                 | строка                 | Уникальный идентификатор типа контента.                                                                                                                                                                                                                                                           |
| **inheritedFrom**      | [itemReference][]      | Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.                                                                                                                                                              |
| **name**               | строка                 | Имя типа контента.                                                                                                                                                                                                                                                                        |
| **order**              | [contentTypeOrder][]   | Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.                                                                                                                                                                                                                           |
| **parentId**           | string                 | Уникальный идентификатор типа контента.                                                                                                                                                                                                                                                           |
| **readOnly**           | Boolean                | Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.                                                                                                                                                                                                            |
| **sealed**             | Boolean                | Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз. Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.                                                                                                                                       |
| **isBuiltIn**          | Boolean                | Указывает, является ли тип контента встроенным типом контента.                                                                                                                                                                                                                                              |
| **documentSet**        | [documentSet][]        | [Метаданные набора](/sharepoint/governance/document-set-planning#about-document-sets) документов.                                                                                                                                                                                                           |
| **documentTemplate**   | [documentSetContent][] | Метаданные шаблона документов. Чтобы убедиться, что документы имеют согласованное содержимое на сайте и его подмышках, можно связать шаблон Word, Excel или PowerPoint с типом контента сайта.                                                                                                    |
| **associatedHubsUrls** | Коллекция (строка)     | Список канонических URL-адресов для сайтов-концентраторов, с которыми связан этот тип контента. Это будет содержать все концентраторы, где этот тип контента находится в очереди для принудительного или уже принудительного. Применение типа контента означает, что тип контента будет применяться к спискам на принудительном сайте. |
| **propagateChanges**   | Boolean                | Если `true`какие-либо изменения, внесенные в тип контента, будут нажаты на унаследованные типы контента и списки, которые реализуют тип контента.                                                                                                                                                                 |

## <a name="relationships"></a>Связи

| Связь    | Тип                      | Описание|
|:----------------|:--------------------------|:-------------------------------|
|   base     | [contentType][]  | Родительский contentType, из которого получен этот тип контента. |
|   columnLinks   | Коллекция [columnLink][] | Коллекция столбцов, необходимых для этого типа контента|
|   baseTypes     | Collection([contentType][])     | Коллекция типов контента, которые являются предками этого типа контента.|
|   columnPositions         | Collection([columnDefinition][]) | Сведения о порядке столбца в типе контента.|
|   columns       | Collection([columnDefinition][])  | Коллекция определений столбцов для этого contentType.|

Дополнительные сведения см. в [публикации "Введение в типы контента и тип контента"][contentTypeIntro].

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "associatedHubsUrls" : ["string"],
  "base": { "@type": "microsoft.graph.contentType" },
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "description": "string",
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "isBuiltIn" : false,
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "propagateChanges" : false,
  "readOnly": false,
  "sealed": false
}
```

[list]: list.md
[listItem]: listitem.md

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
