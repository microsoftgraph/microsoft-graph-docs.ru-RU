---
author: daspek
ms.author: dspektor
title: Тип ресурса ItemActionSet
description: Объект itemActionSet предоставляет сведения о действиях, выполняемых в рамках действия с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 76778f959f52518ca4055a0da471bffeca5a73e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447698"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="8698a-103">Тип ресурса itemActionSet</span><span class="sxs-lookup"><span data-stu-id="8698a-103">itemActionSet resource type</span></span>

<span data-ttu-id="8698a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8698a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8698a-105">Ресурс **itemActionSet** предоставляет сведения о действиях, которые составляют [действие][itemActivity] для элемента.</span><span class="sxs-lookup"><span data-stu-id="8698a-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="8698a-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8698a-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="8698a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8698a-107">Properties</span></span>

<span data-ttu-id="8698a-108">В настоящее время доступны следующие действия.</span><span class="sxs-lookup"><span data-stu-id="8698a-108">The following actions are currently available.</span></span> <span data-ttu-id="8698a-109">Так как новые действия могут быть добавлены в будущем, убедитесь, что ваше приложение может обрабатывать **itemActionSet** , который включает неизвестные действия.</span><span class="sxs-lookup"><span data-stu-id="8698a-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="8698a-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8698a-110">Property name</span></span> | <span data-ttu-id="8698a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8698a-111">Type</span></span>              | <span data-ttu-id="8698a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8698a-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="8698a-113">comment</span><span class="sxs-lookup"><span data-stu-id="8698a-113">comment</span></span>       | <span data-ttu-id="8698a-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-114">[commentAction][]</span></span> | <span data-ttu-id="8698a-115">В элемент добавлен комментарий.</span><span class="sxs-lookup"><span data-stu-id="8698a-115">A comment was added to the item.</span></span>
| <span data-ttu-id="8698a-116">create</span><span class="sxs-lookup"><span data-stu-id="8698a-116">create</span></span>        | <span data-ttu-id="8698a-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-117">[createAction][]</span></span>  | <span data-ttu-id="8698a-118">Был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="8698a-118">An item was created.</span></span>
| <span data-ttu-id="8698a-119">delete</span><span class="sxs-lookup"><span data-stu-id="8698a-119">delete</span></span>        | <span data-ttu-id="8698a-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-120">[deleteAction][]</span></span>  | <span data-ttu-id="8698a-121">Был удален элемент.</span><span class="sxs-lookup"><span data-stu-id="8698a-121">An item was deleted.</span></span>
| <span data-ttu-id="8698a-122">edit</span><span class="sxs-lookup"><span data-stu-id="8698a-122">edit</span></span>          | <span data-ttu-id="8698a-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-123">[editAction][]</span></span>    | <span data-ttu-id="8698a-124">Был изменен элемент.</span><span class="sxs-lookup"><span data-stu-id="8698a-124">An item was edited.</span></span>
| <span data-ttu-id="8698a-125">mention</span><span class="sxs-lookup"><span data-stu-id="8698a-125">mention</span></span>       | <span data-ttu-id="8698a-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-126">[mentionAction][]</span></span> | <span data-ttu-id="8698a-127">Пользователь был упомянут в элементе.</span><span class="sxs-lookup"><span data-stu-id="8698a-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="8698a-128">move</span><span class="sxs-lookup"><span data-stu-id="8698a-128">move</span></span>          | <span data-ttu-id="8698a-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-129">[moveAction][]</span></span>    | <span data-ttu-id="8698a-130">Элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="8698a-130">An item was moved.</span></span>
| <span data-ttu-id="8698a-131">rename</span><span class="sxs-lookup"><span data-stu-id="8698a-131">rename</span></span>        | <span data-ttu-id="8698a-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-132">[renameAction][]</span></span>  | <span data-ttu-id="8698a-133">Элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="8698a-133">An item was renamed.</span></span>
| <span data-ttu-id="8698a-134">restore</span><span class="sxs-lookup"><span data-stu-id="8698a-134">restore</span></span>       | <span data-ttu-id="8698a-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-135">[restoreAction][]</span></span> | <span data-ttu-id="8698a-136">Элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="8698a-136">An item was restored.</span></span>
| <span data-ttu-id="8698a-137">share</span><span class="sxs-lookup"><span data-stu-id="8698a-137">share</span></span>         | <span data-ttu-id="8698a-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-138">[shareAction][]</span></span>   | <span data-ttu-id="8698a-139">К элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="8698a-139">An item was shared.</span></span>
| <span data-ttu-id="8698a-140">version</span><span class="sxs-lookup"><span data-stu-id="8698a-140">version</span></span>       | <span data-ttu-id="8698a-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="8698a-141">[versionAction][]</span></span> | <span data-ttu-id="8698a-142">Для элемента была указана версия.</span><span class="sxs-lookup"><span data-stu-id="8698a-142">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="8698a-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8698a-153">JSON representation</span></span>

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
