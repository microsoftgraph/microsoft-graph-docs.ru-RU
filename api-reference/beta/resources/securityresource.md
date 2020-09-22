---
title: Тип ресурса Секуритиресаурце
description: Представляет ресурсы, связанные с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4d27b5815366bdce76e5f99f0410f67684e608ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988823"
---
# <a name="securityresource-resource-type"></a><span data-ttu-id="52a2b-103">Тип ресурса Секуритиресаурце</span><span class="sxs-lookup"><span data-stu-id="52a2b-103">securityResource resource type</span></span>

<span data-ttu-id="52a2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52a2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52a2b-105">Представляет ресурсы, связанные с оповещением.</span><span class="sxs-lookup"><span data-stu-id="52a2b-105">Represents the resources related to an alert.</span></span>

## <a name="properties"></a><span data-ttu-id="52a2b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="52a2b-106">Properties</span></span>

| <span data-ttu-id="52a2b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="52a2b-107">Property</span></span>   | <span data-ttu-id="52a2b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="52a2b-108">Type</span></span>|<span data-ttu-id="52a2b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="52a2b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52a2b-110">resource</span><span class="sxs-lookup"><span data-stu-id="52a2b-110">resource</span></span>|<span data-ttu-id="52a2b-111">String</span><span class="sxs-lookup"><span data-stu-id="52a2b-111">String</span></span>|<span data-ttu-id="52a2b-112">Имя ресурса, связанного с текущим оповещением.</span><span class="sxs-lookup"><span data-stu-id="52a2b-112">Name of the resource that is related to current alert.</span></span> <span data-ttu-id="52a2b-113">**Обязательное поле**.</span><span class="sxs-lookup"><span data-stu-id="52a2b-113">**Required**.</span></span>|
|<span data-ttu-id="52a2b-114">Ресурса</span><span class="sxs-lookup"><span data-stu-id="52a2b-114">resourceType</span></span>|[<span data-ttu-id="52a2b-115">секуритиресаурцетипе</span><span class="sxs-lookup"><span data-stu-id="52a2b-115">securityResourceType</span></span>](#securityresourcetype-values)|<span data-ttu-id="52a2b-116">Представляет тип ресурсов безопасности, связанных с оповещением.</span><span class="sxs-lookup"><span data-stu-id="52a2b-116">Represents type of security resources related to an alert.</span></span> <span data-ttu-id="52a2b-117">Возможные значения: `attacked`, `related`.</span><span class="sxs-lookup"><span data-stu-id="52a2b-117">Possible values are: `attacked`, `related`.</span></span>|

### <a name="securityresourcetype-values"></a><span data-ttu-id="52a2b-118">значения Секуритиресаурцетипе</span><span class="sxs-lookup"><span data-stu-id="52a2b-118">securityResourceType values</span></span>

|<span data-ttu-id="52a2b-119">Элемент</span><span class="sxs-lookup"><span data-stu-id="52a2b-119">Member</span></span>|<span data-ttu-id="52a2b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="52a2b-120">Value</span></span>|<span data-ttu-id="52a2b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="52a2b-121">Description</span></span>|
|-|-|-|
|<span data-ttu-id="52a2b-122">атаковать</span><span class="sxs-lookup"><span data-stu-id="52a2b-122">attacked</span></span>|<span data-ttu-id="52a2b-123">1 </span><span class="sxs-lookup"><span data-stu-id="52a2b-123">1</span></span>|<span data-ttu-id="52a2b-124">Ресурс был атакован в оповещении.</span><span class="sxs-lookup"><span data-stu-id="52a2b-124">The resource was attacked in the alert.</span></span>|
|<span data-ttu-id="52a2b-125">связываем</span><span class="sxs-lookup"><span data-stu-id="52a2b-125">related</span></span>|<span data-ttu-id="52a2b-126">2 </span><span class="sxs-lookup"><span data-stu-id="52a2b-126">2</span></span>|<span data-ttu-id="52a2b-127">Ресурс связан с оповещением, хотя и не может напрямую атаковаться.</span><span class="sxs-lookup"><span data-stu-id="52a2b-127">The resource is related to the alert, though not directly attacked.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52a2b-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52a2b-128">JSON representation</span></span>

<span data-ttu-id="52a2b-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52a2b-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


