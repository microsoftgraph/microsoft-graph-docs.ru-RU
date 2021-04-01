---
title: тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c34d0bf2d35f51ecae7268ef754a228dc226664a
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473894"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="bd9b8-103">тип ресурса sharingDetail</span><span class="sxs-lookup"><span data-stu-id="bd9b8-103">sharingDetail resource type</span></span>

<span data-ttu-id="bd9b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd9b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd9b8-105">Сложный тип, содержащий свойства [элементов sharedInsight.](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="bd9b8-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bd9b8-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd9b8-106">JSON representation</span></span>
<span data-ttu-id="bd9b8-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd9b8-107">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "sharingReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="bd9b8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd9b8-108">Properties</span></span>

| <span data-ttu-id="bd9b8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd9b8-109">Property</span></span>              | <span data-ttu-id="bd9b8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd9b8-110">Type</span></span>          | <span data-ttu-id="bd9b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd9b8-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="bd9b8-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd9b8-112">sharedDateTime</span></span>        | <span data-ttu-id="bd9b8-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd9b8-113">DateTimeOffset</span></span>| <span data-ttu-id="bd9b8-114">Дата и время последнего общего делиться файлом.</span><span class="sxs-lookup"><span data-stu-id="bd9b8-114">The date and time the file was last shared.</span></span> <span data-ttu-id="bd9b8-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bd9b8-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bd9b8-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="bd9b8-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="bd9b8-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd9b8-117">Read-only.</span></span>  |
| <span data-ttu-id="bd9b8-118">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="bd9b8-118">sharingSubject</span></span>        | <span data-ttu-id="bd9b8-119">String</span><span class="sxs-lookup"><span data-stu-id="bd9b8-119">String</span></span>          | <span data-ttu-id="bd9b8-120">Тема, с которой был общий документ.</span><span class="sxs-lookup"><span data-stu-id="bd9b8-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="bd9b8-121">sharingType</span><span class="sxs-lookup"><span data-stu-id="bd9b8-121">sharingType</span></span>             | <span data-ttu-id="bd9b8-122">String</span><span class="sxs-lookup"><span data-stu-id="bd9b8-122">String</span></span>        | <span data-ttu-id="bd9b8-123">Определяет способ общего делиться документом с помощью "Link", "Attachment", "Group", "Site".</span><span class="sxs-lookup"><span data-stu-id="bd9b8-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="bd9b8-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="bd9b8-124">sharedBy</span></span>                | [<span data-ttu-id="bd9b8-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="bd9b8-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="bd9b8-126">Пользователь, который поделился документом.</span><span class="sxs-lookup"><span data-stu-id="bd9b8-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="bd9b8-127">sharingReference</span><span class="sxs-lookup"><span data-stu-id="bd9b8-127">sharingReference</span></span>        | [<span data-ttu-id="bd9b8-128">resourceReference</span><span class="sxs-lookup"><span data-stu-id="bd9b8-128">resourceReference</span></span>](insights-resourcereference.md)      |  |


