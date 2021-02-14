---
author: daspek
title: Тип ресурса ItemActionSet
description: Объект itemActionSet предоставляет сведения о действиях, которые произошли в рамках действия с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 6dcc630b76adcbec3c719a43280e4b28d1d933e5
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239256"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="24e71-103">Тип ресурса itemActionSet</span><span class="sxs-lookup"><span data-stu-id="24e71-103">itemActionSet resource type</span></span>

<span data-ttu-id="24e71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24e71-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24e71-105">Ресурс **itemActionSet** предоставляет сведения о действиях, которые составили [действие][itemActivity] для элемента.</span><span class="sxs-lookup"><span data-stu-id="24e71-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="24e71-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="24e71-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="24e71-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24e71-107">Properties</span></span>

<span data-ttu-id="24e71-108">В настоящее время доступны следующие действия.</span><span class="sxs-lookup"><span data-stu-id="24e71-108">The following actions are currently available.</span></span> <span data-ttu-id="24e71-109">Так как новые действия могут быть добавлены в будущем, убедитесь, что ваше приложение может обрабатывать **объект itemActionSet,** который включает неизвестные действия.</span><span class="sxs-lookup"><span data-stu-id="24e71-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="24e71-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="24e71-110">Property name</span></span> | <span data-ttu-id="24e71-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24e71-111">Type</span></span>              | <span data-ttu-id="24e71-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24e71-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="24e71-113">comment</span><span class="sxs-lookup"><span data-stu-id="24e71-113">comment</span></span>       | <span data-ttu-id="24e71-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-114">[commentAction][]</span></span> | <span data-ttu-id="24e71-115">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="24e71-115">A comment was added to the item.</span></span>
| <span data-ttu-id="24e71-116">create</span><span class="sxs-lookup"><span data-stu-id="24e71-116">create</span></span>        | <span data-ttu-id="24e71-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-117">[createAction][]</span></span>  | <span data-ttu-id="24e71-118">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="24e71-118">An item was created.</span></span>
| <span data-ttu-id="24e71-119">delete</span><span class="sxs-lookup"><span data-stu-id="24e71-119">delete</span></span>        | <span data-ttu-id="24e71-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-120">[deleteAction][]</span></span>  | <span data-ttu-id="24e71-121">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="24e71-121">An item was deleted.</span></span>
| <span data-ttu-id="24e71-122">edit</span><span class="sxs-lookup"><span data-stu-id="24e71-122">edit</span></span>          | <span data-ttu-id="24e71-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-123">[editAction][]</span></span>    | <span data-ttu-id="24e71-124">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="24e71-124">An item was edited.</span></span>
| <span data-ttu-id="24e71-125">mention</span><span class="sxs-lookup"><span data-stu-id="24e71-125">mention</span></span>       | <span data-ttu-id="24e71-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-126">[mentionAction][]</span></span> | <span data-ttu-id="24e71-127">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="24e71-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="24e71-128">move</span><span class="sxs-lookup"><span data-stu-id="24e71-128">move</span></span>          | <span data-ttu-id="24e71-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-129">[moveAction][]</span></span>    | <span data-ttu-id="24e71-130">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="24e71-130">An item was moved.</span></span>
| <span data-ttu-id="24e71-131">rename</span><span class="sxs-lookup"><span data-stu-id="24e71-131">rename</span></span>        | <span data-ttu-id="24e71-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-132">[renameAction][]</span></span>  | <span data-ttu-id="24e71-133">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="24e71-133">An item was renamed.</span></span>
| <span data-ttu-id="24e71-134">restore</span><span class="sxs-lookup"><span data-stu-id="24e71-134">restore</span></span>       | <span data-ttu-id="24e71-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-135">[restoreAction][]</span></span> | <span data-ttu-id="24e71-136">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="24e71-136">An item was restored.</span></span>
| <span data-ttu-id="24e71-137">share</span><span class="sxs-lookup"><span data-stu-id="24e71-137">share</span></span>         | <span data-ttu-id="24e71-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-138">[shareAction][]</span></span>   | <span data-ttu-id="24e71-139">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="24e71-139">An item was shared.</span></span>
| <span data-ttu-id="24e71-140">version</span><span class="sxs-lookup"><span data-stu-id="24e71-140">version</span></span>       | <span data-ttu-id="24e71-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="24e71-141">[versionAction][]</span></span> | <span data-ttu-id="24e71-142">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="24e71-142">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="24e71-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24e71-153">JSON representation</span></span>

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

