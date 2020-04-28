---
author: daspek
description: Ресурс ItemActionSet предоставляет сведения о действиях, выполненных [Activity] [itemActivity] элемента.
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b3b803b719ad14fabf19574a55360009c3dda14e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523137"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="bc82d-103">Тип ресурса ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="bc82d-103">ItemActionSet resource type</span></span>

<span data-ttu-id="bc82d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc82d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc82d-105">Ресурс **ItemActionSet** содержит сведения о действиях, входящих в состав [операции][itemActivity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="bc82d-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="bc82d-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc82d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc82d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc82d-107">Properties</span></span>

<span data-ttu-id="bc82d-108">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="bc82d-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="bc82d-109">В будущем можно будет вносить в журнал новые действия, поэтому ваше приложение должно быть способно обрабатывать объект **itemActionSet**, содержащий действия, не предусмотренные в приложении.</span><span class="sxs-lookup"><span data-stu-id="bc82d-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="bc82d-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bc82d-110">Property name</span></span> | <span data-ttu-id="bc82d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bc82d-111">Type</span></span>              | <span data-ttu-id="bc82d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bc82d-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="bc82d-113">comment</span><span class="sxs-lookup"><span data-stu-id="bc82d-113">comment</span></span>       | <span data-ttu-id="bc82d-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-114">[commentAction][]</span></span> | <span data-ttu-id="bc82d-115">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="bc82d-115">A comment was added to the item.</span></span>
| <span data-ttu-id="bc82d-116">create</span><span class="sxs-lookup"><span data-stu-id="bc82d-116">create</span></span>        | <span data-ttu-id="bc82d-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-117">[createAction][]</span></span>  | <span data-ttu-id="bc82d-118">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="bc82d-118">An item was created.</span></span>
| <span data-ttu-id="bc82d-119">delete</span><span class="sxs-lookup"><span data-stu-id="bc82d-119">delete</span></span>        | <span data-ttu-id="bc82d-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-120">[deleteAction][]</span></span>  | <span data-ttu-id="bc82d-121">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="bc82d-121">An item was deleted.</span></span>
| <span data-ttu-id="bc82d-122">edit</span><span class="sxs-lookup"><span data-stu-id="bc82d-122">edit</span></span>          | <span data-ttu-id="bc82d-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-123">[editAction][]</span></span>    | <span data-ttu-id="bc82d-124">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="bc82d-124">An item was edited.</span></span>
| <span data-ttu-id="bc82d-125">mention</span><span class="sxs-lookup"><span data-stu-id="bc82d-125">mention</span></span>       | <span data-ttu-id="bc82d-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-126">[mentionAction][]</span></span> | <span data-ttu-id="bc82d-127">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="bc82d-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="bc82d-128">move</span><span class="sxs-lookup"><span data-stu-id="bc82d-128">move</span></span>          | <span data-ttu-id="bc82d-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-129">[moveAction][]</span></span>    | <span data-ttu-id="bc82d-130">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="bc82d-130">An item was moved.</span></span>
| <span data-ttu-id="bc82d-131">rename</span><span class="sxs-lookup"><span data-stu-id="bc82d-131">rename</span></span>        | <span data-ttu-id="bc82d-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-132">[renameAction][]</span></span>  | <span data-ttu-id="bc82d-133">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="bc82d-133">An item was renamed.</span></span>
| <span data-ttu-id="bc82d-134">restore</span><span class="sxs-lookup"><span data-stu-id="bc82d-134">restore</span></span>       | <span data-ttu-id="bc82d-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-135">[restoreAction][]</span></span> | <span data-ttu-id="bc82d-136">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="bc82d-136">An item was restored.</span></span>
| <span data-ttu-id="bc82d-137">share</span><span class="sxs-lookup"><span data-stu-id="bc82d-137">share</span></span>         | <span data-ttu-id="bc82d-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-138">[shareAction][]</span></span>   | <span data-ttu-id="bc82d-139">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="bc82d-139">An item was shared.</span></span>
| <span data-ttu-id="bc82d-140">version</span><span class="sxs-lookup"><span data-stu-id="bc82d-140">version</span></span>       | <span data-ttu-id="bc82d-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="bc82d-141">[versionAction][]</span></span> | <span data-ttu-id="bc82d-142">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="bc82d-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="bc82d-153">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc82d-153">Remarks</span></span>

<span data-ttu-id="bc82d-154">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bc82d-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
