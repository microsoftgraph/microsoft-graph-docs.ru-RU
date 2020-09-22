---
author: JeremyKelley
description: Ресурс FolderView предоставляет или задает рекомендации для пользовательского интерфейса папки.
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9657e22104f621cf59bab48c40e6aaab911dd08c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058449"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="6ea25-103">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="6ea25-103">FolderView resource type</span></span>

<span data-ttu-id="6ea25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ea25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ea25-105">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="6ea25-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="6ea25-106">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="6ea25-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ea25-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ea25-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6ea25-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ea25-108">Properties</span></span>

| <span data-ttu-id="6ea25-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6ea25-109">Property name</span></span>         | <span data-ttu-id="6ea25-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6ea25-110">Type</span></span>   | <span data-ttu-id="6ea25-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea25-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="6ea25-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="6ea25-112">**sortBy**</span></span>            | <span data-ttu-id="6ea25-113">строка</span><span class="sxs-lookup"><span data-stu-id="6ea25-113">string</span></span> | <span data-ttu-id="6ea25-114">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="6ea25-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="6ea25-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="6ea25-115">**sortOrder**</span></span>         | <span data-ttu-id="6ea25-116">строка</span><span class="sxs-lookup"><span data-stu-id="6ea25-116">string</span></span> | <span data-ttu-id="6ea25-p101">Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="6ea25-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="6ea25-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="6ea25-119">**viewType**</span></span>          | <span data-ttu-id="6ea25-120">строка</span><span class="sxs-lookup"><span data-stu-id="6ea25-120">string</span></span> | <span data-ttu-id="6ea25-121">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="6ea25-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="6ea25-122">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="6ea25-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="6ea25-123">Значения свойства sortBy</span><span class="sxs-lookup"><span data-stu-id="6ea25-123">sortBy values</span></span>

<span data-ttu-id="6ea25-124">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6ea25-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="6ea25-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6ea25-125">Value</span></span>                    | <span data-ttu-id="6ea25-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea25-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="6ea25-127">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="6ea25-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="6ea25-128">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="6ea25-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="6ea25-129">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="6ea25-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="6ea25-130">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="6ea25-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="6ea25-p102">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6ea25-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="6ea25-133">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6ea25-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="6ea25-134">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="6ea25-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="6ea25-135">Значения свойства sortOrder</span><span class="sxs-lookup"><span data-stu-id="6ea25-135">sortOrder values</span></span>

<span data-ttu-id="6ea25-136">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6ea25-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="6ea25-137">Значение</span><span class="sxs-lookup"><span data-stu-id="6ea25-137">Value</span></span>        | <span data-ttu-id="6ea25-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea25-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="6ea25-139">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="6ea25-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="6ea25-140">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="6ea25-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="6ea25-141">Значения свойства viewType</span><span class="sxs-lookup"><span data-stu-id="6ea25-141">viewType values</span></span>

<span data-ttu-id="6ea25-142">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6ea25-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="6ea25-143">Значение</span><span class="sxs-lookup"><span data-stu-id="6ea25-143">Value</span></span>        | <span data-ttu-id="6ea25-144">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea25-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="6ea25-145">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="6ea25-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="6ea25-146">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="6ea25-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="6ea25-147">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="6ea25-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="6ea25-148">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="6ea25-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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


