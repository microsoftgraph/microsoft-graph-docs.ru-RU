---
author: daspek
description: Ресурс ItemActivity предоставляет сведения о действиях, выполненных с элементом или в контейнере.
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab96c3169a2d2dc37e6b94ab325866e93fa4d6c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967105"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="c426c-103">Тип ресурса ItemActivity</span><span class="sxs-lookup"><span data-stu-id="c426c-103">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c426c-104">Ресурс **ItemActivity** предоставляет сведения о действиях, выполненных с элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="c426c-104">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="c426c-105">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c426c-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c426c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c426c-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a><span data-ttu-id="c426c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c426c-107">Properties</span></span>

| <span data-ttu-id="c426c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c426c-108">Property</span></span> | <span data-ttu-id="c426c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c426c-109">Type</span></span>                    | <span data-ttu-id="c426c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c426c-110">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="c426c-111">id</span><span class="sxs-lookup"><span data-stu-id="c426c-111">id</span></span>       | <span data-ttu-id="c426c-112">string</span><span class="sxs-lookup"><span data-stu-id="c426c-112">string</span></span>                  | <span data-ttu-id="c426c-113">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="c426c-113">The unique identifier of the activity.</span></span> <span data-ttu-id="c426c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c426c-114">Read-only.</span></span>
| <span data-ttu-id="c426c-115">обращения</span><span class="sxs-lookup"><span data-stu-id="c426c-115">access</span></span>   | <span data-ttu-id="c426c-116">[Акцессактион][]</span><span class="sxs-lookup"><span data-stu-id="c426c-116">[accessAction][]</span></span>        | <span data-ttu-id="c426c-117">Доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="c426c-117">An item was accessed.</span></span>
| <span data-ttu-id="c426c-118">action</span><span class="sxs-lookup"><span data-stu-id="c426c-118">action</span></span>   | <span data-ttu-id="c426c-119">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="c426c-119">[itemActionSet][]</span></span>       | <span data-ttu-id="c426c-120">Сведения о выполненном действии.</span><span class="sxs-lookup"><span data-stu-id="c426c-120">Details about the action that took place.</span></span> <span data-ttu-id="c426c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c426c-121">Read-only.</span></span>
| <span data-ttu-id="c426c-122">actor</span><span class="sxs-lookup"><span data-stu-id="c426c-122">actor</span></span>    | <span data-ttu-id="c426c-123">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c426c-123">[identitySet][]</span></span>         | <span data-ttu-id="c426c-124">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="c426c-124">Identity of who performed the action.</span></span> <span data-ttu-id="c426c-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c426c-125">Read-only.</span></span>
| <span data-ttu-id="c426c-126">location</span><span class="sxs-lookup"><span data-stu-id="c426c-126">location</span></span> | <span data-ttu-id="c426c-127">[location][]</span><span class="sxs-lookup"><span data-stu-id="c426c-127">[location][]</span></span>            | <span data-ttu-id="c426c-128">Физическое расположение, в котором было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="c426c-128">Physical location where the action was performed.</span></span> <span data-ttu-id="c426c-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c426c-129">Read-only.</span></span>
| <span data-ttu-id="c426c-130">times</span><span class="sxs-lookup"><span data-stu-id="c426c-130">times</span></span>    | <span data-ttu-id="c426c-131">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="c426c-131">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="c426c-132">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="c426c-132">Details about when the activity took place.</span></span> <span data-ttu-id="c426c-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c426c-133">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="c426c-137">Связи</span><span class="sxs-lookup"><span data-stu-id="c426c-137">Relationships</span></span>

| <span data-ttu-id="c426c-138">Имя связи</span><span class="sxs-lookup"><span data-stu-id="c426c-138">Relationship name</span></span> | <span data-ttu-id="c426c-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c426c-139">Type</span></span>          | <span data-ttu-id="c426c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c426c-140">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="c426c-141">driveItem</span><span class="sxs-lookup"><span data-stu-id="c426c-141">driveItem</span></span>         | <span data-ttu-id="c426c-142">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c426c-142">[driveItem][]</span></span> | <span data-ttu-id="c426c-143">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="c426c-143">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="c426c-144">listItem</span><span class="sxs-lookup"><span data-stu-id="c426c-144">listItem</span></span>          | <span data-ttu-id="c426c-145">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="c426c-145">[listItem][]</span></span>  | <span data-ttu-id="c426c-146">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="c426c-146">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="c426c-149">Действия</span><span class="sxs-lookup"><span data-stu-id="c426c-149">Actions</span></span>

<span data-ttu-id="c426c-150">Операции, выполненные в ходе действия, описываются в свойстве **action**.</span><span class="sxs-lookup"><span data-stu-id="c426c-150">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="c426c-151">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="c426c-151">Below are the actions that are available today.</span></span>
<span data-ttu-id="c426c-152">В будущем можно будет вносить в журнал новые действия, поэтому убедитесь, что ваше приложение позволяет обрабатывать объект **itemActivity** без каких-либо действий, которые "понимает" ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="c426c-152">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="c426c-153">Название действия</span><span class="sxs-lookup"><span data-stu-id="c426c-153">Action name</span></span> | <span data-ttu-id="c426c-154">Тип</span><span class="sxs-lookup"><span data-stu-id="c426c-154">Type</span></span>              | <span data-ttu-id="c426c-155">Описание</span><span class="sxs-lookup"><span data-stu-id="c426c-155">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="c426c-156">comment</span><span class="sxs-lookup"><span data-stu-id="c426c-156">comment</span></span>     | <span data-ttu-id="c426c-157">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-157">[commentAction][]</span></span> | <span data-ttu-id="c426c-158">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="c426c-158">A comment was added to the item.</span></span>
| <span data-ttu-id="c426c-159">create</span><span class="sxs-lookup"><span data-stu-id="c426c-159">create</span></span>      | <span data-ttu-id="c426c-160">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-160">[createAction][]</span></span>  | <span data-ttu-id="c426c-161">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="c426c-161">An item was created.</span></span>
| <span data-ttu-id="c426c-162">delete</span><span class="sxs-lookup"><span data-stu-id="c426c-162">delete</span></span>      | <span data-ttu-id="c426c-163">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-163">[deleteAction][]</span></span>  | <span data-ttu-id="c426c-164">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="c426c-164">An item was deleted.</span></span>
| <span data-ttu-id="c426c-165">edit</span><span class="sxs-lookup"><span data-stu-id="c426c-165">edit</span></span>        | <span data-ttu-id="c426c-166">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-166">[editAction][]</span></span>    | <span data-ttu-id="c426c-167">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="c426c-167">An item was edited.</span></span>
| <span data-ttu-id="c426c-168">mention</span><span class="sxs-lookup"><span data-stu-id="c426c-168">mention</span></span>     | <span data-ttu-id="c426c-169">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-169">[mentionAction][]</span></span> | <span data-ttu-id="c426c-170">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="c426c-170">A user was mentioned in the item.</span></span>
| <span data-ttu-id="c426c-171">move</span><span class="sxs-lookup"><span data-stu-id="c426c-171">move</span></span>        | <span data-ttu-id="c426c-172">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-172">[moveAction][]</span></span>    | <span data-ttu-id="c426c-173">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="c426c-173">An item was moved.</span></span>
| <span data-ttu-id="c426c-174">rename</span><span class="sxs-lookup"><span data-stu-id="c426c-174">rename</span></span>      | <span data-ttu-id="c426c-175">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-175">[renameAction][]</span></span>  | <span data-ttu-id="c426c-176">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="c426c-176">An item was renamed.</span></span>
| <span data-ttu-id="c426c-177">restore</span><span class="sxs-lookup"><span data-stu-id="c426c-177">restore</span></span>     | <span data-ttu-id="c426c-178">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-178">[restoreAction][]</span></span> | <span data-ttu-id="c426c-179">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="c426c-179">An item was restored.</span></span>
| <span data-ttu-id="c426c-180">share</span><span class="sxs-lookup"><span data-stu-id="c426c-180">share</span></span>       | <span data-ttu-id="c426c-181">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-181">[shareAction][]</span></span>   | <span data-ttu-id="c426c-182">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="c426c-182">An item was shared.</span></span>
| <span data-ttu-id="c426c-183">version</span><span class="sxs-lookup"><span data-stu-id="c426c-183">version</span></span>     | <span data-ttu-id="c426c-184">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="c426c-184">[versionAction][]</span></span> | <span data-ttu-id="c426c-185">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="c426c-185">An item was versioned.</span></span>

[Акцессактион]: accessaction.md
[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="c426c-198">Замечания</span><span class="sxs-lookup"><span data-stu-id="c426c-198">Remarks</span></span>

<span data-ttu-id="c426c-199">В настоящее время ресурс **ItemActivity** доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c426c-199">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
