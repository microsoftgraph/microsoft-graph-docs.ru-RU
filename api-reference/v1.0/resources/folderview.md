---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 2b254568ec97bb5bce49e1143dbb83a183fade11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824173"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="2046f-102">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="2046f-102">FolderView resource type</span></span>

<span data-ttu-id="2046f-103">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="2046f-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="2046f-104">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="2046f-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2046f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2046f-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="2046f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2046f-106">Properties</span></span>

| <span data-ttu-id="2046f-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2046f-107">Property name</span></span>         | <span data-ttu-id="2046f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2046f-108">Type</span></span>   | <span data-ttu-id="2046f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2046f-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="2046f-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="2046f-110">**sortBy**</span></span>            | <span data-ttu-id="2046f-111">строка</span><span class="sxs-lookup"><span data-stu-id="2046f-111">string</span></span> | <span data-ttu-id="2046f-112">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="2046f-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="2046f-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="2046f-113">**sortOrder**</span></span>         | <span data-ttu-id="2046f-114">строка</span><span class="sxs-lookup"><span data-stu-id="2046f-114">string</span></span> | <span data-ttu-id="2046f-115">Если значение равно true, то необходимо отсортировать элементы по убыванию.</span><span class="sxs-lookup"><span data-stu-id="2046f-115">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="2046f-116">В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="2046f-116">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="2046f-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="2046f-117">**viewType**</span></span>          | <span data-ttu-id="2046f-118">строка</span><span class="sxs-lookup"><span data-stu-id="2046f-118">string</span></span> | <span data-ttu-id="2046f-119">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="2046f-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="2046f-120">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="2046f-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="2046f-121">Параметры sortBy</span><span class="sxs-lookup"><span data-stu-id="2046f-121">sortBy options</span></span>

<span data-ttu-id="2046f-122">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="2046f-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="2046f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2046f-123">Value</span></span>                    | <span data-ttu-id="2046f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2046f-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="2046f-125">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="2046f-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="2046f-126">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="2046f-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="2046f-127">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="2046f-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="2046f-128">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="2046f-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="2046f-129">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**.</span><span class="sxs-lookup"><span data-stu-id="2046f-129">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="2046f-130">Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2046f-130">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="2046f-131">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2046f-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="2046f-132">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="2046f-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="2046f-133">Параметры sortOrder</span><span class="sxs-lookup"><span data-stu-id="2046f-133">sortOrder options</span></span>

<span data-ttu-id="2046f-134">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="2046f-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="2046f-135">Значение</span><span class="sxs-lookup"><span data-stu-id="2046f-135">Value</span></span>        | <span data-ttu-id="2046f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="2046f-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="2046f-137">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="2046f-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="2046f-138">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="2046f-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="2046f-139">Параметры viewType</span><span class="sxs-lookup"><span data-stu-id="2046f-139">viewType options</span></span>

<span data-ttu-id="2046f-140">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="2046f-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="2046f-141">Значение</span><span class="sxs-lookup"><span data-stu-id="2046f-141">Value</span></span>        | <span data-ttu-id="2046f-142">Описание</span><span class="sxs-lookup"><span data-stu-id="2046f-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="2046f-143">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="2046f-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="2046f-144">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="2046f-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="2046f-145">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="2046f-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="2046f-146">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="2046f-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->
