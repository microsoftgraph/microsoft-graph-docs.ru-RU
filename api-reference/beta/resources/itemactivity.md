---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemActivity
localization_priority: Normal
ms.openlocfilehash: 5e2be549c3e3e9e799449679b605577ecd782a94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517297"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="27d38-102">Тип ресурса ItemActivity</span><span class="sxs-lookup"><span data-stu-id="27d38-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d38-103">Ресурс **ItemActivity** предоставляет сведения о действиях, выполненных с элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="27d38-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="27d38-104">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="27d38-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27d38-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27d38-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="27d38-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="27d38-106">Properties</span></span>

| <span data-ttu-id="27d38-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="27d38-107">Property</span></span> | <span data-ttu-id="27d38-108">Тип</span><span class="sxs-lookup"><span data-stu-id="27d38-108">Type</span></span>                    | <span data-ttu-id="27d38-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27d38-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="27d38-110">id</span><span class="sxs-lookup"><span data-stu-id="27d38-110">id</span></span>       | <span data-ttu-id="27d38-111">string</span><span class="sxs-lookup"><span data-stu-id="27d38-111">string</span></span>                  | <span data-ttu-id="27d38-112">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="27d38-112">The unique identifier of the activity.</span></span> <span data-ttu-id="27d38-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27d38-113">Read-only.</span></span>
| <span data-ttu-id="27d38-114">Access</span><span class="sxs-lookup"><span data-stu-id="27d38-114">access</span></span>   | <span data-ttu-id="27d38-115">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-115">[accessAction][]</span></span>        | <span data-ttu-id="27d38-116">Обращения к элемента.</span><span class="sxs-lookup"><span data-stu-id="27d38-116">An item was accessed.</span></span>
| <span data-ttu-id="27d38-117">action</span><span class="sxs-lookup"><span data-stu-id="27d38-117">action</span></span>   | <span data-ttu-id="27d38-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="27d38-118">[itemActionSet][]</span></span>       | <span data-ttu-id="27d38-119">Сведения о выполненном действии.</span><span class="sxs-lookup"><span data-stu-id="27d38-119">Details about the action that took place.</span></span> <span data-ttu-id="27d38-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27d38-120">Read-only.</span></span>
| <span data-ttu-id="27d38-121">actor</span><span class="sxs-lookup"><span data-stu-id="27d38-121">actor</span></span>    | <span data-ttu-id="27d38-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="27d38-122">[identitySet][]</span></span>         | <span data-ttu-id="27d38-123">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="27d38-123">Identity of who performed the action.</span></span> <span data-ttu-id="27d38-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27d38-124">Read-only.</span></span>
| <span data-ttu-id="27d38-125">location</span><span class="sxs-lookup"><span data-stu-id="27d38-125">location</span></span> | <span data-ttu-id="27d38-126">[location][]</span><span class="sxs-lookup"><span data-stu-id="27d38-126">[location][]</span></span>            | <span data-ttu-id="27d38-127">Физическое расположение, где было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="27d38-127">Physical location where the action was performed.</span></span> <span data-ttu-id="27d38-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27d38-128">Read-only.</span></span>
| <span data-ttu-id="27d38-129">times</span><span class="sxs-lookup"><span data-stu-id="27d38-129">times</span></span>    | <span data-ttu-id="27d38-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="27d38-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="27d38-131">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="27d38-131">Details about when the activity took place.</span></span> <span data-ttu-id="27d38-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27d38-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="27d38-136">Связи</span><span class="sxs-lookup"><span data-stu-id="27d38-136">Relationships</span></span>

| <span data-ttu-id="27d38-137">Имя связи</span><span class="sxs-lookup"><span data-stu-id="27d38-137">Relationship name</span></span> | <span data-ttu-id="27d38-138">Тип</span><span class="sxs-lookup"><span data-stu-id="27d38-138">Type</span></span>          | <span data-ttu-id="27d38-139">Описание</span><span class="sxs-lookup"><span data-stu-id="27d38-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="27d38-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="27d38-140">driveItem</span></span>         | <span data-ttu-id="27d38-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="27d38-141">[driveItem][]</span></span> | <span data-ttu-id="27d38-142">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="27d38-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="27d38-143">listItem</span><span class="sxs-lookup"><span data-stu-id="27d38-143">listItem</span></span>          | <span data-ttu-id="27d38-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="27d38-144">[listItem][]</span></span>  | <span data-ttu-id="27d38-145">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="27d38-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="27d38-148">Действия</span><span class="sxs-lookup"><span data-stu-id="27d38-148">Actions</span></span>

<span data-ttu-id="27d38-149">Операции, выполненные в ходе действия, описываются в свойстве **action**.</span><span class="sxs-lookup"><span data-stu-id="27d38-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="27d38-150">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="27d38-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="27d38-151">В будущем можно будет вносить в журнал новые действия, поэтому убедитесь, что ваше приложение позволяет обрабатывать объект **itemActivity** без каких-либо действий, которые "понимает" ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="27d38-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="27d38-152">Название действия</span><span class="sxs-lookup"><span data-stu-id="27d38-152">Action name</span></span> | <span data-ttu-id="27d38-153">Тип</span><span class="sxs-lookup"><span data-stu-id="27d38-153">Type</span></span>              | <span data-ttu-id="27d38-154">Описание</span><span class="sxs-lookup"><span data-stu-id="27d38-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="27d38-155">comment</span><span class="sxs-lookup"><span data-stu-id="27d38-155">comment</span></span>     | <span data-ttu-id="27d38-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-156">[commentAction][]</span></span> | <span data-ttu-id="27d38-157">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="27d38-157">A comment was added to the item.</span></span>
| <span data-ttu-id="27d38-158">create</span><span class="sxs-lookup"><span data-stu-id="27d38-158">create</span></span>      | <span data-ttu-id="27d38-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-159">[createAction][]</span></span>  | <span data-ttu-id="27d38-160">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="27d38-160">An item was created.</span></span>
| <span data-ttu-id="27d38-161">delete</span><span class="sxs-lookup"><span data-stu-id="27d38-161">delete</span></span>      | <span data-ttu-id="27d38-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-162">[deleteAction][]</span></span>  | <span data-ttu-id="27d38-163">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="27d38-163">An item was deleted.</span></span>
| <span data-ttu-id="27d38-164">edit</span><span class="sxs-lookup"><span data-stu-id="27d38-164">edit</span></span>        | <span data-ttu-id="27d38-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-165">[editAction][]</span></span>    | <span data-ttu-id="27d38-166">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="27d38-166">An item was edited.</span></span>
| <span data-ttu-id="27d38-167">mention</span><span class="sxs-lookup"><span data-stu-id="27d38-167">mention</span></span>     | <span data-ttu-id="27d38-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-168">[mentionAction][]</span></span> | <span data-ttu-id="27d38-169">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="27d38-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="27d38-170">move</span><span class="sxs-lookup"><span data-stu-id="27d38-170">move</span></span>        | <span data-ttu-id="27d38-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-171">[moveAction][]</span></span>    | <span data-ttu-id="27d38-172">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="27d38-172">An item was moved.</span></span>
| <span data-ttu-id="27d38-173">rename</span><span class="sxs-lookup"><span data-stu-id="27d38-173">rename</span></span>      | <span data-ttu-id="27d38-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-174">[renameAction][]</span></span>  | <span data-ttu-id="27d38-175">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="27d38-175">An item was renamed.</span></span>
| <span data-ttu-id="27d38-176">restore</span><span class="sxs-lookup"><span data-stu-id="27d38-176">restore</span></span>     | <span data-ttu-id="27d38-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-177">[restoreAction][]</span></span> | <span data-ttu-id="27d38-178">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="27d38-178">An item was restored.</span></span>
| <span data-ttu-id="27d38-179">share</span><span class="sxs-lookup"><span data-stu-id="27d38-179">share</span></span>       | <span data-ttu-id="27d38-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-180">[shareAction][]</span></span>   | <span data-ttu-id="27d38-181">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="27d38-181">An item was shared.</span></span>
| <span data-ttu-id="27d38-182">version</span><span class="sxs-lookup"><span data-stu-id="27d38-182">version</span></span>     | <span data-ttu-id="27d38-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="27d38-183">[versionAction][]</span></span> | <span data-ttu-id="27d38-184">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="27d38-184">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="27d38-197">Замечания</span><span class="sxs-lookup"><span data-stu-id="27d38-197">Remarks</span></span>

<span data-ttu-id="27d38-198">В настоящее время ресурс **ItemActivity** доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="27d38-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
