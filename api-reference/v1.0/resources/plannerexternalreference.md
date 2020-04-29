---
title: Тип ресурса Планнерекстерналреференце
description: Ресурс **планнерекстерналреференце** представляет метаданные ссылки (например, файл, URL-адрес). Это значение пар "свойство-значение" в объекте Екстерналреференцес.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3bc6a2e27d207dcbca7026c39b0067d7d6fc1561
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533999"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="018f8-104">Тип ресурса Планнерекстерналреференце</span><span class="sxs-lookup"><span data-stu-id="018f8-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="018f8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="018f8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="018f8-106">Ресурс **планнерекстерналреференце** представляет метаданные ссылки (например, файл, URL-адрес).</span><span class="sxs-lookup"><span data-stu-id="018f8-106">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="018f8-107">Это значение пар "свойство-значение" в [объекте екстерналреференцес](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="018f8-107">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="018f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="018f8-108">Properties</span></span>
| <span data-ttu-id="018f8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="018f8-109">Property</span></span>     | <span data-ttu-id="018f8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="018f8-110">Type</span></span>   |<span data-ttu-id="018f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="018f8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="018f8-112">alias</span><span class="sxs-lookup"><span data-stu-id="018f8-112">alias</span></span>|<span data-ttu-id="018f8-113">String</span><span class="sxs-lookup"><span data-stu-id="018f8-113">String</span></span>|<span data-ttu-id="018f8-114">Псевдоним имени для описания ссылки.</span><span class="sxs-lookup"><span data-stu-id="018f8-114">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="018f8-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="018f8-115">lastModifiedBy</span></span>|[<span data-ttu-id="018f8-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="018f8-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="018f8-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="018f8-117">Read-only.</span></span> <span data-ttu-id="018f8-118">Идентификатор пользователя, на который последний раз изменился.</span><span class="sxs-lookup"><span data-stu-id="018f8-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="018f8-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="018f8-119">lastModifiedDateTime</span></span>|<span data-ttu-id="018f8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="018f8-120">DateTimeOffset</span></span>|<span data-ttu-id="018f8-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="018f8-121">Read-only.</span></span> <span data-ttu-id="018f8-122">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="018f8-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="018f8-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="018f8-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="018f8-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="018f8-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="018f8-125">превиевприорити</span><span class="sxs-lookup"><span data-stu-id="018f8-125">previewPriority</span></span>|<span data-ttu-id="018f8-126">String</span><span class="sxs-lookup"><span data-stu-id="018f8-126">String</span></span>|<span data-ttu-id="018f8-127">Используется для задания относительного порядка приоритетов, в соответствии с которым ссылка будет отображаться в качестве предварительной версии для задачи.</span><span class="sxs-lookup"><span data-stu-id="018f8-127">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="018f8-128">type</span><span class="sxs-lookup"><span data-stu-id="018f8-128">type</span></span>|<span data-ttu-id="018f8-129">String</span><span class="sxs-lookup"><span data-stu-id="018f8-129">String</span></span>|<span data-ttu-id="018f8-130">Используется для описания типа ссылки.</span><span class="sxs-lookup"><span data-stu-id="018f8-130">Used to describe the type of the reference.</span></span> <span data-ttu-id="018f8-131">Типы включают: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="018f8-131">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="018f8-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="018f8-132">JSON representation</span></span>
<span data-ttu-id="018f8-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="018f8-133">Here is a JSON representation of the resource.</span></span>

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
