---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: a29bdad0ae5e06d3d1b55f1fb7ceb630bec1b564
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819672"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="87bc1-102">Тип ресурса ItemActivity</span><span class="sxs-lookup"><span data-stu-id="87bc1-102">ItemActivity resource type</span></span>

> <span data-ttu-id="87bc1-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87bc1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87bc1-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bc1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87bc1-105">Ресурс **ItemActivity** предоставляет сведения о действиях, выполненных с элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="87bc1-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="87bc1-106">В настоящее время он доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="87bc1-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87bc1-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="87bc1-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="87bc1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="87bc1-108">Properties</span></span>

| <span data-ttu-id="87bc1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="87bc1-109">Property</span></span> | <span data-ttu-id="87bc1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="87bc1-110">Type</span></span>                    | <span data-ttu-id="87bc1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="87bc1-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="87bc1-112">id</span><span class="sxs-lookup"><span data-stu-id="87bc1-112">id</span></span>       | <span data-ttu-id="87bc1-113">строка</span><span class="sxs-lookup"><span data-stu-id="87bc1-113">string</span></span>                  | <span data-ttu-id="87bc1-114">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="87bc1-114">The unique identifier of the activity.</span></span> <span data-ttu-id="87bc1-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87bc1-115">Read-only.</span></span>
| <span data-ttu-id="87bc1-116">Access</span><span class="sxs-lookup"><span data-stu-id="87bc1-116">access</span></span>   | <span data-ttu-id="87bc1-117">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-117">[accessAction][]</span></span>        | <span data-ttu-id="87bc1-118">Обращения к элемента.</span><span class="sxs-lookup"><span data-stu-id="87bc1-118">An item was accessed.</span></span>
| <span data-ttu-id="87bc1-119">action</span><span class="sxs-lookup"><span data-stu-id="87bc1-119">action</span></span>   | <span data-ttu-id="87bc1-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-120">[itemActionSet][]</span></span>       | <span data-ttu-id="87bc1-121">Сведения о выполненном действии.</span><span class="sxs-lookup"><span data-stu-id="87bc1-121">Details about the action that took place.</span></span> <span data-ttu-id="87bc1-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87bc1-122">Read-only.</span></span>
| <span data-ttu-id="87bc1-123">actor</span><span class="sxs-lookup"><span data-stu-id="87bc1-123">actor</span></span>    | <span data-ttu-id="87bc1-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-124">[identitySet][]</span></span>         | <span data-ttu-id="87bc1-125">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="87bc1-125">Identity of who performed the action.</span></span> <span data-ttu-id="87bc1-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87bc1-126">Read-only.</span></span>
| <span data-ttu-id="87bc1-127">location</span><span class="sxs-lookup"><span data-stu-id="87bc1-127">location</span></span> | <span data-ttu-id="87bc1-128">[location][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-128">[location][]</span></span>            | <span data-ttu-id="87bc1-129">Физическое расположение, где было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="87bc1-129">Physical location where the action was performed.</span></span> <span data-ttu-id="87bc1-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87bc1-130">Read-only.</span></span>
| <span data-ttu-id="87bc1-131">times</span><span class="sxs-lookup"><span data-stu-id="87bc1-131">times</span></span>    | <span data-ttu-id="87bc1-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="87bc1-133">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="87bc1-133">Details about when the activity took place.</span></span> <span data-ttu-id="87bc1-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87bc1-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="87bc1-138">Связи</span><span class="sxs-lookup"><span data-stu-id="87bc1-138">Relationships</span></span>

| <span data-ttu-id="87bc1-139">Имя связи</span><span class="sxs-lookup"><span data-stu-id="87bc1-139">Relationship name</span></span> | <span data-ttu-id="87bc1-140">Тип</span><span class="sxs-lookup"><span data-stu-id="87bc1-140">Type</span></span>          | <span data-ttu-id="87bc1-141">Описание</span><span class="sxs-lookup"><span data-stu-id="87bc1-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="87bc1-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="87bc1-142">driveItem</span></span>         | <span data-ttu-id="87bc1-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-143">[driveItem][]</span></span> | <span data-ttu-id="87bc1-144">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="87bc1-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="87bc1-145">listItem</span><span class="sxs-lookup"><span data-stu-id="87bc1-145">listItem</span></span>          | <span data-ttu-id="87bc1-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-146">[listItem][]</span></span>  | <span data-ttu-id="87bc1-147">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="87bc1-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="87bc1-150">Действия</span><span class="sxs-lookup"><span data-stu-id="87bc1-150">Actions</span></span>

<span data-ttu-id="87bc1-151">Операции, выполненные в ходе действия, описываются в свойстве **action**.</span><span class="sxs-lookup"><span data-stu-id="87bc1-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="87bc1-152">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="87bc1-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="87bc1-153">В будущем можно будет вносить в журнал новые действия, поэтому убедитесь, что ваше приложение позволяет обрабатывать объект **itemActivity** без каких-либо действий, которые "понимает" ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="87bc1-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="87bc1-154">Название действия</span><span class="sxs-lookup"><span data-stu-id="87bc1-154">Action name</span></span> | <span data-ttu-id="87bc1-155">Тип</span><span class="sxs-lookup"><span data-stu-id="87bc1-155">Type</span></span>              | <span data-ttu-id="87bc1-156">Описание</span><span class="sxs-lookup"><span data-stu-id="87bc1-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="87bc1-157">comment</span><span class="sxs-lookup"><span data-stu-id="87bc1-157">comment</span></span>     | <span data-ttu-id="87bc1-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-158">[commentAction][]</span></span> | <span data-ttu-id="87bc1-159">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="87bc1-159">A comment was added to the item.</span></span>
| <span data-ttu-id="87bc1-160">create</span><span class="sxs-lookup"><span data-stu-id="87bc1-160">create</span></span>      | <span data-ttu-id="87bc1-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-161">[createAction][]</span></span>  | <span data-ttu-id="87bc1-162">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="87bc1-162">An item was created.</span></span>
| <span data-ttu-id="87bc1-163">delete</span><span class="sxs-lookup"><span data-stu-id="87bc1-163">delete</span></span>      | <span data-ttu-id="87bc1-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-164">[deleteAction][]</span></span>  | <span data-ttu-id="87bc1-165">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="87bc1-165">An item was deleted.</span></span>
| <span data-ttu-id="87bc1-166">edit</span><span class="sxs-lookup"><span data-stu-id="87bc1-166">edit</span></span>        | <span data-ttu-id="87bc1-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-167">[editAction][]</span></span>    | <span data-ttu-id="87bc1-168">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="87bc1-168">An item was edited.</span></span>
| <span data-ttu-id="87bc1-169">mention</span><span class="sxs-lookup"><span data-stu-id="87bc1-169">mention</span></span>     | <span data-ttu-id="87bc1-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-170">[mentionAction][]</span></span> | <span data-ttu-id="87bc1-171">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="87bc1-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="87bc1-172">move</span><span class="sxs-lookup"><span data-stu-id="87bc1-172">move</span></span>        | <span data-ttu-id="87bc1-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-173">[moveAction][]</span></span>    | <span data-ttu-id="87bc1-174">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="87bc1-174">An item was moved.</span></span>
| <span data-ttu-id="87bc1-175">rename</span><span class="sxs-lookup"><span data-stu-id="87bc1-175">rename</span></span>      | <span data-ttu-id="87bc1-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-176">[renameAction][]</span></span>  | <span data-ttu-id="87bc1-177">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="87bc1-177">An item was renamed.</span></span>
| <span data-ttu-id="87bc1-178">restore</span><span class="sxs-lookup"><span data-stu-id="87bc1-178">restore</span></span>     | <span data-ttu-id="87bc1-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-179">[restoreAction][]</span></span> | <span data-ttu-id="87bc1-180">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="87bc1-180">An item was restored.</span></span>
| <span data-ttu-id="87bc1-181">share</span><span class="sxs-lookup"><span data-stu-id="87bc1-181">share</span></span>       | <span data-ttu-id="87bc1-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-182">[shareAction][]</span></span>   | <span data-ttu-id="87bc1-183">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="87bc1-183">An item was shared.</span></span>
| <span data-ttu-id="87bc1-184">version</span><span class="sxs-lookup"><span data-stu-id="87bc1-184">version</span></span>     | <span data-ttu-id="87bc1-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="87bc1-185">[versionAction][]</span></span> | <span data-ttu-id="87bc1-186">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="87bc1-186">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="87bc1-199">Замечания</span><span class="sxs-lookup"><span data-stu-id="87bc1-199">Remarks</span></span>

<span data-ttu-id="87bc1-200">В настоящее время ресурс **ItemActivity** доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="87bc1-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
