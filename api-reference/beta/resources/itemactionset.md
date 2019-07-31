---
author: daspek
description: Ресурс ItemActionSet предоставляет сведения о действиях, выполненных [Activity] [itemActivity] элемента.
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8053942fe96011b018e46681d69d308f65aa5d5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967149"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="84370-103">Тип ресурса ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="84370-103">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84370-104">Ресурс **ItemActionSet** содержит сведения о действиях, входящих в состав [операции][itemActivity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="84370-104">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="84370-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84370-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

## <a name="properties"></a><span data-ttu-id="84370-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="84370-106">Properties</span></span>

<span data-ttu-id="84370-107">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="84370-107">Below are the actions that are available today.</span></span>
<span data-ttu-id="84370-108">В будущем можно будет вносить в журнал новые действия, поэтому ваше приложение должно быть способно обрабатывать объект **itemActionSet**, содержащий действия, не предусмотренные в приложении.</span><span class="sxs-lookup"><span data-stu-id="84370-108">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="84370-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="84370-109">Property name</span></span> | <span data-ttu-id="84370-110">Тип</span><span class="sxs-lookup"><span data-stu-id="84370-110">Type</span></span>              | <span data-ttu-id="84370-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84370-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="84370-112">comment</span><span class="sxs-lookup"><span data-stu-id="84370-112">comment</span></span>       | <span data-ttu-id="84370-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-113">[commentAction][]</span></span> | <span data-ttu-id="84370-114">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="84370-114">A comment was added to the item.</span></span>
| <span data-ttu-id="84370-115">create</span><span class="sxs-lookup"><span data-stu-id="84370-115">create</span></span>        | <span data-ttu-id="84370-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-116">[createAction][]</span></span>  | <span data-ttu-id="84370-117">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="84370-117">An item was created.</span></span>
| <span data-ttu-id="84370-118">delete</span><span class="sxs-lookup"><span data-stu-id="84370-118">delete</span></span>        | <span data-ttu-id="84370-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-119">[deleteAction][]</span></span>  | <span data-ttu-id="84370-120">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="84370-120">An item was deleted.</span></span>
| <span data-ttu-id="84370-121">edit</span><span class="sxs-lookup"><span data-stu-id="84370-121">edit</span></span>          | <span data-ttu-id="84370-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-122">[editAction][]</span></span>    | <span data-ttu-id="84370-123">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="84370-123">An item was edited.</span></span>
| <span data-ttu-id="84370-124">mention</span><span class="sxs-lookup"><span data-stu-id="84370-124">mention</span></span>       | <span data-ttu-id="84370-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-125">[mentionAction][]</span></span> | <span data-ttu-id="84370-126">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="84370-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="84370-127">move</span><span class="sxs-lookup"><span data-stu-id="84370-127">move</span></span>          | <span data-ttu-id="84370-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-128">[moveAction][]</span></span>    | <span data-ttu-id="84370-129">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="84370-129">An item was moved.</span></span>
| <span data-ttu-id="84370-130">rename</span><span class="sxs-lookup"><span data-stu-id="84370-130">rename</span></span>        | <span data-ttu-id="84370-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-131">[renameAction][]</span></span>  | <span data-ttu-id="84370-132">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="84370-132">An item was renamed.</span></span>
| <span data-ttu-id="84370-133">restore</span><span class="sxs-lookup"><span data-stu-id="84370-133">restore</span></span>       | <span data-ttu-id="84370-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-134">[restoreAction][]</span></span> | <span data-ttu-id="84370-135">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="84370-135">An item was restored.</span></span>
| <span data-ttu-id="84370-136">share</span><span class="sxs-lookup"><span data-stu-id="84370-136">share</span></span>         | <span data-ttu-id="84370-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-137">[shareAction][]</span></span>   | <span data-ttu-id="84370-138">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="84370-138">An item was shared.</span></span>
| <span data-ttu-id="84370-139">version</span><span class="sxs-lookup"><span data-stu-id="84370-139">version</span></span>       | <span data-ttu-id="84370-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="84370-140">[versionAction][]</span></span> | <span data-ttu-id="84370-141">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="84370-141">An item was versioned.</span></span>

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="84370-152">Замечания</span><span class="sxs-lookup"><span data-stu-id="84370-152">Remarks</span></span>

<span data-ttu-id="84370-153">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="84370-153">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
