---
author: rahmit
description: Этот ресурс представляет страницу в списке SitePages.
ms.date: 03/15/2018
title: Ситепаже
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240ab50f31d500fad960768bb6c45cb9c6ff6511
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965049"
---
# <a name="sitepage-resource"></a><span data-ttu-id="bc523-103">ресурс Ситепаже</span><span class="sxs-lookup"><span data-stu-id="bc523-103">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc523-104">Этот ресурс представляет страницу в [списке][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="bc523-104">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="bc523-105">Он содержит заголовок, макет и коллекцию [веб-частей][]s.</span><span class="sxs-lookup"><span data-stu-id="bc523-105">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="bc523-106">Задачи на странице</span><span class="sxs-lookup"><span data-stu-id="bc523-106">Tasks on a page</span></span>

<span data-ttu-id="bc523-107">Для ресурсов **ситепаже** доступны следующие задачи.</span><span class="sxs-lookup"><span data-stu-id="bc523-107">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="bc523-108">Все приведенные ниже примеры относятся к [сайту][], например: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="bc523-108">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="bc523-109">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="bc523-109">Common task</span></span>                     | <span data-ttu-id="bc523-110">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="bc523-110">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="bc523-111">[Перечисление страниц][]</span><span class="sxs-lookup"><span data-stu-id="bc523-111">[List pages][]</span></span>                  | <span data-ttu-id="bc523-112">ПОЛУЧЕНИЕ/Pages</span><span class="sxs-lookup"><span data-stu-id="bc523-112">GET /pages</span></span>
| <span data-ttu-id="bc523-113">[Вывод страницы][]</span><span class="sxs-lookup"><span data-stu-id="bc523-113">[Get page][]</span></span>                    | <span data-ttu-id="bc523-114">ПОЛУЧЕНИЕ/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="bc523-114">GET /pages/{page-id}</span></span>
| <span data-ttu-id="bc523-115">[создание][];</span><span class="sxs-lookup"><span data-stu-id="bc523-115">[Create][]</span></span>                      | <span data-ttu-id="bc523-116">POST/Pages</span><span class="sxs-lookup"><span data-stu-id="bc523-116">POST /pages</span></span>
| <span data-ttu-id="bc523-117">[удаление][];</span><span class="sxs-lookup"><span data-stu-id="bc523-117">[Delete][]</span></span>                      | <span data-ttu-id="bc523-118">Удаление/Пажес/{Паже-ИД}</span><span class="sxs-lookup"><span data-stu-id="bc523-118">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="bc523-119">[публикация][];</span><span class="sxs-lookup"><span data-stu-id="bc523-119">[Publish][]</span></span>                     | <span data-ttu-id="bc523-120">POST/Пажес/{Паже-ИД}/публиш</span><span class="sxs-lookup"><span data-stu-id="bc523-120">POST /pages/{page-id}/publish</span></span>

[Перечисление страниц]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Вывод страницы]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Создание]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[публикация]: ../api/sitepage-publish.md;
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="bc523-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc523-126">JSON representation</span></span>

<span data-ttu-id="bc523-127">Ниже показано представление ресурса **ситепаже** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc523-127">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc523-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc523-128">Properties</span></span>

<span data-ttu-id="bc523-129">Ресурс **ситепаже** имеет следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="bc523-129">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="bc523-130">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bc523-130">Property name</span></span>    | <span data-ttu-id="bc523-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc523-131">Type</span></span>                         | <span data-ttu-id="bc523-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc523-132">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="bc523-133">contentType</span><span class="sxs-lookup"><span data-stu-id="bc523-133">contentType</span></span>      | <span data-ttu-id="bc523-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="bc523-134">[contentTypeInfo][]</span></span>          | <span data-ttu-id="bc523-135">Тип контента страницы.</span><span class="sxs-lookup"><span data-stu-id="bc523-135">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="bc523-136">Контент страницы</span><span class="sxs-lookup"><span data-stu-id="bc523-136">Page Content</span></span>

<span data-ttu-id="bc523-137">Ресурс **ситепаже** имеет следующие поля контента.</span><span class="sxs-lookup"><span data-stu-id="bc523-137">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="bc523-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bc523-138">Property name</span></span>      | <span data-ttu-id="bc523-139">Тип</span><span class="sxs-lookup"><span data-stu-id="bc523-139">Type</span></span>                       | <span data-ttu-id="bc523-140">Описание</span><span class="sxs-lookup"><span data-stu-id="bc523-140">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="bc523-141">title</span><span class="sxs-lookup"><span data-stu-id="bc523-141">title</span></span>              | <span data-ttu-id="bc523-142">string</span><span class="sxs-lookup"><span data-stu-id="bc523-142">string</span></span>                     | <span data-ttu-id="bc523-143">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="bc523-143">The title of the page.</span></span>
| <span data-ttu-id="bc523-144">pageLayout</span><span class="sxs-lookup"><span data-stu-id="bc523-144">pageLayout</span></span>         | <span data-ttu-id="bc523-145">string</span><span class="sxs-lookup"><span data-stu-id="bc523-145">string</span></span>                     | <span data-ttu-id="bc523-146">Имя макета страницы.</span><span class="sxs-lookup"><span data-stu-id="bc523-146">The name of the page layout of the page.</span></span>
| <span data-ttu-id="bc523-147">webParts</span><span class="sxs-lookup"><span data-stu-id="bc523-147">webParts</span></span>           | <span data-ttu-id="bc523-148">[Частей][]</span><span class="sxs-lookup"><span data-stu-id="bc523-148">[webPart][]</span></span>                | <span data-ttu-id="bc523-149">Веб-части на странице.</span><span class="sxs-lookup"><span data-stu-id="bc523-149">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="bc523-150">Метаданные для разработки</span><span class="sxs-lookup"><span data-stu-id="bc523-150">Authoring Metadata</span></span>

<span data-ttu-id="bc523-151">Ресурс **ситепаже** содержит следующие метаданные, связанные с созданием и отправкой.</span><span class="sxs-lookup"><span data-stu-id="bc523-151">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="bc523-152">Свойство Публишингстате будет отражать состояние создания страницы, например извлеченный или опубликованный.</span><span class="sxs-lookup"><span data-stu-id="bc523-152">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="bc523-153">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bc523-153">Property name</span></span>          | <span data-ttu-id="bc523-154">Тип</span><span class="sxs-lookup"><span data-stu-id="bc523-154">Type</span></span>                   | <span data-ttu-id="bc523-155">Описание</span><span class="sxs-lookup"><span data-stu-id="bc523-155">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="bc523-156">publishingState</span><span class="sxs-lookup"><span data-stu-id="bc523-156">publishingState</span></span>        | <span data-ttu-id="bc523-157">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="bc523-157">[publicationFacet][]</span></span>   | <span data-ttu-id="bc523-158">Состояние публикации и версия MM.mm страницы.</span><span class="sxs-lookup"><span data-stu-id="bc523-158">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="bc523-159">Ниже перечислены свойства, которые наследуются от ресурса **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="bc523-159">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="bc523-160">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bc523-160">Property name</span></span>        | <span data-ttu-id="bc523-161">Тип</span><span class="sxs-lookup"><span data-stu-id="bc523-161">Type</span></span>              | <span data-ttu-id="bc523-162">Описание</span><span class="sxs-lookup"><span data-stu-id="bc523-162">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="bc523-163">id</span><span class="sxs-lookup"><span data-stu-id="bc523-163">id</span></span>                   | <span data-ttu-id="bc523-164">строка</span><span class="sxs-lookup"><span data-stu-id="bc523-164">string</span></span>            | <span data-ttu-id="bc523-p104">Уникальный идентификатор элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="bc523-167">name</span><span class="sxs-lookup"><span data-stu-id="bc523-167">name</span></span>                 | <span data-ttu-id="bc523-168">string</span><span class="sxs-lookup"><span data-stu-id="bc523-168">string</span></span>            | <span data-ttu-id="bc523-169">Имя или название элемента.</span><span class="sxs-lookup"><span data-stu-id="bc523-169">The name / title of the item.</span></span>
| <span data-ttu-id="bc523-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="bc523-170">createdBy</span></span>            | <span data-ttu-id="bc523-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bc523-171">[identitySet][]</span></span>   | <span data-ttu-id="bc523-172">Удостоверение создателя данного элемента.</span><span class="sxs-lookup"><span data-stu-id="bc523-172">Identity of the creator of this item.</span></span> <span data-ttu-id="bc523-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-173">Read-only.</span></span>
| <span data-ttu-id="bc523-174">eTag</span><span class="sxs-lookup"><span data-stu-id="bc523-174">eTag</span></span>                 | <span data-ttu-id="bc523-175">string</span><span class="sxs-lookup"><span data-stu-id="bc523-175">string</span></span>            | <span data-ttu-id="bc523-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="bc523-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bc523-178">lastModifiedBy</span></span>       | <span data-ttu-id="bc523-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bc523-179">[identitySet][]</span></span>   | <span data-ttu-id="bc523-180">Удостоверение пользователя, который последним изменил данный элемент.</span><span class="sxs-lookup"><span data-stu-id="bc523-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="bc523-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-181">Read-only.</span></span>
| <span data-ttu-id="bc523-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc523-182">lastModifiedDateTime</span></span> | <span data-ttu-id="bc523-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc523-183">DateTimeOffset</span></span>    | <span data-ttu-id="bc523-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bc523-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="bc523-186">parentReference</span></span>      | <span data-ttu-id="bc523-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="bc523-187">[itemReference][]</span></span> | <span data-ttu-id="bc523-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bc523-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="bc523-190">webUrl</span></span>               | <span data-ttu-id="bc523-191">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="bc523-191">string (url)</span></span>      | <span data-ttu-id="bc523-p110">URL-адрес для отображения элемента в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc523-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="bc523-194">Связи</span><span class="sxs-lookup"><span data-stu-id="bc523-194">Relationships</span></span>

<span data-ttu-id="bc523-195">У ресурса **ситепаже** нет отношений с другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="bc523-195">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[сайта]: site.md
[site]: site.md
[Частей]: webpart.md
[webPart]: webpart.md

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
