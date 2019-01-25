---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentType
localization_priority: Normal
ms.openlocfilehash: c90dd8889d07f903a7d3c79d9e4e5db3b9f2a30b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522975"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="2f229-102">Тип ресурса contentType</span><span class="sxs-lookup"><span data-stu-id="2f229-102">ContentType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f229-103">Ресурс **contentType** представляет _тип контента_ в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2f229-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="2f229-104">Типы контента позволяют задать набор столбцов, которые должны присутствовать в каждом элементе [**listItem**][listItem] в [**списке**][list].</span><span class="sxs-lookup"><span data-stu-id="2f229-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="2f229-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2f229-105">JSON representation</span></span>

<span data-ttu-id="2f229-106">Ниже показано представление ресурса **contentType** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f229-106">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

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

## <a name="properties"></a><span data-ttu-id="2f229-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f229-107">Properties</span></span>

| <span data-ttu-id="2f229-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2f229-108">Property name</span></span>     | <span data-ttu-id="2f229-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2f229-109">Type</span></span>                 | <span data-ttu-id="2f229-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f229-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="2f229-111">**description**</span><span class="sxs-lookup"><span data-stu-id="2f229-111">**description**</span></span>   | <span data-ttu-id="2f229-112">string</span><span class="sxs-lookup"><span data-stu-id="2f229-112">string</span></span>               | <span data-ttu-id="2f229-113">Текст с описанием элемента.</span><span class="sxs-lookup"><span data-stu-id="2f229-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="2f229-114">**group**</span><span class="sxs-lookup"><span data-stu-id="2f229-114">**group**</span></span>         | <span data-ttu-id="2f229-115">string</span><span class="sxs-lookup"><span data-stu-id="2f229-115">string</span></span>               | <span data-ttu-id="2f229-116">Имя группы, которой принадлежит этот тип контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="2f229-117">Позволяет упорядочить связанные типы контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-117">Helps organize related content types.</span></span>
| <span data-ttu-id="2f229-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="2f229-118">**hidden**</span></span>        | <span data-ttu-id="2f229-119">boolean</span><span class="sxs-lookup"><span data-stu-id="2f229-119">boolean</span></span>              | <span data-ttu-id="2f229-120">Указывает, является ли данный тип контента скрытым в меню "Создать" в списке.</span><span class="sxs-lookup"><span data-stu-id="2f229-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="2f229-121">**id**</span><span class="sxs-lookup"><span data-stu-id="2f229-121">**id**</span></span>            | <span data-ttu-id="2f229-122">string</span><span class="sxs-lookup"><span data-stu-id="2f229-122">string</span></span>               | <span data-ttu-id="2f229-123">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="2f229-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="2f229-124">**inheritedFrom**</span></span> | <span data-ttu-id="2f229-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2f229-125">[itemReference][]</span></span>    | <span data-ttu-id="2f229-126">Если этот тип контента унаследован от другой области (например, сайта), он будет содержать ссылку на элемент, в котором определен тип контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="2f229-127">**name**</span><span class="sxs-lookup"><span data-stu-id="2f229-127">**name**</span></span>          | <span data-ttu-id="2f229-128">string</span><span class="sxs-lookup"><span data-stu-id="2f229-128">string</span></span>               | <span data-ttu-id="2f229-129">Имя типа контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-129">The name of the content type.</span></span>
| <span data-ttu-id="2f229-130">**order**</span><span class="sxs-lookup"><span data-stu-id="2f229-130">**order**</span></span>         | <span data-ttu-id="2f229-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="2f229-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="2f229-132">Указывает порядок, в котором тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="2f229-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="2f229-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="2f229-133">**parentId**</span></span>      | <span data-ttu-id="2f229-134">string</span><span class="sxs-lookup"><span data-stu-id="2f229-134">string</span></span>               | <span data-ttu-id="2f229-135">Уникальный идентификатор типа контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="2f229-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="2f229-136">**readOnly**</span></span>      | <span data-ttu-id="2f229-137">boolean</span><span class="sxs-lookup"><span data-stu-id="2f229-137">boolean</span></span>              | <span data-ttu-id="2f229-138">Если это свойство имеет значение `true`, вам не удастся изменить тип контента. Чтобы изменить тип контента, потребуется сначала присвоить этому свойству значение `false`.</span><span class="sxs-lookup"><span data-stu-id="2f229-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="2f229-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="2f229-139">**sealed**</span></span>        | <span data-ttu-id="2f229-140">boolean</span><span class="sxs-lookup"><span data-stu-id="2f229-140">boolean</span></span>              | <span data-ttu-id="2f229-141">Если это свойство имеет значение `true`, пользователям не удастся изменить тип контента. Кроме того, вам не удастся изменить тип контента с помощью операции сдвига вниз.</span><span class="sxs-lookup"><span data-stu-id="2f229-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="2f229-142">Только администраторы семейств веб-сайтов могут блокировать или разблокировать типы контента.</span><span class="sxs-lookup"><span data-stu-id="2f229-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="2f229-143">Связи</span><span class="sxs-lookup"><span data-stu-id="2f229-143">Relationships</span></span>

| <span data-ttu-id="2f229-144">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2f229-144">Property name</span></span>   | <span data-ttu-id="2f229-145">Тип</span><span class="sxs-lookup"><span data-stu-id="2f229-145">Type</span></span>                      | <span data-ttu-id="2f229-146">Описание</span><span class="sxs-lookup"><span data-stu-id="2f229-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="2f229-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="2f229-147">**columnLinks**</span></span> | <span data-ttu-id="2f229-148">Коллекция [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="2f229-148">[columnLink][] collection</span></span> | <span data-ttu-id="2f229-149">Коллекция столбцов, необходимых для этого типа контента</span><span class="sxs-lookup"><span data-stu-id="2f229-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="2f229-150">Дополнительные сведения см. в статье [Общие сведения о типах контента и их публикации][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="2f229-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/contentType.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
