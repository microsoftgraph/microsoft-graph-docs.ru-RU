---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: f82242da39ebc13d769a0a3471b60dd4ac9df8dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542321"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="6084d-102">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="6084d-102">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6084d-103">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="6084d-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="6084d-104">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="6084d-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6084d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6084d-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="6084d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6084d-106">Properties</span></span>

| <span data-ttu-id="6084d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6084d-107">Property name</span></span>         | <span data-ttu-id="6084d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6084d-108">Type</span></span>   | <span data-ttu-id="6084d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6084d-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="6084d-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="6084d-110">**sortBy**</span></span>            | <span data-ttu-id="6084d-111">string</span><span class="sxs-lookup"><span data-stu-id="6084d-111">string</span></span> | <span data-ttu-id="6084d-112">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="6084d-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="6084d-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="6084d-113">**sortOrder**</span></span>         | <span data-ttu-id="6084d-114">string</span><span class="sxs-lookup"><span data-stu-id="6084d-114">string</span></span> | <span data-ttu-id="6084d-p101">Если значение равно true, то необходимо отсортировать элементы по убыванию. В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="6084d-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="6084d-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="6084d-117">**viewType**</span></span>          | <span data-ttu-id="6084d-118">строка</span><span class="sxs-lookup"><span data-stu-id="6084d-118">string</span></span> | <span data-ttu-id="6084d-119">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="6084d-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="6084d-120">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="6084d-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="6084d-121">Значения свойства sortBy</span><span class="sxs-lookup"><span data-stu-id="6084d-121">sortBy values</span></span>

<span data-ttu-id="6084d-122">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6084d-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="6084d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6084d-123">Value</span></span>                    | <span data-ttu-id="6084d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6084d-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="6084d-125">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="6084d-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="6084d-126">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="6084d-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="6084d-127">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="6084d-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="6084d-128">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="6084d-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="6084d-p102">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**. Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6084d-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="6084d-131">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6084d-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="6084d-132">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="6084d-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="6084d-133">Значения свойства sortOrder</span><span class="sxs-lookup"><span data-stu-id="6084d-133">sortOrder values</span></span>

<span data-ttu-id="6084d-134">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6084d-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="6084d-135">Значение</span><span class="sxs-lookup"><span data-stu-id="6084d-135">Value</span></span>        | <span data-ttu-id="6084d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6084d-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="6084d-137">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="6084d-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="6084d-138">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="6084d-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="6084d-139">Значения свойства viewType</span><span class="sxs-lookup"><span data-stu-id="6084d-139">viewType values</span></span>

<span data-ttu-id="6084d-140">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="6084d-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="6084d-141">Значение</span><span class="sxs-lookup"><span data-stu-id="6084d-141">Value</span></span>        | <span data-ttu-id="6084d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="6084d-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="6084d-143">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="6084d-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="6084d-144">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="6084d-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="6084d-145">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="6084d-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="6084d-146">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="6084d-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
