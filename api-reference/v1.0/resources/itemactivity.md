---
author: daspek
ms.author: dspektor
title: Тип ресурса itemActivity
description: Объект itemActivity предоставляет сведения о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c05493ddeb8e007da6ba8b7508369b4d013e672
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970797"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="6157c-103">Тип ресурса itemActivity</span><span class="sxs-lookup"><span data-stu-id="6157c-103">itemActivity resource type</span></span>

<span data-ttu-id="6157c-104">Ресурс **itemActivity** предоставляет сведения о действиях, выполняемых над элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="6157c-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="6157c-105">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6157c-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="6157c-106">Действия, выполняемые в itemActivity, подробно описаны в свойстве [itemActionSet][] .</span><span class="sxs-lookup"><span data-stu-id="6157c-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="6157c-107">**Примечание:** **itemActivity** в настоящее время доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6157c-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="6157c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6157c-109">Properties</span></span>

| <span data-ttu-id="6157c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6157c-110">Property</span></span> | <span data-ttu-id="6157c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6157c-111">Type</span></span>                    | <span data-ttu-id="6157c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6157c-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="6157c-113">id</span><span class="sxs-lookup"><span data-stu-id="6157c-113">id</span></span>       | <span data-ttu-id="6157c-114">string</span><span class="sxs-lookup"><span data-stu-id="6157c-114">string</span></span>                  | <span data-ttu-id="6157c-115">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="6157c-115">The unique identifier of the activity.</span></span> <span data-ttu-id="6157c-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6157c-116">Read-only.</span></span>
| <span data-ttu-id="6157c-117">обращения</span><span class="sxs-lookup"><span data-stu-id="6157c-117">access</span></span>   | <span data-ttu-id="6157c-118">[Акцессактион][]</span><span class="sxs-lookup"><span data-stu-id="6157c-118">[accessAction][]</span></span>        | <span data-ttu-id="6157c-119">Доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="6157c-119">An item was accessed.</span></span>
| <span data-ttu-id="6157c-120">actor</span><span class="sxs-lookup"><span data-stu-id="6157c-120">actor</span></span>    | <span data-ttu-id="6157c-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6157c-121">[identitySet][]</span></span>         | <span data-ttu-id="6157c-122">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="6157c-122">Identity of who performed the action.</span></span> <span data-ttu-id="6157c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6157c-123">Read-only.</span></span>
| <span data-ttu-id="6157c-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6157c-124">activityDateTime</span></span>    | <span data-ttu-id="6157c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6157c-125">DateTimeOffset</span></span> | <span data-ttu-id="6157c-126">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="6157c-126">Details about when the activity took place.</span></span> <span data-ttu-id="6157c-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6157c-127">Read-only.</span></span>

[Акцессактион]: accessAction.md
[accessAction]: accessAction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="6157c-130">Связи</span><span class="sxs-lookup"><span data-stu-id="6157c-130">Relationships</span></span>

| <span data-ttu-id="6157c-131">Имя связи</span><span class="sxs-lookup"><span data-stu-id="6157c-131">Relationship name</span></span> | <span data-ttu-id="6157c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6157c-132">Type</span></span>          | <span data-ttu-id="6157c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6157c-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="6157c-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="6157c-134">driveItem</span></span>         | <span data-ttu-id="6157c-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6157c-135">[driveItem][]</span></span> | <span data-ttu-id="6157c-136">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="6157c-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="6157c-137">listItem</span><span class="sxs-lookup"><span data-stu-id="6157c-137">listItem</span></span>          | <span data-ttu-id="6157c-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="6157c-138">[listItem][]</span></span>  | <span data-ttu-id="6157c-139">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="6157c-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="6157c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6157c-142">JSON representation</span></span>

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
