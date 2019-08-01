---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: Ресурс contentType представляет тип контента в SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b26f9b7a3bafb7b6185aa781c1f842f7c20adab3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029640"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="a33a8-103">Тип ресурса contentType</span><span class="sxs-lookup"><span data-stu-id="a33a8-103">ContentType resource type</span></span>

<span data-ttu-id="a33a8-104">Ресурс **contentType** представляет _тип контента_ в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a33a8-104">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="a33a8-105">Типы контента позволяют определить набор столбцов, которые должны присутствовать в каждом элементе [**ListItem**][listItem] в [**списке**][list].</span><span class="sxs-lookup"><span data-stu-id="a33a8-105">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="a33a8-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a33a8-106">JSON representation</span></span>

<span data-ttu-id="a33a8-107">Ниже показано представление ресурса **contentType** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a33a8-107">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="a33a8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a33a8-108">Properties</span></span>

| <span data-ttu-id="a33a8-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a33a8-109">Property name</span></span>     | <span data-ttu-id="a33a8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a33a8-110">Type</span></span>                 | <span data-ttu-id="a33a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a33a8-111">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="a33a8-112">**description**</span><span class="sxs-lookup"><span data-stu-id="a33a8-112">**description**</span></span>   | <span data-ttu-id="a33a8-113">строка</span><span class="sxs-lookup"><span data-stu-id="a33a8-113">string</span></span>               | <span data-ttu-id="a33a8-114">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-114">The descriptive text for the item.</span></span>
| <span data-ttu-id="a33a8-115">**group**</span><span class="sxs-lookup"><span data-stu-id="a33a8-115">**group**</span></span>         | <span data-ttu-id="a33a8-116">string</span><span class="sxs-lookup"><span data-stu-id="a33a8-116">string</span></span>               | <span data-ttu-id="a33a8-117">Имя группы, которой принадлежит этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-117">The name of the group this content type belongs to.</span></span> <span data-ttu-id="a33a8-118">Позволяет упорядочить связанные типы контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-118">Helps organize related content types.</span></span>
| <span data-ttu-id="a33a8-119">**hidden**</span><span class="sxs-lookup"><span data-stu-id="a33a8-119">**hidden**</span></span>        | <span data-ttu-id="a33a8-120">логический</span><span class="sxs-lookup"><span data-stu-id="a33a8-120">boolean</span></span>              | <span data-ttu-id="a33a8-121">Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.</span><span class="sxs-lookup"><span data-stu-id="a33a8-121">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="a33a8-122">**id**</span><span class="sxs-lookup"><span data-stu-id="a33a8-122">**id**</span></span>            | <span data-ttu-id="a33a8-123">string</span><span class="sxs-lookup"><span data-stu-id="a33a8-123">string</span></span>               | <span data-ttu-id="a33a8-124">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-124">The unique identifier of the content type.</span></span>
| <span data-ttu-id="a33a8-125">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="a33a8-125">**inheritedFrom**</span></span> | <span data-ttu-id="a33a8-126">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="a33a8-126">[itemReference][]</span></span>    | <span data-ttu-id="a33a8-127">Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-127">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="a33a8-128">**name**</span><span class="sxs-lookup"><span data-stu-id="a33a8-128">**name**</span></span>          | <span data-ttu-id="a33a8-129">string</span><span class="sxs-lookup"><span data-stu-id="a33a8-129">string</span></span>               | <span data-ttu-id="a33a8-130">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-130">The name of the content type.</span></span>
| <span data-ttu-id="a33a8-131">**order**</span><span class="sxs-lookup"><span data-stu-id="a33a8-131">**order**</span></span>         | <span data-ttu-id="a33a8-132">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="a33a8-132">[contentTypeOrder][]</span></span> | <span data-ttu-id="a33a8-133">Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="a33a8-133">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="a33a8-134">**parentId**</span><span class="sxs-lookup"><span data-stu-id="a33a8-134">**parentId**</span></span>      | <span data-ttu-id="a33a8-135">string</span><span class="sxs-lookup"><span data-stu-id="a33a8-135">string</span></span>               | <span data-ttu-id="a33a8-136">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-136">The unique identifier of the content type.</span></span>
| <span data-ttu-id="a33a8-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="a33a8-137">**readOnly**</span></span>      | <span data-ttu-id="a33a8-138">boolean</span><span class="sxs-lookup"><span data-stu-id="a33a8-138">boolean</span></span>              | <span data-ttu-id="a33a8-139">Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.</span><span class="sxs-lookup"><span data-stu-id="a33a8-139">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="a33a8-140">**sealed**</span><span class="sxs-lookup"><span data-stu-id="a33a8-140">**sealed**</span></span>        | <span data-ttu-id="a33a8-141">boolean</span><span class="sxs-lookup"><span data-stu-id="a33a8-141">boolean</span></span>              | <span data-ttu-id="a33a8-142">Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз.</span><span class="sxs-lookup"><span data-stu-id="a33a8-142">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="a33a8-143">Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.</span><span class="sxs-lookup"><span data-stu-id="a33a8-143">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="a33a8-144">Связи</span><span class="sxs-lookup"><span data-stu-id="a33a8-144">Relationships</span></span>

| <span data-ttu-id="a33a8-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a33a8-145">Property name</span></span>   | <span data-ttu-id="a33a8-146">Тип</span><span class="sxs-lookup"><span data-stu-id="a33a8-146">Type</span></span>                      | <span data-ttu-id="a33a8-147">Описание</span><span class="sxs-lookup"><span data-stu-id="a33a8-147">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="a33a8-148">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="a33a8-148">**columnLinks**</span></span> | <span data-ttu-id="a33a8-149">Коллекция [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="a33a8-149">[columnLink][] collection</span></span> | <span data-ttu-id="a33a8-150">Коллекция столбцов, необходимых для этого типа контента</span><span class="sxs-lookup"><span data-stu-id="a33a8-150">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="a33a8-151">Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="a33a8-151">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
