---
author: daspek
description: Ресурс contentType представляет тип контента в SharePoint.
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: bcd888d01f47b98fa5a55a4b6da2fdfe2028e05b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962660"
---
# <a name="contenttype-resource-type"></a>тип ресурса contentType

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип контента в SharePoint.
Типы контента позволяют определить набор столбцов, которые должны присутствовать на каждом [**listItem**][listItem] в [**списке.**][list]

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список contentTypes на сайте](../api/site-list-contenttypes.md)|[коллекция contentType](../resources/contenttype.md)|Получите список объектов [contentType](../resources/contenttype.md) и их свойств на [сайте.](../resources/site.md)|
|[Список contentTypes в списке](../api/list-list-contenttypes.md)|[коллекция contentType](../resources/contenttype.md)|Получите список объектов [contentType](../resources/contenttype.md) и их свойств в [списке.](../resources/list.md)|
|[Создание contentType для сайта](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Создание нового [объекта contentType](../resources/contenttype.md) на [сайте.](../resources/site.md)|
|[Get contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|Ознакомьтесь с свойствами и отношениями объекта [contentType.](../resources/contenttype.md)|
|[Обновление contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|Обновление свойств объекта [contentType.](../resources/contenttype.md)|
|[Удаление contentType](../api/contenttype-delete.md)|Нет|Удаляет объект [contentType.](../resources/contenttype.md)|
|[isPublished](../api/contenttype-ispublished.md)|Boolean| Проверка [публикации contentType.](../resources/contenttype.md)|
|[publish](../api/contenttype-publish.md)|[contentType](../resources/contenttype.md)| Публикация [контентаType](../resources/contenttype.md).|
|[unpublish](../api/contenttype-unpublish.md)|[contentType](../resources/contenttype.md)|Unpublish a [contentType](../resources/contenttype.md).|
|[addCopy](../api/contenttype-addcopy.md)|[contentType](../resources/contenttype.md)|Добавьте копию [contentType](../resources/contenttype.md) с [сайта](../resources/site.md) в [список).](../resources/list.md)|
|[associateWithHubSites](../api/contenttype-associatewithhubsites.md)|[contentType](../resources/contenttype.md)|Связывает [contentType](../resources/contenttype.md) со списком концентраторов.|
|[copyToDefaultContentLocation](../api/contenttype-copytodefaultcontentlocation.md)|[contentType](../resources/contenttype.md)| Скопируйте файл в расположение контента по умолчанию в [contentType.](../resources/contenttype.md)|
|[Список столбцов](../api/contenttype-list-columns.md)|[коллекция columnDefinition](../resources/columnDefinition.md)|Получите коллекцию столбцов, представленных в [качестве ресурсов columnDefinition,](../resources/columnDefinition.md) в **contentType.**|
|[Создание столбца](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columnDefinition.md)|Добавление столбца к **типу контента** на сайте или в списке.|


## <a name="properties"></a>Свойства

| Имя свойства     | Тип                 | Описание
|:------------------|:---------------------|:----------------------------------
| **description**   | строка               | Текст с описанием элемента.
| **group**         | string               | Имя группы, которой принадлежит этот тип контента. Позволяет упорядочить связанные типы контента.
| **hidden**        | Boolean              | Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.
| **id**            | string               | Уникальный идентификатор типа контента.
| **inheritedFrom** | [itemReference][]    | Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.
| **name**          | string               | Имя типа контента.
| **order**         | [contentTypeOrder][] | Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.
| **parentId**      | string               | Уникальный идентификатор типа контента.
| **readOnly**      | Boolean              | Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.
| **sealed**        | Boolean              | Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз. Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.
| **isBuiltIn**            | Boolean| Указывает, является ли тип контента встроенным типом контента. 
| **documentSet**       | [documentSet][]      | [Метаданные набора](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) документов.
| **documentTemplate**  | [documentSetContent][] | Метаданные шаблона документов. Чтобы убедиться, что документы имеют согласованный контент на сайте и его подмышках, можно связать шаблон Word, Excel или PowerPoint с типом контента сайта.
| **associatedHubsUrls**       | Коллекция (строка) | Список канонических URL-адресов для сайтов-концентраторов, с которыми связан этот тип контента. Это будет содержать все концентраторы, где этот тип контента находится в очереди для принудительного или уже принудительного. Применение типа контента означает, что тип контента будет применяться к спискам на принудительном сайте.
| **propagateChanges**   | Boolean              | Если какие-либо изменения, внесенные в тип контента, будут нажаты на унаследованные типы контента и списки, которые `true` реализуют тип контента.



## <a name="relationships"></a>Связи

| Имя свойства   | Тип                      | Описание
|:----------------|:--------------------------|:-------------------------------
| **база**   | [contentType][]  | Родительский contentType, из которого получен этот тип контента. 
| **columnLinks** | Коллекция [columnLink][] | Коллекция столбцов, необходимых для этого типа контента
| **baseTypes**   | Коллекция ([contentType][])     | Коллекция типов контента, которые являются предками этого типа контента.
| **columnPositions**       | Коллекция ([columnDefinition][]) | Сведения о порядке столбца в типе контента.
| **columns**     | Коллекция ([columnDefinition][])  | Коллекция определений столбцов для этого contentType.

Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса **contentType.**

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
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "base": { "@type": "microsoft.graph.contentType" },
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "isBuiltIn" : false,
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "associatedHubsUrls" : ["string"],
  "propagateChanges" : false,
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }]
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


