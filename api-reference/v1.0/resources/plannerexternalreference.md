---
title: Тип ресурса Планнерекстерналреференце
description: Ресурс **планнерекстерналреференце** представляет метаданные ссылки (например, файл, URL-адрес). Это значение пар "свойство-значение" в объекте Екстерналреференцес.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f95c6661dd179a7078980894b87184059598319d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462363"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="d15ee-104">Тип ресурса Планнерекстерналреференце</span><span class="sxs-lookup"><span data-stu-id="d15ee-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="d15ee-105">Ресурс **планнерекстерналреференце** представляет метаданные ссылки (например, файл, URL-адрес).</span><span class="sxs-lookup"><span data-stu-id="d15ee-105">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="d15ee-106">Это значение пар "свойство-значение" в [объекте екстерналреференцес](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="d15ee-106">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="d15ee-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d15ee-107">Properties</span></span>
| <span data-ttu-id="d15ee-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d15ee-108">Property</span></span>     | <span data-ttu-id="d15ee-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d15ee-109">Type</span></span>   |<span data-ttu-id="d15ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d15ee-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d15ee-111">alias</span><span class="sxs-lookup"><span data-stu-id="d15ee-111">alias</span></span>|<span data-ttu-id="d15ee-112">String</span><span class="sxs-lookup"><span data-stu-id="d15ee-112">String</span></span>|<span data-ttu-id="d15ee-113">Псевдоним имени для описания ссылки.</span><span class="sxs-lookup"><span data-stu-id="d15ee-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="d15ee-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d15ee-114">lastModifiedBy</span></span>|[<span data-ttu-id="d15ee-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="d15ee-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="d15ee-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d15ee-116">Read-only.</span></span> <span data-ttu-id="d15ee-117">Идентификатор пользователя, на который последний раз изменился.</span><span class="sxs-lookup"><span data-stu-id="d15ee-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="d15ee-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d15ee-118">lastModifiedDateTime</span></span>|<span data-ttu-id="d15ee-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d15ee-119">DateTimeOffset</span></span>|<span data-ttu-id="d15ee-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d15ee-120">Read-only.</span></span> <span data-ttu-id="d15ee-121">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="d15ee-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="d15ee-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d15ee-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d15ee-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d15ee-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d15ee-124">Превиевприорити</span><span class="sxs-lookup"><span data-stu-id="d15ee-124">previewPriority</span></span>|<span data-ttu-id="d15ee-125">String</span><span class="sxs-lookup"><span data-stu-id="d15ee-125">String</span></span>|<span data-ttu-id="d15ee-126">Используется для задания относительного порядка приоритетов, в соответствии с которым ссылка будет отображаться в качестве предварительной версии для задачи.</span><span class="sxs-lookup"><span data-stu-id="d15ee-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="d15ee-127">type</span><span class="sxs-lookup"><span data-stu-id="d15ee-127">type</span></span>|<span data-ttu-id="d15ee-128">String</span><span class="sxs-lookup"><span data-stu-id="d15ee-128">String</span></span>|<span data-ttu-id="d15ee-129">Используется для описания типа ссылки.</span><span class="sxs-lookup"><span data-stu-id="d15ee-129">Used to describe the type of the reference.</span></span> <span data-ttu-id="d15ee-130">Типы включают: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="d15ee-130">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d15ee-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d15ee-131">JSON representation</span></span>
<span data-ttu-id="d15ee-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d15ee-132">Here is a JSON representation of the resource.</span></span>

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
