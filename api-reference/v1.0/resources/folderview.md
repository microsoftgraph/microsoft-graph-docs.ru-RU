---
author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2af23d76083b14bf26afe2cfd9a67388870d1f8a
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240026"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="3d61d-103">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="3d61d-103">FolderView resource type</span></span>

<span data-ttu-id="3d61d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d61d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d61d-105">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="3d61d-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="3d61d-106">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="3d61d-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d61d-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d61d-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="3d61d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d61d-108">Properties</span></span>

| <span data-ttu-id="3d61d-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3d61d-109">Property name</span></span>         | <span data-ttu-id="3d61d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3d61d-110">Type</span></span>   | <span data-ttu-id="3d61d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d61d-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="3d61d-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="3d61d-112">**sortBy**</span></span>            | <span data-ttu-id="3d61d-113">строка</span><span class="sxs-lookup"><span data-stu-id="3d61d-113">string</span></span> | <span data-ttu-id="3d61d-114">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="3d61d-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="3d61d-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="3d61d-115">**sortOrder**</span></span>         | <span data-ttu-id="3d61d-116">строка</span><span class="sxs-lookup"><span data-stu-id="3d61d-116">string</span></span> | <span data-ttu-id="3d61d-p101">Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="3d61d-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="3d61d-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="3d61d-119">**viewType**</span></span>          | <span data-ttu-id="3d61d-120">строка</span><span class="sxs-lookup"><span data-stu-id="3d61d-120">string</span></span> | <span data-ttu-id="3d61d-121">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="3d61d-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="3d61d-122">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="3d61d-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="3d61d-123">Параметры sortBy</span><span class="sxs-lookup"><span data-stu-id="3d61d-123">sortBy options</span></span>

<span data-ttu-id="3d61d-124">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="3d61d-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="3d61d-125">Значение</span><span class="sxs-lookup"><span data-stu-id="3d61d-125">Value</span></span>                    | <span data-ttu-id="3d61d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3d61d-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="3d61d-127">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="3d61d-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="3d61d-128">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="3d61d-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="3d61d-129">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="3d61d-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="3d61d-130">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="3d61d-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="3d61d-p102">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="3d61d-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="3d61d-133">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="3d61d-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="3d61d-134">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="3d61d-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="3d61d-135">Параметры sortOrder</span><span class="sxs-lookup"><span data-stu-id="3d61d-135">sortOrder options</span></span>

<span data-ttu-id="3d61d-136">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="3d61d-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="3d61d-137">Значение</span><span class="sxs-lookup"><span data-stu-id="3d61d-137">Value</span></span>        | <span data-ttu-id="3d61d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3d61d-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="3d61d-139">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="3d61d-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="3d61d-140">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="3d61d-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="3d61d-141">Параметры viewType</span><span class="sxs-lookup"><span data-stu-id="3d61d-141">viewType options</span></span>

<span data-ttu-id="3d61d-142">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="3d61d-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="3d61d-143">Значение</span><span class="sxs-lookup"><span data-stu-id="3d61d-143">Value</span></span>        | <span data-ttu-id="3d61d-144">Описание</span><span class="sxs-lookup"><span data-stu-id="3d61d-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="3d61d-145">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="3d61d-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="3d61d-146">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="3d61d-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="3d61d-147">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="3d61d-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="3d61d-148">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="3d61d-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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

