---
author: daspek
description: Ресурс contentType представляет тип контента в SharePoint.
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2af8291f33f62517e33349fb66408131f576e89a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444296"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="6a7ac-103">тип ресурса contentType</span><span class="sxs-lookup"><span data-stu-id="6a7ac-103">contentType resource type</span></span>

<span data-ttu-id="6a7ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a7ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a7ac-105">Представляет тип _контента в_ SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-105">Represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="6a7ac-106">Типы контента позволяют определить набор столбцов, которые должны присутствовать на каждом [**listItem**][listItem] в [**списке.**][list]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

## <a name="properties"></a><span data-ttu-id="6a7ac-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a7ac-107">Properties</span></span>

| <span data-ttu-id="6a7ac-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6a7ac-108">Property name</span></span>     | <span data-ttu-id="6a7ac-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a7ac-109">Type</span></span>                 | <span data-ttu-id="6a7ac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a7ac-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="6a7ac-111">**description**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-111">**description**</span></span>   | <span data-ttu-id="6a7ac-112">строка</span><span class="sxs-lookup"><span data-stu-id="6a7ac-112">string</span></span>               | <span data-ttu-id="6a7ac-113">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="6a7ac-114">**group**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-114">**group**</span></span>         | <span data-ttu-id="6a7ac-115">string</span><span class="sxs-lookup"><span data-stu-id="6a7ac-115">string</span></span>               | <span data-ttu-id="6a7ac-116">Имя группы, которой принадлежит этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="6a7ac-117">Позволяет упорядочить связанные типы контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-117">Helps organize related content types.</span></span>
| <span data-ttu-id="6a7ac-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-118">**hidden**</span></span>        | <span data-ttu-id="6a7ac-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a7ac-119">Boolean</span></span>              | <span data-ttu-id="6a7ac-120">Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="6a7ac-121">**id**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-121">**id**</span></span>            | <span data-ttu-id="6a7ac-122">string</span><span class="sxs-lookup"><span data-stu-id="6a7ac-122">string</span></span>               | <span data-ttu-id="6a7ac-123">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="6a7ac-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-124">**inheritedFrom**</span></span> | <span data-ttu-id="6a7ac-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-125">[itemReference][]</span></span>    | <span data-ttu-id="6a7ac-126">Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="6a7ac-127">**name**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-127">**name**</span></span>          | <span data-ttu-id="6a7ac-128">string</span><span class="sxs-lookup"><span data-stu-id="6a7ac-128">string</span></span>               | <span data-ttu-id="6a7ac-129">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-129">The name of the content type.</span></span>
| <span data-ttu-id="6a7ac-130">**order**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-130">**order**</span></span>         | <span data-ttu-id="6a7ac-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="6a7ac-132">Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="6a7ac-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-133">**parentId**</span></span>      | <span data-ttu-id="6a7ac-134">string</span><span class="sxs-lookup"><span data-stu-id="6a7ac-134">string</span></span>               | <span data-ttu-id="6a7ac-135">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="6a7ac-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-136">**readOnly**</span></span>      | <span data-ttu-id="6a7ac-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a7ac-137">Boolean</span></span>              | <span data-ttu-id="6a7ac-138">Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="6a7ac-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-139">**sealed**</span></span>        | <span data-ttu-id="6a7ac-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a7ac-140">Boolean</span></span>              | <span data-ttu-id="6a7ac-141">Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="6a7ac-142">Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-142">Only site collection administrators can seal or unseal content types.</span></span>
| <span data-ttu-id="6a7ac-143">**isBuiltIn**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-143">**isBuiltIn**</span></span>            | <span data-ttu-id="6a7ac-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a7ac-144">Boolean</span></span>| <span data-ttu-id="6a7ac-145">Указывает, является ли тип контента встроенным типом контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-145">Specifies if a content type is a built-in content type.</span></span> 
| <span data-ttu-id="6a7ac-146">**documentSet**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-146">**documentSet**</span></span>       | <span data-ttu-id="6a7ac-147">[documentSet][]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-147">[documentSet][]</span></span>      | <span data-ttu-id="6a7ac-148">[Метаданные набора](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) документов.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-148">[Document Set](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) metadata.</span></span>
| <span data-ttu-id="6a7ac-149">**documentTemplate**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-149">**documentTemplate**</span></span>  | <span data-ttu-id="6a7ac-150">[documentSetContent][]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-150">[documentSetContent][]</span></span> | <span data-ttu-id="6a7ac-151">Метаданные шаблона документов.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-151">Document template metadata.</span></span> <span data-ttu-id="6a7ac-152">Чтобы убедиться, что документы имеют согласованный контент на сайте и его подмышках, можно связать шаблон Word, Excel или PowerPoint с типом контента сайта.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-152">To make sure that documents have consistent content across a site and its subsites, you can associate a Word, Excel, or PowerPoint template with a site content type.</span></span>
| <span data-ttu-id="6a7ac-153">**associatedHubsUrls**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-153">**associatedHubsUrls**</span></span>       | <span data-ttu-id="6a7ac-154">Коллекция (строка)</span><span class="sxs-lookup"><span data-stu-id="6a7ac-154">Collection(string)</span></span> | <span data-ttu-id="6a7ac-155">Список канонических URL-адресов для сайтов-концентраторов, с которыми связан этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-155">List of canonical URLs for hub sites with which this content type is associated to.</span></span> <span data-ttu-id="6a7ac-156">Это будет содержать все концентраторы, где этот тип контента находится в очереди для принудительного или уже принудительного.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-156">This will contain all hubsites where this content type is queued to be enforced or is already enforced.</span></span> <span data-ttu-id="6a7ac-157">Применение типа контента означает, что тип контента будет применяться к спискам на принудительном сайте.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-157">Enforcing a content type means that the content type will be applied to the lists in the enforced sites.</span></span>
| <span data-ttu-id="6a7ac-158">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-158">**propagateChanges**</span></span>   | <span data-ttu-id="6a7ac-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a7ac-159">Boolean</span></span>              | <span data-ttu-id="6a7ac-160">Если какие-либо изменения, внесенные в тип контента, будут нажаты на унаследованные типы контента и списки, которые `true` реализуют тип контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-160">If `true`, any changes made to the content type will be pushed to inherited content types and lists that implement the content type.</span></span>



## <a name="relationships"></a><span data-ttu-id="6a7ac-161">Связи</span><span class="sxs-lookup"><span data-stu-id="6a7ac-161">Relationships</span></span>

| <span data-ttu-id="6a7ac-162">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6a7ac-162">Property name</span></span>   | <span data-ttu-id="6a7ac-163">Тип</span><span class="sxs-lookup"><span data-stu-id="6a7ac-163">Type</span></span>                      | <span data-ttu-id="6a7ac-164">Описание</span><span class="sxs-lookup"><span data-stu-id="6a7ac-164">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="6a7ac-165">**база**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-165">**base**</span></span>   | <span data-ttu-id="6a7ac-166">[contentType][]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-166">[contentType][]</span></span>  | <span data-ttu-id="6a7ac-167">Родительский contentType, из которого получен этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-167">Parent contentType from which this content type is derived.</span></span> 
| <span data-ttu-id="6a7ac-168">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-168">**columnLinks**</span></span> | <span data-ttu-id="6a7ac-169">Коллекция [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="6a7ac-169">[columnLink][] collection</span></span> | <span data-ttu-id="6a7ac-170">Коллекция столбцов, необходимых для этого типа контента</span><span class="sxs-lookup"><span data-stu-id="6a7ac-170">The collection of columns that are required by this content type</span></span>
| <span data-ttu-id="6a7ac-171">**baseTypes**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-171">**baseTypes**</span></span>   | <span data-ttu-id="6a7ac-172">Коллекция ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="6a7ac-172">Collection([contentType][])</span></span>     | <span data-ttu-id="6a7ac-173">Коллекция типов контента, которые являются предками этого типа контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-173">The collection of content types that are ancestors of this content type.</span></span>
| <span data-ttu-id="6a7ac-174">**columnPositions**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-174">**columnPositions**</span></span>       | <span data-ttu-id="6a7ac-175">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="6a7ac-175">Collection([columnDefinition][])</span></span> | <span data-ttu-id="6a7ac-176">Сведения о порядке столбца в типе контента.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-176">Column order information in a content type.</span></span>
| <span data-ttu-id="6a7ac-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-177">**columns**</span></span>     | <span data-ttu-id="6a7ac-178">Коллекция ([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="6a7ac-178">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="6a7ac-179">Коллекция определений столбцов для этого contentType.</span><span class="sxs-lookup"><span data-stu-id="6a7ac-179">The collection of column definitions for this contentType.</span></span>

<span data-ttu-id="6a7ac-180">Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="6a7ac-180">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a><span data-ttu-id="6a7ac-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a7ac-188">JSON representation</span></span>

<span data-ttu-id="6a7ac-189">Ниже приводится представление JSON ресурса **contentType.**</span><span class="sxs-lookup"><span data-stu-id="6a7ac-189">The following is a JSON representation of a **contentType** resource.</span></span>

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


