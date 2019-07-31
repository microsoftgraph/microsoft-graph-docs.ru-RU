---
author: daspek
description: Ресурс contentType представляет тип контента в SharePoint.
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7376b431154595f9b3d2de1931918b629e74acb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012865"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="7de88-103">Тип ресурса contentType</span><span class="sxs-lookup"><span data-stu-id="7de88-103">ContentType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7de88-104">Ресурс **contentType** представляет _тип контента_ в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7de88-104">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="7de88-105">Типы контента позволяют определить набор столбцов, которые должны присутствовать в каждом элементе [**ListItem**][listItem] в [**списке**][list].</span><span class="sxs-lookup"><span data-stu-id="7de88-105">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="7de88-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7de88-106">JSON representation</span></span>

<span data-ttu-id="7de88-107">Ниже показано представление ресурса **contentType** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7de88-107">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="7de88-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7de88-108">Properties</span></span>

| <span data-ttu-id="7de88-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7de88-109">Property name</span></span>     | <span data-ttu-id="7de88-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7de88-110">Type</span></span>                 | <span data-ttu-id="7de88-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7de88-111">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="7de88-112">**description**</span><span class="sxs-lookup"><span data-stu-id="7de88-112">**description**</span></span>   | <span data-ttu-id="7de88-113">строка</span><span class="sxs-lookup"><span data-stu-id="7de88-113">string</span></span>               | <span data-ttu-id="7de88-114">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="7de88-114">The descriptive text for the item.</span></span>
| <span data-ttu-id="7de88-115">**group**</span><span class="sxs-lookup"><span data-stu-id="7de88-115">**group**</span></span>         | <span data-ttu-id="7de88-116">string</span><span class="sxs-lookup"><span data-stu-id="7de88-116">string</span></span>               | <span data-ttu-id="7de88-117">Имя группы, которой принадлежит этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-117">The name of the group this content type belongs to.</span></span> <span data-ttu-id="7de88-118">Позволяет упорядочить связанные типы контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-118">Helps organize related content types.</span></span>
| <span data-ttu-id="7de88-119">**hidden**</span><span class="sxs-lookup"><span data-stu-id="7de88-119">**hidden**</span></span>        | <span data-ttu-id="7de88-120">логический</span><span class="sxs-lookup"><span data-stu-id="7de88-120">boolean</span></span>              | <span data-ttu-id="7de88-121">Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.</span><span class="sxs-lookup"><span data-stu-id="7de88-121">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="7de88-122">**id**</span><span class="sxs-lookup"><span data-stu-id="7de88-122">**id**</span></span>            | <span data-ttu-id="7de88-123">string</span><span class="sxs-lookup"><span data-stu-id="7de88-123">string</span></span>               | <span data-ttu-id="7de88-124">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-124">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7de88-125">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="7de88-125">**inheritedFrom**</span></span> | <span data-ttu-id="7de88-126">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7de88-126">[itemReference][]</span></span>    | <span data-ttu-id="7de88-127">Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-127">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="7de88-128">**name**</span><span class="sxs-lookup"><span data-stu-id="7de88-128">**name**</span></span>          | <span data-ttu-id="7de88-129">string</span><span class="sxs-lookup"><span data-stu-id="7de88-129">string</span></span>               | <span data-ttu-id="7de88-130">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-130">The name of the content type.</span></span>
| <span data-ttu-id="7de88-131">**order**</span><span class="sxs-lookup"><span data-stu-id="7de88-131">**order**</span></span>         | <span data-ttu-id="7de88-132">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="7de88-132">[contentTypeOrder][]</span></span> | <span data-ttu-id="7de88-133">Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="7de88-133">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="7de88-134">**parentId**</span><span class="sxs-lookup"><span data-stu-id="7de88-134">**parentId**</span></span>      | <span data-ttu-id="7de88-135">string</span><span class="sxs-lookup"><span data-stu-id="7de88-135">string</span></span>               | <span data-ttu-id="7de88-136">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-136">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7de88-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="7de88-137">**readOnly**</span></span>      | <span data-ttu-id="7de88-138">boolean</span><span class="sxs-lookup"><span data-stu-id="7de88-138">boolean</span></span>              | <span data-ttu-id="7de88-139">Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.</span><span class="sxs-lookup"><span data-stu-id="7de88-139">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="7de88-140">**sealed**</span><span class="sxs-lookup"><span data-stu-id="7de88-140">**sealed**</span></span>        | <span data-ttu-id="7de88-141">boolean</span><span class="sxs-lookup"><span data-stu-id="7de88-141">boolean</span></span>              | <span data-ttu-id="7de88-142">Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз.</span><span class="sxs-lookup"><span data-stu-id="7de88-142">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="7de88-143">Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.</span><span class="sxs-lookup"><span data-stu-id="7de88-143">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="7de88-144">Связи</span><span class="sxs-lookup"><span data-stu-id="7de88-144">Relationships</span></span>

| <span data-ttu-id="7de88-145">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7de88-145">Property name</span></span>   | <span data-ttu-id="7de88-146">Тип</span><span class="sxs-lookup"><span data-stu-id="7de88-146">Type</span></span>                      | <span data-ttu-id="7de88-147">Описание</span><span class="sxs-lookup"><span data-stu-id="7de88-147">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="7de88-148">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="7de88-148">**columnLinks**</span></span> | <span data-ttu-id="7de88-149">Коллекция [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="7de88-149">[columnLink][] collection</span></span> | <span data-ttu-id="7de88-150">Коллекция столбцов, необходимых для этого типа контента</span><span class="sxs-lookup"><span data-stu-id="7de88-150">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="7de88-151">Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="7de88-151">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
