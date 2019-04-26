---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: bcb68f94574512fd7e952db036a86f242652851d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339865"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="f8c19-102">Тип ресурса ItemActivity</span><span class="sxs-lookup"><span data-stu-id="f8c19-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c19-103">Ресурс **ItemActivity** предоставляет сведения о действиях, выполненных с элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="f8c19-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="f8c19-104">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f8c19-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8c19-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8c19-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f8c19-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8c19-106">Properties</span></span>

| <span data-ttu-id="f8c19-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8c19-107">Property</span></span> | <span data-ttu-id="f8c19-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f8c19-108">Type</span></span>                    | <span data-ttu-id="f8c19-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f8c19-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="f8c19-110">id</span><span class="sxs-lookup"><span data-stu-id="f8c19-110">id</span></span>       | <span data-ttu-id="f8c19-111">string</span><span class="sxs-lookup"><span data-stu-id="f8c19-111">string</span></span>                  | <span data-ttu-id="f8c19-112">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="f8c19-112">The unique identifier of the activity.</span></span> <span data-ttu-id="f8c19-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f8c19-113">Read-only.</span></span>
| <span data-ttu-id="f8c19-114">обращения</span><span class="sxs-lookup"><span data-stu-id="f8c19-114">access</span></span>   | <span data-ttu-id="f8c19-115">[Акцессактион][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-115">[accessAction][]</span></span>        | <span data-ttu-id="f8c19-116">Доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="f8c19-116">An item was accessed.</span></span>
| <span data-ttu-id="f8c19-117">action</span><span class="sxs-lookup"><span data-stu-id="f8c19-117">action</span></span>   | <span data-ttu-id="f8c19-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-118">[itemActionSet][]</span></span>       | <span data-ttu-id="f8c19-119">Сведения о выполненном действии.</span><span class="sxs-lookup"><span data-stu-id="f8c19-119">Details about the action that took place.</span></span> <span data-ttu-id="f8c19-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f8c19-120">Read-only.</span></span>
| <span data-ttu-id="f8c19-121">actor</span><span class="sxs-lookup"><span data-stu-id="f8c19-121">actor</span></span>    | <span data-ttu-id="f8c19-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-122">[identitySet][]</span></span>         | <span data-ttu-id="f8c19-123">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="f8c19-123">Identity of who performed the action.</span></span> <span data-ttu-id="f8c19-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f8c19-124">Read-only.</span></span>
| <span data-ttu-id="f8c19-125">location</span><span class="sxs-lookup"><span data-stu-id="f8c19-125">location</span></span> | <span data-ttu-id="f8c19-126">[location][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-126">[location][]</span></span>            | <span data-ttu-id="f8c19-127">Физическое расположение, в котором было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="f8c19-127">Physical location where the action was performed.</span></span> <span data-ttu-id="f8c19-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f8c19-128">Read-only.</span></span>
| <span data-ttu-id="f8c19-129">times</span><span class="sxs-lookup"><span data-stu-id="f8c19-129">times</span></span>    | <span data-ttu-id="f8c19-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="f8c19-131">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="f8c19-131">Details about when the activity took place.</span></span> <span data-ttu-id="f8c19-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f8c19-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="f8c19-136">Связи</span><span class="sxs-lookup"><span data-stu-id="f8c19-136">Relationships</span></span>

| <span data-ttu-id="f8c19-137">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f8c19-137">Relationship name</span></span> | <span data-ttu-id="f8c19-138">Тип</span><span class="sxs-lookup"><span data-stu-id="f8c19-138">Type</span></span>          | <span data-ttu-id="f8c19-139">Описание</span><span class="sxs-lookup"><span data-stu-id="f8c19-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="f8c19-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="f8c19-140">driveItem</span></span>         | <span data-ttu-id="f8c19-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-141">[driveItem][]</span></span> | <span data-ttu-id="f8c19-142">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="f8c19-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="f8c19-143">listItem</span><span class="sxs-lookup"><span data-stu-id="f8c19-143">listItem</span></span>          | <span data-ttu-id="f8c19-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-144">[listItem][]</span></span>  | <span data-ttu-id="f8c19-145">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="f8c19-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="f8c19-148">Действия</span><span class="sxs-lookup"><span data-stu-id="f8c19-148">Actions</span></span>

<span data-ttu-id="f8c19-149">Операции, выполненные в ходе действия, описываются в свойстве **action**.</span><span class="sxs-lookup"><span data-stu-id="f8c19-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="f8c19-150">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="f8c19-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="f8c19-151">В будущем можно будет вносить в журнал новые действия, поэтому убедитесь, что ваше приложение позволяет обрабатывать объект **itemActivity** без каких-либо действий, которые "понимает" ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="f8c19-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="f8c19-152">Название действия</span><span class="sxs-lookup"><span data-stu-id="f8c19-152">Action name</span></span> | <span data-ttu-id="f8c19-153">Тип</span><span class="sxs-lookup"><span data-stu-id="f8c19-153">Type</span></span>              | <span data-ttu-id="f8c19-154">Описание</span><span class="sxs-lookup"><span data-stu-id="f8c19-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="f8c19-155">comment</span><span class="sxs-lookup"><span data-stu-id="f8c19-155">comment</span></span>     | <span data-ttu-id="f8c19-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-156">[commentAction][]</span></span> | <span data-ttu-id="f8c19-157">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="f8c19-157">A comment was added to the item.</span></span>
| <span data-ttu-id="f8c19-158">create</span><span class="sxs-lookup"><span data-stu-id="f8c19-158">create</span></span>      | <span data-ttu-id="f8c19-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-159">[createAction][]</span></span>  | <span data-ttu-id="f8c19-160">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="f8c19-160">An item was created.</span></span>
| <span data-ttu-id="f8c19-161">delete</span><span class="sxs-lookup"><span data-stu-id="f8c19-161">delete</span></span>      | <span data-ttu-id="f8c19-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-162">[deleteAction][]</span></span>  | <span data-ttu-id="f8c19-163">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="f8c19-163">An item was deleted.</span></span>
| <span data-ttu-id="f8c19-164">edit</span><span class="sxs-lookup"><span data-stu-id="f8c19-164">edit</span></span>        | <span data-ttu-id="f8c19-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-165">[editAction][]</span></span>    | <span data-ttu-id="f8c19-166">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="f8c19-166">An item was edited.</span></span>
| <span data-ttu-id="f8c19-167">mention</span><span class="sxs-lookup"><span data-stu-id="f8c19-167">mention</span></span>     | <span data-ttu-id="f8c19-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-168">[mentionAction][]</span></span> | <span data-ttu-id="f8c19-169">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="f8c19-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="f8c19-170">move</span><span class="sxs-lookup"><span data-stu-id="f8c19-170">move</span></span>        | <span data-ttu-id="f8c19-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-171">[moveAction][]</span></span>    | <span data-ttu-id="f8c19-172">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="f8c19-172">An item was moved.</span></span>
| <span data-ttu-id="f8c19-173">rename</span><span class="sxs-lookup"><span data-stu-id="f8c19-173">rename</span></span>      | <span data-ttu-id="f8c19-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-174">[renameAction][]</span></span>  | <span data-ttu-id="f8c19-175">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="f8c19-175">An item was renamed.</span></span>
| <span data-ttu-id="f8c19-176">restore</span><span class="sxs-lookup"><span data-stu-id="f8c19-176">restore</span></span>     | <span data-ttu-id="f8c19-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-177">[restoreAction][]</span></span> | <span data-ttu-id="f8c19-178">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="f8c19-178">An item was restored.</span></span>
| <span data-ttu-id="f8c19-179">share</span><span class="sxs-lookup"><span data-stu-id="f8c19-179">share</span></span>       | <span data-ttu-id="f8c19-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-180">[shareAction][]</span></span>   | <span data-ttu-id="f8c19-181">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="f8c19-181">An item was shared.</span></span>
| <span data-ttu-id="f8c19-182">version</span><span class="sxs-lookup"><span data-stu-id="f8c19-182">version</span></span>     | <span data-ttu-id="f8c19-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="f8c19-183">[versionAction][]</span></span> | <span data-ttu-id="f8c19-184">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="f8c19-184">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="f8c19-197">Замечания</span><span class="sxs-lookup"><span data-stu-id="f8c19-197">Remarks</span></span>

<span data-ttu-id="f8c19-198">В настоящее время ресурс **ItemActivity** доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f8c19-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

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
