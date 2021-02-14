---
author: daspek
title: Тип ресурса itemActivity
description: Объект itemActivity предоставляет сведения о действии, которое произошло с элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ef213dd50e5a6be8a96880ccd1a64f15f183f54b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238689"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="3991b-103">Тип ресурса itemActivity</span><span class="sxs-lookup"><span data-stu-id="3991b-103">itemActivity resource type</span></span>

<span data-ttu-id="3991b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3991b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3991b-105">Ресурс **itemActivity** предоставляет сведения о действиях, которые произошли в элементе или контейнере.</span><span class="sxs-lookup"><span data-stu-id="3991b-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="3991b-106">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3991b-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="3991b-107">Действия, которые произошли в объекте itemActivity, подробно описаны в [свойстве itemActionSet.][]</span><span class="sxs-lookup"><span data-stu-id="3991b-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="3991b-108">**Примечание.** **ItemActivity** в настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3991b-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="3991b-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="3991b-110">Properties</span></span>

| <span data-ttu-id="3991b-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="3991b-111">Property</span></span> | <span data-ttu-id="3991b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3991b-112">Type</span></span>                    | <span data-ttu-id="3991b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3991b-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="3991b-114">id</span><span class="sxs-lookup"><span data-stu-id="3991b-114">id</span></span>       | <span data-ttu-id="3991b-115">string</span><span class="sxs-lookup"><span data-stu-id="3991b-115">string</span></span>                  | <span data-ttu-id="3991b-116">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="3991b-116">The unique identifier of the activity.</span></span> <span data-ttu-id="3991b-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3991b-117">Read-only.</span></span>
| <span data-ttu-id="3991b-118">access</span><span class="sxs-lookup"><span data-stu-id="3991b-118">access</span></span>   | <span data-ttu-id="3991b-119">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="3991b-119">[accessAction][]</span></span>        | <span data-ttu-id="3991b-120">Был доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="3991b-120">An item was accessed.</span></span>
| <span data-ttu-id="3991b-121">actor</span><span class="sxs-lookup"><span data-stu-id="3991b-121">actor</span></span>    | <span data-ttu-id="3991b-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3991b-122">[identitySet][]</span></span>         | <span data-ttu-id="3991b-123">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="3991b-123">Identity of who performed the action.</span></span> <span data-ttu-id="3991b-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3991b-124">Read-only.</span></span>
| <span data-ttu-id="3991b-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="3991b-125">activityDateTime</span></span>    | <span data-ttu-id="3991b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3991b-126">DateTimeOffset</span></span> | <span data-ttu-id="3991b-127">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="3991b-127">Details about when the activity took place.</span></span> <span data-ttu-id="3991b-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3991b-128">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="3991b-131">Связи</span><span class="sxs-lookup"><span data-stu-id="3991b-131">Relationships</span></span>

| <span data-ttu-id="3991b-132">Имя связи</span><span class="sxs-lookup"><span data-stu-id="3991b-132">Relationship name</span></span> | <span data-ttu-id="3991b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3991b-133">Type</span></span>          | <span data-ttu-id="3991b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3991b-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="3991b-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="3991b-135">driveItem</span></span>         | <span data-ttu-id="3991b-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="3991b-136">[driveItem][]</span></span> | <span data-ttu-id="3991b-137">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="3991b-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="3991b-138">listItem</span><span class="sxs-lookup"><span data-stu-id="3991b-138">listItem</span></span>          | <span data-ttu-id="3991b-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="3991b-139">[listItem][]</span></span>  | <span data-ttu-id="3991b-140">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="3991b-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="3991b-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3991b-143">JSON representation</span></span>

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

