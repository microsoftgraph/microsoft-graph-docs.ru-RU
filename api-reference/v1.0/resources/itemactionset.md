---
author: daspek
ms.author: dspektor
title: Тип ресурса ItemActionSet
description: Объект itemActionSet предоставляет сведения о действиях, выполняемых в рамках действия с элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 065a6126e2e4a2f78cecfb2ae5497fac28e16899
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970799"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="5389c-103">Тип ресурса itemActionSet</span><span class="sxs-lookup"><span data-stu-id="5389c-103">itemActionSet resource type</span></span>

<span data-ttu-id="5389c-104">Ресурс **itemActionSet** предоставляет сведения о действиях, которые составляют [действие] [ itemActivity] для элемента.</span><span class="sxs-lookup"><span data-stu-id="5389c-104">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="5389c-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5389c-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="5389c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5389c-106">Properties</span></span>

<span data-ttu-id="5389c-107">В настоящее время доступны следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5389c-107">The following actions are currently available.</span></span> <span data-ttu-id="5389c-108">Так как новые действия могут быть добавлены в будущем, убедитесь, что ваше приложение может обрабатывать **itemActionSet** , который включает неизвестные действия.</span><span class="sxs-lookup"><span data-stu-id="5389c-108">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="5389c-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5389c-109">Property name</span></span> | <span data-ttu-id="5389c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5389c-110">Type</span></span>              | <span data-ttu-id="5389c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5389c-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="5389c-112">comment</span><span class="sxs-lookup"><span data-stu-id="5389c-112">comment</span></span>       | <span data-ttu-id="5389c-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-113">[commentAction][]</span></span> | <span data-ttu-id="5389c-114">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="5389c-114">A comment was added to the item.</span></span>
| <span data-ttu-id="5389c-115">create</span><span class="sxs-lookup"><span data-stu-id="5389c-115">create</span></span>        | <span data-ttu-id="5389c-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-116">[createAction][]</span></span>  | <span data-ttu-id="5389c-117">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="5389c-117">An item was created.</span></span>
| <span data-ttu-id="5389c-118">delete</span><span class="sxs-lookup"><span data-stu-id="5389c-118">delete</span></span>        | <span data-ttu-id="5389c-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-119">[deleteAction][]</span></span>  | <span data-ttu-id="5389c-120">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="5389c-120">An item was deleted.</span></span>
| <span data-ttu-id="5389c-121">edit</span><span class="sxs-lookup"><span data-stu-id="5389c-121">edit</span></span>          | <span data-ttu-id="5389c-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-122">[editAction][]</span></span>    | <span data-ttu-id="5389c-123">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="5389c-123">An item was edited.</span></span>
| <span data-ttu-id="5389c-124">mention</span><span class="sxs-lookup"><span data-stu-id="5389c-124">mention</span></span>       | <span data-ttu-id="5389c-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-125">[mentionAction][]</span></span> | <span data-ttu-id="5389c-126">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="5389c-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="5389c-127">move</span><span class="sxs-lookup"><span data-stu-id="5389c-127">move</span></span>          | <span data-ttu-id="5389c-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-128">[moveAction][]</span></span>    | <span data-ttu-id="5389c-129">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="5389c-129">An item was moved.</span></span>
| <span data-ttu-id="5389c-130">rename</span><span class="sxs-lookup"><span data-stu-id="5389c-130">rename</span></span>        | <span data-ttu-id="5389c-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-131">[renameAction][]</span></span>  | <span data-ttu-id="5389c-132">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="5389c-132">An item was renamed.</span></span>
| <span data-ttu-id="5389c-133">restore</span><span class="sxs-lookup"><span data-stu-id="5389c-133">restore</span></span>       | <span data-ttu-id="5389c-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-134">[restoreAction][]</span></span> | <span data-ttu-id="5389c-135">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="5389c-135">An item was restored.</span></span>
| <span data-ttu-id="5389c-136">share</span><span class="sxs-lookup"><span data-stu-id="5389c-136">share</span></span>         | <span data-ttu-id="5389c-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-137">[shareAction][]</span></span>   | <span data-ttu-id="5389c-138">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="5389c-138">An item was shared.</span></span>
| <span data-ttu-id="5389c-139">version</span><span class="sxs-lookup"><span data-stu-id="5389c-139">version</span></span>       | <span data-ttu-id="5389c-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="5389c-140">[versionAction][]</span></span> | <span data-ttu-id="5389c-141">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="5389c-141">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="5389c-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5389c-152">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
