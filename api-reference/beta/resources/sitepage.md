---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
ms.openlocfilehash: 65cfe61dadd1708abffe2d01abbbb15f40d158ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080470"
---
# <a name="sitepage-resource"></a>sitePage ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Этот ресурс представляет страницу SitePages [списка][].
Он содержит заголовок, макет и коллекцию s [веб-части][].

## <a name="tasks-on-a-page"></a>Задачи на странице

Для **sitePage** ресурсов доступны следующие задачи.
Всех приведенных ниже примерах относительны [сайта][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.

| Стандартная задача                     | Метод HTTP
|:--------------------------------|:------------------------------
| [Перечисление страниц][]                  | Получение /pages
| [Получение страницы][]                    | Получение /pages/ {идентификатор страницы}
| [Create][]                      | POST /pages
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

## <a name="page-content"></a>Контент страницы

Ресурс **sitePage** имеет следующие поля содержимого.

| Имя свойства      | Тип                       | Описание
|:-------------------|:---------------------------|:---------------------------
| должности.              | строка                     | Заголовок страницы.
| pageLayout         | string                     | Имя страницы макета страницы.
| веб-части           | [веб-части][]                | Веб-частей на странице.

## <a name="authoring-metadata"></a>Создание метаданных

Ресурс **sitePage** имеет следующие метаданные, связанные с разработки. Свойство publishingState будет отражают состояние как извлечь или опубликовать разработки страниц.

| Имя свойства          | Тип                   | Description
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][].   | Состояния публикации и MM.mm версия страницы.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание
|:---------------------|:------------------|:----------------------------------
| id                   | строка            | Уникальный идентификатор элемента. Только для чтения.
| name                 | строка            | Имя или название элемента.
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
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md.
[site]: site.md
[веб-части]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
