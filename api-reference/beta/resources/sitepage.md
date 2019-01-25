---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522303"
---
# <a name="sitepage-resource"></a>sitePage ресурсов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот ресурс представляет страницу SitePages [списка][].
Он содержит заголовок, макет и коллекцию s [веб-части][].

## <a name="tasks-on-a-page"></a>Задачи на странице

Для **sitePage** ресурсов доступны следующие задачи.
Все приведенные ниже примеры относятся к сайту, например [][].

| Стандартная задача                     | Метод HTTP
|:--------------------------------|:------------------------------
| [Перечисление страниц][]                  | Запрос GET для страниц
| [Получение страницы][]                    | Получение /pages/ {идентификатор страницы}
| [Create][]                      | POST pages
| [Delete][]                      | Удаление /pages/ {идентификатор страницы}
| [Publish][]                     | Учет /pages/ {идентификатор страницы} аудио- и публикация

[Перечисление страниц]: ../api/sitepage-list.md
[Получение страницы]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>Представление JSON

Ниже представлена JSON **sitePage** ресурса.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

Ресурс **sitePage** имеет следующие свойства.

| Имя свойства    | Тип                         | Описание
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | Тип страницы содержимого.

## <a name="page-content"></a>Содержимое страницы

Ресурс **sitePage** имеет следующие поля содержимого.

| Имя свойства      | Тип                       | Описание
|:-------------------|:---------------------------|:---------------------------
| должности.              | строка                     | Заголовок страницы.
| pageLayout         | string                     | Имя страницы макета страницы.
| веб-части           | веб-часть                | Веб-частей на странице.

## <a name="authoring-metadata"></a>Создание метаданных

Ресурс **sitePage** имеет следующие метаданные, связанные с разработки. Свойство publishingState будет отражают состояние как извлечь или опубликовать разработки страниц.

| Имя свойства          | Тип                   | Описание
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][].   | Состояния публикации и MM.mm версия страницы.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание
|:---------------------|:------------------|:----------------------------------
| id                   | string            | Уникальный идентификатор элемента. Только для чтения.
| name                 | string            | Имя или название элемента.
| createdBy            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.
| eTag                 | string            | ETag для элемента. Только для чтения.
| lastModifiedBy       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| lastModifiedDateTime | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.
| parentReference      | [itemReference][] | Дата и время последнего изменения элемента. Только для чтения.
| webUrl               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

Ресурс **sitePage** не имеет отношения к другим ресурсам.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[списки]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md.
[site]: site.md
веб-часть

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
