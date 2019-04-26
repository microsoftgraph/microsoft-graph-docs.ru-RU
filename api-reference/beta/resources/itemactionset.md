---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: 3fab75c6a63630f57dae8d0578691ba10622231d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569958"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="b5693-102">Тип ресурса ItemActionSet</span><span class="sxs-lookup"><span data-stu-id="b5693-102">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5693-103">Ресурс **ItemActionSet** содержит сведения о действиях, входящих в состав [операции][itemActivity] над элементом.</span><span class="sxs-lookup"><span data-stu-id="b5693-103">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b5693-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5693-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b5693-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5693-105">Properties</span></span>

<span data-ttu-id="b5693-106">Ниже перечислены действия, доступные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="b5693-106">Below are the actions that are available today.</span></span>
<span data-ttu-id="b5693-107">В будущем можно будет вносить в журнал новые действия, поэтому ваше приложение должно быть способно обрабатывать объект **itemActionSet**, содержащий действия, не предусмотренные в приложении.</span><span class="sxs-lookup"><span data-stu-id="b5693-107">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="b5693-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b5693-108">Property name</span></span> | <span data-ttu-id="b5693-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b5693-109">Type</span></span>              | <span data-ttu-id="b5693-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b5693-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="b5693-111">comment</span><span class="sxs-lookup"><span data-stu-id="b5693-111">comment</span></span>       | <span data-ttu-id="b5693-112">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-112">[commentAction][]</span></span> | <span data-ttu-id="b5693-113">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="b5693-113">A comment was added to the item.</span></span>
| <span data-ttu-id="b5693-114">create</span><span class="sxs-lookup"><span data-stu-id="b5693-114">create</span></span>        | <span data-ttu-id="b5693-115">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-115">[createAction][]</span></span>  | <span data-ttu-id="b5693-116">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="b5693-116">An item was created.</span></span>
| <span data-ttu-id="b5693-117">delete</span><span class="sxs-lookup"><span data-stu-id="b5693-117">delete</span></span>        | <span data-ttu-id="b5693-118">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-118">[deleteAction][]</span></span>  | <span data-ttu-id="b5693-119">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="b5693-119">An item was deleted.</span></span>
| <span data-ttu-id="b5693-120">edit</span><span class="sxs-lookup"><span data-stu-id="b5693-120">edit</span></span>          | <span data-ttu-id="b5693-121">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-121">[editAction][]</span></span>    | <span data-ttu-id="b5693-122">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="b5693-122">An item was edited.</span></span>
| <span data-ttu-id="b5693-123">mention</span><span class="sxs-lookup"><span data-stu-id="b5693-123">mention</span></span>       | <span data-ttu-id="b5693-124">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-124">[mentionAction][]</span></span> | <span data-ttu-id="b5693-125">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="b5693-125">A user was mentioned in the item.</span></span>
| <span data-ttu-id="b5693-126">move</span><span class="sxs-lookup"><span data-stu-id="b5693-126">move</span></span>          | <span data-ttu-id="b5693-127">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-127">[moveAction][]</span></span>    | <span data-ttu-id="b5693-128">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="b5693-128">An item was moved.</span></span>
| <span data-ttu-id="b5693-129">rename</span><span class="sxs-lookup"><span data-stu-id="b5693-129">rename</span></span>        | <span data-ttu-id="b5693-130">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-130">[renameAction][]</span></span>  | <span data-ttu-id="b5693-131">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="b5693-131">An item was renamed.</span></span>
| <span data-ttu-id="b5693-132">restore</span><span class="sxs-lookup"><span data-stu-id="b5693-132">restore</span></span>       | <span data-ttu-id="b5693-133">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-133">[restoreAction][]</span></span> | <span data-ttu-id="b5693-134">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="b5693-134">An item was restored.</span></span>
| <span data-ttu-id="b5693-135">share</span><span class="sxs-lookup"><span data-stu-id="b5693-135">share</span></span>         | <span data-ttu-id="b5693-136">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-136">[shareAction][]</span></span>   | <span data-ttu-id="b5693-137">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="b5693-137">An item was shared.</span></span>
| <span data-ttu-id="b5693-138">version</span><span class="sxs-lookup"><span data-stu-id="b5693-138">version</span></span>       | <span data-ttu-id="b5693-139">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="b5693-139">[versionAction][]</span></span> | <span data-ttu-id="b5693-140">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="b5693-140">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b5693-151">Замечания</span><span class="sxs-lookup"><span data-stu-id="b5693-151">Remarks</span></span>

<span data-ttu-id="b5693-152">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b5693-152">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
