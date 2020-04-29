---
author: daspek
ms.author: dspektor
title: Тип ресурса itemActivity
description: Объект itemActivity предоставляет сведения о действиях, которые были выполнены над элементом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1ffbcc84f3cb399b131ae40c46cae9230e4cac8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447677"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="aa7fd-103">Тип ресурса itemActivity</span><span class="sxs-lookup"><span data-stu-id="aa7fd-103">itemActivity resource type</span></span>

<span data-ttu-id="aa7fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa7fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa7fd-105">Ресурс **itemActivity** предоставляет сведения о действиях, выполняемых над элементом или в контейнере.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="aa7fd-106">В настоящее время доступен только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="aa7fd-107">Действия, выполняемые в itemActivity, подробно описаны в свойстве [itemActionSet][] .</span><span class="sxs-lookup"><span data-stu-id="aa7fd-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="aa7fd-108">**Note:** **itemActivity** в настоящее время доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="aa7fd-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa7fd-110">Properties</span></span>

| <span data-ttu-id="aa7fd-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa7fd-111">Property</span></span> | <span data-ttu-id="aa7fd-112">Тип</span><span class="sxs-lookup"><span data-stu-id="aa7fd-112">Type</span></span>                    | <span data-ttu-id="aa7fd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="aa7fd-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="aa7fd-114">id</span><span class="sxs-lookup"><span data-stu-id="aa7fd-114">id</span></span>       | <span data-ttu-id="aa7fd-115">string</span><span class="sxs-lookup"><span data-stu-id="aa7fd-115">string</span></span>                  | <span data-ttu-id="aa7fd-116">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-116">The unique identifier of the activity.</span></span> <span data-ttu-id="aa7fd-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-117">Read-only.</span></span>
| <span data-ttu-id="aa7fd-118">обращения</span><span class="sxs-lookup"><span data-stu-id="aa7fd-118">access</span></span>   | <span data-ttu-id="aa7fd-119">[акцессактион][]</span><span class="sxs-lookup"><span data-stu-id="aa7fd-119">[accessAction][]</span></span>        | <span data-ttu-id="aa7fd-120">Доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-120">An item was accessed.</span></span>
| <span data-ttu-id="aa7fd-121">actor</span><span class="sxs-lookup"><span data-stu-id="aa7fd-121">actor</span></span>    | <span data-ttu-id="aa7fd-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="aa7fd-122">[identitySet][]</span></span>         | <span data-ttu-id="aa7fd-123">Удостоверение, выполнившее действие.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-123">Identity of who performed the action.</span></span> <span data-ttu-id="aa7fd-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-124">Read-only.</span></span>
| <span data-ttu-id="aa7fd-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="aa7fd-125">activityDateTime</span></span>    | <span data-ttu-id="aa7fd-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa7fd-126">DateTimeOffset</span></span> | <span data-ttu-id="aa7fd-127">Сведения о том, когда было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-127">Details about when the activity took place.</span></span> <span data-ttu-id="aa7fd-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-128">Read-only.</span></span>

[акцессактион]: accessaction.md
[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="aa7fd-131">Связи</span><span class="sxs-lookup"><span data-stu-id="aa7fd-131">Relationships</span></span>

| <span data-ttu-id="aa7fd-132">Имя связи</span><span class="sxs-lookup"><span data-stu-id="aa7fd-132">Relationship name</span></span> | <span data-ttu-id="aa7fd-133">Тип</span><span class="sxs-lookup"><span data-stu-id="aa7fd-133">Type</span></span>          | <span data-ttu-id="aa7fd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="aa7fd-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="aa7fd-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="aa7fd-135">driveItem</span></span>         | <span data-ttu-id="aa7fd-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="aa7fd-136">[driveItem][]</span></span> | <span data-ttu-id="aa7fd-137">Представляет объект **driveItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="aa7fd-138">listItem</span><span class="sxs-lookup"><span data-stu-id="aa7fd-138">listItem</span></span>          | <span data-ttu-id="aa7fd-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="aa7fd-139">[listItem][]</span></span>  | <span data-ttu-id="aa7fd-140">Представляет объект **listItem**, с которым было выполнено действие.</span><span class="sxs-lookup"><span data-stu-id="aa7fd-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="aa7fd-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa7fd-143">JSON representation</span></span>

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
