---
title: тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference представляет** метаданные ссылки (вложения, такие как файл, URL-адрес). Это значение пар значения свойства в объекте externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 536e7b6a933ffdad610bf6cce561b2546d60e5d2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722316"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="76058-104">тип ресурса plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="76058-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="76058-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76058-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76058-106">Ресурс **plannerExternalReference представляет** метаданные ссылки (вложения, такие как файл, URL-адрес).</span><span class="sxs-lookup"><span data-stu-id="76058-106">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="76058-107">Это значение пар свойств-значений в [объекте externalReferences.](plannerexternalreferences.md)</span><span class="sxs-lookup"><span data-stu-id="76058-107">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="76058-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="76058-108">Properties</span></span>
| <span data-ttu-id="76058-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="76058-109">Property</span></span>     | <span data-ttu-id="76058-110">Тип</span><span class="sxs-lookup"><span data-stu-id="76058-110">Type</span></span>   |<span data-ttu-id="76058-111">Описание</span><span class="sxs-lookup"><span data-stu-id="76058-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76058-112">alias</span><span class="sxs-lookup"><span data-stu-id="76058-112">alias</span></span>|<span data-ttu-id="76058-113">String</span><span class="sxs-lookup"><span data-stu-id="76058-113">String</span></span>|<span data-ttu-id="76058-114">Псевдоним имени для описания ссылки.</span><span class="sxs-lookup"><span data-stu-id="76058-114">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="76058-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="76058-115">lastModifiedBy</span></span>|[<span data-ttu-id="76058-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="76058-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="76058-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76058-117">Read-only.</span></span> <span data-ttu-id="76058-118">Пользовательский ID, с помощью которого он был изменен в последний раз.</span><span class="sxs-lookup"><span data-stu-id="76058-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="76058-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76058-119">lastModifiedDateTime</span></span>|<span data-ttu-id="76058-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76058-120">DateTimeOffset</span></span>|<span data-ttu-id="76058-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76058-121">Read-only.</span></span> <span data-ttu-id="76058-122">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="76058-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="76058-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="76058-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="76058-124">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="76058-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="76058-125">previewPriority</span><span class="sxs-lookup"><span data-stu-id="76058-125">previewPriority</span></span>|<span data-ttu-id="76058-126">String</span><span class="sxs-lookup"><span data-stu-id="76058-126">String</span></span>|<span data-ttu-id="76058-127">Используется для задания порядка относительного приоритета, в котором ссылка будет показана в качестве предварительного просмотра задачи.</span><span class="sxs-lookup"><span data-stu-id="76058-127">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="76058-128">type</span><span class="sxs-lookup"><span data-stu-id="76058-128">type</span></span>|<span data-ttu-id="76058-129">String</span><span class="sxs-lookup"><span data-stu-id="76058-129">String</span></span>|<span data-ttu-id="76058-130">Используется для описания типа ссылки.</span><span class="sxs-lookup"><span data-stu-id="76058-130">Used to describe the type of the reference.</span></span> <span data-ttu-id="76058-131">Типы включают: `PowerPoint` `Word` , , , `Excel` `Other` .</span><span class="sxs-lookup"><span data-stu-id="76058-131">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76058-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76058-132">JSON representation</span></span>
<span data-ttu-id="76058-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76058-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

