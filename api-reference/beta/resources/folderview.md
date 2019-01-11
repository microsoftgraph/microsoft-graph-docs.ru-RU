---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 717dd93d82f109926cabf0168e4e176d7c68cd35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861539"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="e0dfb-102">Тип ресурса FolderView</span><span class="sxs-lookup"><span data-stu-id="e0dfb-102">FolderView resource type</span></span>

> <span data-ttu-id="e0dfb-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0dfb-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0dfb-105">Ресурс **FolderView** предоставляет или задает рекомендации для пользовательского интерфейса папки.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="e0dfb-106">Он доступен в свойстве [folder][folder-facet] ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="e0dfb-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0dfb-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0dfb-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="e0dfb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0dfb-108">Properties</span></span>

| <span data-ttu-id="e0dfb-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e0dfb-109">Property name</span></span>         | <span data-ttu-id="e0dfb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0dfb-110">Type</span></span>   | <span data-ttu-id="e0dfb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0dfb-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="e0dfb-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="e0dfb-112">**sortBy**</span></span>            | <span data-ttu-id="e0dfb-113">строка</span><span class="sxs-lookup"><span data-stu-id="e0dfb-113">string</span></span> | <span data-ttu-id="e0dfb-114">Метод сортировки содержимого папки.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="e0dfb-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="e0dfb-115">**sortOrder**</span></span>         | <span data-ttu-id="e0dfb-116">строка</span><span class="sxs-lookup"><span data-stu-id="e0dfb-116">string</span></span> | <span data-ttu-id="e0dfb-117">Если значение равно true, то необходимо отсортировать элементы по убыванию.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="e0dfb-118">В противном случае необходимо отсортировать элементы по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="e0dfb-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="e0dfb-119">**viewType**</span></span>          | <span data-ttu-id="e0dfb-120">строка</span><span class="sxs-lookup"><span data-stu-id="e0dfb-120">string</span></span> | <span data-ttu-id="e0dfb-121">Тип представления, который следует использовать для представления папки.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="e0dfb-122">Вы можете использовать свойство _sortBy_ для управления порядком сортировки элементов в приложениях, использующих аспект **viewType**.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="e0dfb-123">Значения свойства sortBy</span><span class="sxs-lookup"><span data-stu-id="e0dfb-123">sortBy values</span></span>

<span data-ttu-id="e0dfb-124">Для свойства **sortBy** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="e0dfb-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e0dfb-125">Value</span></span>                    | <span data-ttu-id="e0dfb-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e0dfb-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="e0dfb-127">Порядок сортировки, используемый по умолчанию, в приложении.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="e0dfb-128">Элементы следует упорядочить по их свойству **name**.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="e0dfb-129">Элементы следует упорядочить по их типам.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="e0dfb-130">Элементы следует упорядочить по их свойству **size**.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="e0dfb-131">Элементы следует упорядочить по свойству **takenDateTime** аспекта **photo**.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="e0dfb-132">Если это свойство недоступно, следует использовать свойство **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="e0dfb-133">Элементы следует упорядочить по их свойству **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="e0dfb-134">Для элементов используется настраиваемая последовательность, указанная пользователем.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="e0dfb-135">Значения свойства sortOrder</span><span class="sxs-lookup"><span data-stu-id="e0dfb-135">sortOrder values</span></span>

<span data-ttu-id="e0dfb-136">Для свойства **sortOrder** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="e0dfb-137">Значение</span><span class="sxs-lookup"><span data-stu-id="e0dfb-137">Value</span></span>        | <span data-ttu-id="e0dfb-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e0dfb-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="e0dfb-139">Элементы следует упорядочить по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="e0dfb-140">Элементы следует упорядочить по убыванию.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="e0dfb-141">Значения свойства viewType</span><span class="sxs-lookup"><span data-stu-id="e0dfb-141">viewType values</span></span>

<span data-ttu-id="e0dfb-142">Для свойства **viewType** определены указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="e0dfb-143">Значение</span><span class="sxs-lookup"><span data-stu-id="e0dfb-143">Value</span></span>        | <span data-ttu-id="e0dfb-144">Описание</span><span class="sxs-lookup"><span data-stu-id="e0dfb-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="e0dfb-145">Тип представления, используемый по умолчанию, для приложения.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="e0dfb-146">Представление, в котором для представления элементов driveItems используются значки.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="e0dfb-147">Представление с несколькими столбцами, в которых указаны дополнительные сведения о каждом элементе.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="e0dfb-148">Представление, в котором для представления элементов используются большие эскизы элементов driveItems.</span><span class="sxs-lookup"><span data-stu-id="e0dfb-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
