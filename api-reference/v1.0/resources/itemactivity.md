---
author: daspek
ms.author: dspektor
title: Тип ресурса itemActivity
description: Объект itemActivity предоставляет сведения о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98ae9e4881de18c94490469b10df43b2aaf58140
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536689"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="61b54-103">Тип ресурса itemActivity</span><span class="sxs-lookup"><span data-stu-id="61b54-103">itemActivity resource type</span></span>

<span data-ttu-id="61b54-104">Ресурс **itemActivity** предоставляет сведения о действиях, выполняемых над элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="61b54-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="61b54-105">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="61b54-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="61b54-106">Действия, выполняемые в itemActivity, подробно описаны в свойстве [itemActionSet][] .</span><span class="sxs-lookup"><span data-stu-id="61b54-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="61b54-107">**Примечание:** **itemActivity** в настоящее время доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="61b54-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="61b54-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="61b54-109">Properties</span></span>

| <span data-ttu-id="61b54-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="61b54-110">Property</span></span> | <span data-ttu-id="61b54-111">Тип</span><span class="sxs-lookup"><span data-stu-id="61b54-111">Type</span></span>                    | <span data-ttu-id="61b54-112">Описание</span><span class="sxs-lookup"><span data-stu-id="61b54-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="61b54-113">id</span><span class="sxs-lookup"><span data-stu-id="61b54-113">id</span></span>       | <span data-ttu-id="61b54-114">string</span><span class="sxs-lookup"><span data-stu-id="61b54-114">string</span></span>                  | <span data-ttu-id="61b54-115">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="61b54-115">The unique identifier of the activity.</span></span> <span data-ttu-id="61b54-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61b54-116">Read-only.</span></span>
| <span data-ttu-id="61b54-117">обращения</span><span class="sxs-lookup"><span data-stu-id="61b54-117">access</span></span>   | <span data-ttu-id="61b54-118">[Акцессактион][]</span><span class="sxs-lookup"><span data-stu-id="61b54-118">[accessAction][]</span></span>        | <span data-ttu-id="61b54-119">Доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="61b54-119">An item was accessed.</span></span>
| <span data-ttu-id="61b54-120">actor</span><span class="sxs-lookup"><span data-stu-id="61b54-120">actor</span></span>    | <span data-ttu-id="61b54-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="61b54-121">[identitySet][]</span></span>         | <span data-ttu-id="61b54-122">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="61b54-122">Identity of who performed the action.</span></span> <span data-ttu-id="61b54-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61b54-123">Read-only.</span></span>
| <span data-ttu-id="61b54-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="61b54-124">activityDateTime</span></span>    | <span data-ttu-id="61b54-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61b54-125">DateTimeOffset</span></span> | <span data-ttu-id="61b54-126">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="61b54-126">Details about when the activity took place.</span></span> <span data-ttu-id="61b54-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61b54-127">Read-only.</span></span>

[Акцессактион]: accessaction.md
[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="61b54-130">Связи</span><span class="sxs-lookup"><span data-stu-id="61b54-130">Relationships</span></span>

| <span data-ttu-id="61b54-131">Имя связи</span><span class="sxs-lookup"><span data-stu-id="61b54-131">Relationship name</span></span> | <span data-ttu-id="61b54-132">Тип</span><span class="sxs-lookup"><span data-stu-id="61b54-132">Type</span></span>          | <span data-ttu-id="61b54-133">Описание</span><span class="sxs-lookup"><span data-stu-id="61b54-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="61b54-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="61b54-134">driveItem</span></span>         | <span data-ttu-id="61b54-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="61b54-135">[driveItem][]</span></span> | <span data-ttu-id="61b54-136">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="61b54-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="61b54-137">listItem</span><span class="sxs-lookup"><span data-stu-id="61b54-137">listItem</span></span>          | <span data-ttu-id="61b54-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="61b54-138">[listItem][]</span></span>  | <span data-ttu-id="61b54-139">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="61b54-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="61b54-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61b54-142">JSON representation</span></span>

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
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
