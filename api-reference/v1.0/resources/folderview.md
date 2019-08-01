---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67ec2e079348cc45664804d39314e6c81f4548e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032454"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="688d9-103">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="688d9-103">FolderView resource type</span></span>

<span data-ttu-id="688d9-104">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="688d9-104">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="688d9-105">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="688d9-105">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="688d9-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="688d9-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="688d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="688d9-107">Properties</span></span>

| <span data-ttu-id="688d9-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="688d9-108">Property name</span></span>         | <span data-ttu-id="688d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="688d9-109">Type</span></span>   | <span data-ttu-id="688d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="688d9-110">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="688d9-111">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="688d9-111">**sortBy**</span></span>            | <span data-ttu-id="688d9-112">string</span><span class="sxs-lookup"><span data-stu-id="688d9-112">string</span></span> | <span data-ttu-id="688d9-113">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="688d9-113">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="688d9-114">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="688d9-114">**sortOrder**</span></span>         | <span data-ttu-id="688d9-115">string</span><span class="sxs-lookup"><span data-stu-id="688d9-115">string</span></span> | <span data-ttu-id="688d9-p101">Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="688d9-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="688d9-118">**viewType**</span><span class="sxs-lookup"><span data-stu-id="688d9-118">**viewType**</span></span>          | <span data-ttu-id="688d9-119">строка</span><span class="sxs-lookup"><span data-stu-id="688d9-119">string</span></span> | <span data-ttu-id="688d9-120">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="688d9-120">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="688d9-121">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="688d9-121">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="688d9-122">Параметры sortBy</span><span class="sxs-lookup"><span data-stu-id="688d9-122">sortBy options</span></span>

<span data-ttu-id="688d9-123">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="688d9-123">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="688d9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="688d9-124">Value</span></span>                    | <span data-ttu-id="688d9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="688d9-125">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="688d9-126">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="688d9-126">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="688d9-127">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="688d9-127">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="688d9-128">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="688d9-128">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="688d9-129">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="688d9-129">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="688d9-p102">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="688d9-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="688d9-132">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="688d9-132">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="688d9-133">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="688d9-133">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="688d9-134">Параметры sortOrder</span><span class="sxs-lookup"><span data-stu-id="688d9-134">sortOrder options</span></span>

<span data-ttu-id="688d9-135">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="688d9-135">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="688d9-136">Значение</span><span class="sxs-lookup"><span data-stu-id="688d9-136">Value</span></span>        | <span data-ttu-id="688d9-137">Описание</span><span class="sxs-lookup"><span data-stu-id="688d9-137">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="688d9-138">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="688d9-138">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="688d9-139">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="688d9-139">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="688d9-140">Параметры viewType</span><span class="sxs-lookup"><span data-stu-id="688d9-140">viewType options</span></span>

<span data-ttu-id="688d9-141">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="688d9-141">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="688d9-142">Значение</span><span class="sxs-lookup"><span data-stu-id="688d9-142">Value</span></span>        | <span data-ttu-id="688d9-143">Описание</span><span class="sxs-lookup"><span data-stu-id="688d9-143">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="688d9-144">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="688d9-144">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="688d9-145">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="688d9-145">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="688d9-146">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="688d9-146">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="688d9-147">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="688d9-147">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
