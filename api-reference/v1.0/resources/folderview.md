---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 01b9860284f87ea31a969055fe2bfc7da624d3b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564115"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="9c83d-102">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="9c83d-102">FolderView resource type</span></span>

<span data-ttu-id="9c83d-103">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="9c83d-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="9c83d-104">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="9c83d-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c83d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c83d-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="9c83d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c83d-106">Properties</span></span>

| <span data-ttu-id="9c83d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9c83d-107">Property name</span></span>         | <span data-ttu-id="9c83d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9c83d-108">Type</span></span>   | <span data-ttu-id="9c83d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c83d-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="9c83d-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="9c83d-110">**sortBy**</span></span>            | <span data-ttu-id="9c83d-111">string</span><span class="sxs-lookup"><span data-stu-id="9c83d-111">string</span></span> | <span data-ttu-id="9c83d-112">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="9c83d-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="9c83d-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="9c83d-113">**sortOrder**</span></span>         | <span data-ttu-id="9c83d-114">string</span><span class="sxs-lookup"><span data-stu-id="9c83d-114">string</span></span> | <span data-ttu-id="9c83d-p101">Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="9c83d-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="9c83d-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="9c83d-117">**viewType**</span></span>          | <span data-ttu-id="9c83d-118">строка</span><span class="sxs-lookup"><span data-stu-id="9c83d-118">string</span></span> | <span data-ttu-id="9c83d-119">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="9c83d-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="9c83d-120">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="9c83d-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="9c83d-121">Параметры sortBy</span><span class="sxs-lookup"><span data-stu-id="9c83d-121">sortBy options</span></span>

<span data-ttu-id="9c83d-122">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="9c83d-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="9c83d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9c83d-123">Value</span></span>                    | <span data-ttu-id="9c83d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9c83d-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="9c83d-125">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="9c83d-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="9c83d-126">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="9c83d-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="9c83d-127">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="9c83d-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="9c83d-128">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="9c83d-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="9c83d-p102">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="9c83d-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="9c83d-131">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="9c83d-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="9c83d-132">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="9c83d-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="9c83d-133">Параметры sortOrder</span><span class="sxs-lookup"><span data-stu-id="9c83d-133">sortOrder options</span></span>

<span data-ttu-id="9c83d-134">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="9c83d-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="9c83d-135">Значение</span><span class="sxs-lookup"><span data-stu-id="9c83d-135">Value</span></span>        | <span data-ttu-id="9c83d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9c83d-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="9c83d-137">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="9c83d-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="9c83d-138">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="9c83d-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="9c83d-139">Параметры viewType</span><span class="sxs-lookup"><span data-stu-id="9c83d-139">viewType options</span></span>

<span data-ttu-id="9c83d-140">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="9c83d-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="9c83d-141">Значение</span><span class="sxs-lookup"><span data-stu-id="9c83d-141">Value</span></span>        | <span data-ttu-id="9c83d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="9c83d-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="9c83d-143">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="9c83d-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="9c83d-144">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="9c83d-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="9c83d-145">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="9c83d-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="9c83d-146">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="9c83d-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
