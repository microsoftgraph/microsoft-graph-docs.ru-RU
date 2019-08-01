---
author: daspek
ms.author: dspektor
title: Тип ресурса ItemActionSet
description: Объект itemActionSet предоставляет сведения о действиях, выполняемых в рамках действия с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a28a3380761e2d1914d7c088e5927fc5d3addd4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036724"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="b0d50-103">Тип ресурса itemActionSet</span><span class="sxs-lookup"><span data-stu-id="b0d50-103">itemActionSet resource type</span></span>

<span data-ttu-id="b0d50-104">Ресурс **itemActionSet** предоставляет сведения о действиях, которые составляют [действие][itemActivity] для элемента.</span><span class="sxs-lookup"><span data-stu-id="b0d50-104">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="b0d50-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b0d50-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b0d50-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0d50-106">Properties</span></span>

<span data-ttu-id="b0d50-107">В настоящее время доступны следующие действия.</span><span class="sxs-lookup"><span data-stu-id="b0d50-107">The following actions are currently available.</span></span> <span data-ttu-id="b0d50-108">Так как новые действия могут быть добавлены в будущем, убедитесь, что ваше приложение может обрабатывать **itemActionSet** , который включает неизвестные действия.</span><span class="sxs-lookup"><span data-stu-id="b0d50-108">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="b0d50-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b0d50-109">Property name</span></span> | <span data-ttu-id="b0d50-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b0d50-110">Type</span></span>              | <span data-ttu-id="b0d50-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0d50-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="b0d50-112">comment</span><span class="sxs-lookup"><span data-stu-id="b0d50-112">comment</span></span>       | <span data-ttu-id="b0d50-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-113">[commentAction][]</span></span> | <span data-ttu-id="b0d50-114">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="b0d50-114">A comment was added to the item.</span></span>
| <span data-ttu-id="b0d50-115">create</span><span class="sxs-lookup"><span data-stu-id="b0d50-115">create</span></span>        | <span data-ttu-id="b0d50-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-116">[createAction][]</span></span>  | <span data-ttu-id="b0d50-117">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="b0d50-117">An item was created.</span></span>
| <span data-ttu-id="b0d50-118">delete</span><span class="sxs-lookup"><span data-stu-id="b0d50-118">delete</span></span>        | <span data-ttu-id="b0d50-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-119">[deleteAction][]</span></span>  | <span data-ttu-id="b0d50-120">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="b0d50-120">An item was deleted.</span></span>
| <span data-ttu-id="b0d50-121">edit</span><span class="sxs-lookup"><span data-stu-id="b0d50-121">edit</span></span>          | <span data-ttu-id="b0d50-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-122">[editAction][]</span></span>    | <span data-ttu-id="b0d50-123">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="b0d50-123">An item was edited.</span></span>
| <span data-ttu-id="b0d50-124">mention</span><span class="sxs-lookup"><span data-stu-id="b0d50-124">mention</span></span>       | <span data-ttu-id="b0d50-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-125">[mentionAction][]</span></span> | <span data-ttu-id="b0d50-126">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="b0d50-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="b0d50-127">move</span><span class="sxs-lookup"><span data-stu-id="b0d50-127">move</span></span>          | <span data-ttu-id="b0d50-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-128">[moveAction][]</span></span>    | <span data-ttu-id="b0d50-129">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="b0d50-129">An item was moved.</span></span>
| <span data-ttu-id="b0d50-130">rename</span><span class="sxs-lookup"><span data-stu-id="b0d50-130">rename</span></span>        | <span data-ttu-id="b0d50-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-131">[renameAction][]</span></span>  | <span data-ttu-id="b0d50-132">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="b0d50-132">An item was renamed.</span></span>
| <span data-ttu-id="b0d50-133">restore</span><span class="sxs-lookup"><span data-stu-id="b0d50-133">restore</span></span>       | <span data-ttu-id="b0d50-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-134">[restoreAction][]</span></span> | <span data-ttu-id="b0d50-135">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="b0d50-135">An item was restored.</span></span>
| <span data-ttu-id="b0d50-136">share</span><span class="sxs-lookup"><span data-stu-id="b0d50-136">share</span></span>         | <span data-ttu-id="b0d50-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-137">[shareAction][]</span></span>   | <span data-ttu-id="b0d50-138">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="b0d50-138">An item was shared.</span></span>
| <span data-ttu-id="b0d50-139">version</span><span class="sxs-lookup"><span data-stu-id="b0d50-139">version</span></span>       | <span data-ttu-id="b0d50-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="b0d50-140">[versionAction][]</span></span> | <span data-ttu-id="b0d50-141">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="b0d50-141">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="b0d50-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0d50-152">JSON representation</span></span>

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
