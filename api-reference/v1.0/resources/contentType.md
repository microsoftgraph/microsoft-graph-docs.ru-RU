---
author: daspek
description: Ресурс contentType представляет тип контента в SharePoint.
title: Тип ресурса contentType
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6c7c45b74088902f4f1565b52c96577cfcd6e3ca
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191347"
---
# <a name="contenttype-resource-type"></a>Тип ресурса contentType

Пространство имен: microsoft.graph


Представляет тип контента в SharePoint.
Типы контента позволяют определить набор столбцов, которые должны присутствовать на каждом [**элементе listItem**][listItem] в [**списке**][list].

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление contentTypes на сайте](../api/site-list-contenttypes.md)|[Коллекция contentType](../resources/contenttype.md)|Получение списка объектов [contentType](../resources/contenttype.md) и их свойств на [сайте](../resources/site.md).|
|[Перечисление contentTypes в списке](../api/list-list-contenttypes.md)|[Коллекция contentType](../resources/contenttype.md)|Получение списка объектов [contentType](../resources/contenttype.md) и их свойств в [списке](../resources/list.md).|
|[Создание contentType для сайта](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Создайте объект [contentType](../resources/contenttype.md) на [сайте](../resources/site.md).|
|[Получение contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|Чтение свойств и связей объекта [contentType](../resources/contenttype.md) .|
|[Обновление contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|Обновление свойств объекта [contentType](../resources/contenttype.md) .|
|[Удаление contentType](../api/contenttype-delete.md)|Нет|Удаляет объект [contentType](../resources/contenttype.md) .|
|[isPublished](../api/contenttype-ispublished.md)|Логическое| Проверяет, опубликован [ли contentType](../resources/contenttype.md) .|
|[publish](../api/contenttype-publish.md)|[contentType](../resources/contenttype.md)| Публикация [contentType](../resources/contenttype.md).|
|[unpublish](../api/contenttype-unpublish.md)|[contentType](../resources/contenttype.md)|Отмена публикации [contentType](../resources/contenttype.md).|
|[addCopy](../api/contenttype-addcopy.md)|[contentType](../resources/contenttype.md)|Добавьте копию [contentType](../resources/contenttype.md) с [сайта](../resources/site.md) в [список](../resources/list.md).|
|[associateWithHubSites](../api/contenttype-associatewithhubsites.md)|[contentType](../resources/contenttype.md)|Связывает [contentType](../resources/contenttype.md) со списком центральных сайтов.|
|[copyToDefaultContentLocation](../api/contenttype-copytodefaultcontentlocation.md)|[contentType](../resources/contenttype.md)| Скопируйте файл в расположение содержимого по умолчанию в [contentType](../resources/contenttype.md).|
|[Перечисление столбцов](../api/contenttype-list-columns.md)|[Коллекция columnDefinition](../resources/columnDefinition.md)|Получение коллекции столбцов, представленных в виде [ресурсов columnDefinition](../resources/columnDefinition.md) , в **contentType**.|
|[Создание столбца](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columnDefinition.md)|Добавление столбца к **типу контента** на сайте или в списке.|
|[GetCompatibleHubContentTypes](../api/contenttype-getcompatiblehubcontenttypes.md)|[Коллекция contentType](../resources/contenttype.md)|Получение списка совместимых типов контента из центра типов контента, которые можно добавить на целевой [сайт](../resources/site.md) или [в список](../resources/list.md).|
|[addCopyFromContentTypeHub](../api/contenttype-addcopyfromcontenttypehub.md)|[contentType](../resources/contenttype.md)|Добавьте или синхронизируйте копию опубликованного типа контента из концентратора типов контента на целевой [сайт](../resources/site.md) или [список](../resources/list.md).|


## <a name="properties"></a>Свойства

| Свойство     | Тип                 | Описание|
|:------------------|:---------------------|:----------------------------------|
| associatedHubsUrls         | Collection(string) | Список канонических URL-адресов для центральных сайтов, с которыми связан этот тип контента. Он будет содержать все центральные сайты, на которых этот тип контента поставлен в очередь для принудительного применения или уже применен. Принудительное применение типа контента означает, что тип контента будет применяться к спискам на сайтах с принудительной проверкой.|
| description       | строка               | Текст с описанием элемента.|
| documentSet         | [documentSet][]      | [Метаданные набора](/sharepoint/governance/document-set-planning#about-document-sets) документов.|
| documentTemplate    | [documentSetContent][] | Метаданные шаблона документа. Чтобы убедиться, что документы имеют согласованное содержимое на сайте и его дочерних сайтах, можно связать шаблон Word, Excel или PowerPoint с типом контента сайта.|
| group             | string               | Имя группы, которой принадлежит этот тип контента. Позволяет упорядочить связанные типы контента.|
| hidden            | Логический              | Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.|
| id                | string               | Уникальный идентификатор типа контента.|
| inheritedFrom   | [itemReference][]    | Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.|
| isBuiltIn            | Boolean| Указывает, является ли тип контента встроенным типом контента. |
| name              | string               | Имя типа контента.|
| Заказ             | [contentTypeOrder][] | Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.|
| Parentid          | string               | Уникальный идентификатор типа контента.|
| propagateChanges     | Логическое              | Если `true`изменения, внесенные в тип контента, будут отправлены в унаследованные типы контента и списки, реализующие тип контента.|
| readOnly          | Логическое              | Если `true`тип контента не может быть изменен, если это значение не задано в первую очередь `false`.|
| sealed            | Логическое              | Если `true`тип контента не может быть изменен пользователями или с помощью операций push-down. Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.|


## <a name="relationships"></a>Связи

| Связь    | Тип                      | Описание|
|:----------------|:--------------------------|:-------------------------------|
| base     | [contentType][]  | Родительский тип contentType, от которого наследуется этот тип контента. |
| columnLinks   | Коллекция [columnLink][] | Коллекция столбцов, необходимых для этого типа контента.|
| baseTypes     | Collection([contentType][])     | Коллекция типов контента, которые являются предками этого типа контента.|
| columnPositions         | Collection([columnDefinition][]) | Сведения о порядке столбцов в типе контента.|
| columns       | Collection([columnDefinition][])  | Коллекция определений столбцов для данного contentType.|

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

Ниже приведено представление ресурса **contentType в формате JSON** .

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


