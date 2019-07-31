---
author: JeremyKelley
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5238c749d509339cd0e922e49b7e2d4d2da3b23f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973550"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="efeee-103">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="efeee-103">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efeee-104">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="efeee-104">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="efeee-105">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="efeee-105">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efeee-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efeee-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a><span data-ttu-id="efeee-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="efeee-107">Properties</span></span>

| <span data-ttu-id="efeee-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="efeee-108">Property name</span></span>         | <span data-ttu-id="efeee-109">Тип</span><span class="sxs-lookup"><span data-stu-id="efeee-109">Type</span></span>   | <span data-ttu-id="efeee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="efeee-110">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="efeee-111">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="efeee-111">**sortBy**</span></span>            | <span data-ttu-id="efeee-112">string</span><span class="sxs-lookup"><span data-stu-id="efeee-112">string</span></span> | <span data-ttu-id="efeee-113">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="efeee-113">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="efeee-114">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="efeee-114">**sortOrder**</span></span>         | <span data-ttu-id="efeee-115">string</span><span class="sxs-lookup"><span data-stu-id="efeee-115">string</span></span> | <span data-ttu-id="efeee-p101">Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="efeee-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="efeee-118">**viewType**</span><span class="sxs-lookup"><span data-stu-id="efeee-118">**viewType**</span></span>          | <span data-ttu-id="efeee-119">строка</span><span class="sxs-lookup"><span data-stu-id="efeee-119">string</span></span> | <span data-ttu-id="efeee-120">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="efeee-120">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="efeee-121">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="efeee-121">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="efeee-122">Значения свойства sortBy</span><span class="sxs-lookup"><span data-stu-id="efeee-122">sortBy values</span></span>

<span data-ttu-id="efeee-123">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="efeee-123">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="efeee-124">Значение</span><span class="sxs-lookup"><span data-stu-id="efeee-124">Value</span></span>                    | <span data-ttu-id="efeee-125">Описание</span><span class="sxs-lookup"><span data-stu-id="efeee-125">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="efeee-126">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="efeee-126">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="efeee-127">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="efeee-127">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="efeee-128">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="efeee-128">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="efeee-129">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="efeee-129">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="efeee-p102">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="efeee-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="efeee-132">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="efeee-132">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="efeee-133">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="efeee-133">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="efeee-134">Значения свойства sortOrder</span><span class="sxs-lookup"><span data-stu-id="efeee-134">sortOrder values</span></span>

<span data-ttu-id="efeee-135">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="efeee-135">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="efeee-136">Значение</span><span class="sxs-lookup"><span data-stu-id="efeee-136">Value</span></span>        | <span data-ttu-id="efeee-137">Описание</span><span class="sxs-lookup"><span data-stu-id="efeee-137">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="efeee-138">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="efeee-138">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="efeee-139">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="efeee-139">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="efeee-140">Значения свойства viewType</span><span class="sxs-lookup"><span data-stu-id="efeee-140">viewType values</span></span>

<span data-ttu-id="efeee-141">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="efeee-141">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="efeee-142">Значение</span><span class="sxs-lookup"><span data-stu-id="efeee-142">Value</span></span>        | <span data-ttu-id="efeee-143">Описание</span><span class="sxs-lookup"><span data-stu-id="efeee-143">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="efeee-144">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="efeee-144">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="efeee-145">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="efeee-145">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="efeee-146">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="efeee-146">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="efeee-147">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="efeee-147">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
