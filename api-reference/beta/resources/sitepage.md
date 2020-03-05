---
author: rahmit
description: Этот ресурс представляет страницу в списке SitePages.
ms.date: 03/15/2018
title: ситепаже
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 6b7ce7bc14ce95ec4573fb7660cb584703d4a54e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520536"
---
# <a name="sitepage-resource"></a>ресурс Ситепаже

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот ресурс представляет страницу в [списке][]SitePages.
Он содержит заголовок, макет и коллекцию [веб-частей][]s.

## <a name="tasks-on-a-page"></a>Задачи на странице

Для ресурсов **ситепаже** доступны следующие задачи.
Все приведенные ниже примеры относятся к [сайту][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.

| Стандартная задача                     | Метод HTTP
|:--------------------------------|:------------------------------
| [Перечисление страниц][]                  | ПОЛУЧЕНИЕ/Pages
| [Вывод страницы][]                    | ПОЛУЧЕНИЕ/Пажес/{Паже-ИД}
| [создание][];                      | POST/Pages
| [удаление][];                      | Удаление/Пажес/{Паже-ИД}
| [публикация][];                     | POST/Пажес/{Паже-ИД}/публиш

[Перечисление страниц]: ../api/sitepage-list.md
[Вывод страницы]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса **ситепаже** в формате JSON.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

Ресурс **ситепаже** имеет следующие свойства.

| Имя свойства    | Тип                         | Описание
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | Тип контента страницы.

## <a name="page-content"></a>Контент страницы

Ресурс **ситепаже** имеет следующие поля контента.

| Имя свойства      | Тип                       | Описание
|:-------------------|:---------------------------|:---------------------------
| title              | string                     | Заголовок страницы.
| pageLayout         | строка                     | Имя макета страницы.
| webParts           | [Частей][]                | Веб-части на странице.

## <a name="authoring-metadata"></a>Метаданные для разработки

Ресурс **ситепаже** содержит следующие метаданные, связанные с созданием и отправкой. Свойство Публишингстате будет отражать состояние создания страницы, например извлеченный или опубликованный.

| Имя свойства          | Тип                   | Описание
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][].   | Состояние публикации и версия MM.mm страницы.

Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.

| Имя свойства        | Тип              | Описание
|:---------------------|:------------------|:----------------------------------
| id                   | строка            | Уникальный идентификатор элемента. Только для чтения.
| name                 | string            | Имя или название элемента.
| createdBy            | [identitySet][]   | Удостоверение создателя данного элемента. Только для чтения.
| eTag                 | string            | ETag для элемента. Только для чтения.
| lastModifiedBy       | [identitySet][]   | Удостоверение пользователя, который последним изменил данный элемент. Только для чтения.
| lastModifiedDateTime | DateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.
| parentReference      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Только для чтения.
| webUrl               | строка (url-адрес)      | URL-адрес для отображения элемента в браузере. Только для чтения.

## <a name="relationships"></a>Связи

У ресурса **ситепаже** нет отношений с другими ресурсами.

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
[Частей]: webpart.md

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
  "suppressions": []
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
