---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d9947e256001abd8168c886a0435e0725b3a1483
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072846"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="c858b-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c858b-103">physicalAddress resource type</span></span>

<span data-ttu-id="c858b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c858b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c858b-105">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="c858b-105">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="c858b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c858b-106">Properties</span></span>
| <span data-ttu-id="c858b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c858b-107">Property</span></span>     | <span data-ttu-id="c858b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c858b-108">Type</span></span>   |<span data-ttu-id="c858b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c858b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c858b-110">city</span><span class="sxs-lookup"><span data-stu-id="c858b-110">city</span></span>|<span data-ttu-id="c858b-111">String</span><span class="sxs-lookup"><span data-stu-id="c858b-111">String</span></span>|<span data-ttu-id="c858b-112">Город.</span><span class="sxs-lookup"><span data-stu-id="c858b-112">The city.</span></span>|
|<span data-ttu-id="c858b-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c858b-113">countryOrRegion</span></span>|<span data-ttu-id="c858b-114">String</span><span class="sxs-lookup"><span data-stu-id="c858b-114">String</span></span>|<span data-ttu-id="c858b-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="c858b-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="c858b-117">postalCode</span><span class="sxs-lookup"><span data-stu-id="c858b-117">postalCode</span></span>|<span data-ttu-id="c858b-118">String</span><span class="sxs-lookup"><span data-stu-id="c858b-118">String</span></span>|<span data-ttu-id="c858b-119">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="c858b-119">The postal code.</span></span>|
|<span data-ttu-id="c858b-120">state</span><span class="sxs-lookup"><span data-stu-id="c858b-120">state</span></span>|<span data-ttu-id="c858b-121">String</span><span class="sxs-lookup"><span data-stu-id="c858b-121">String</span></span>|<span data-ttu-id="c858b-122">Штат.</span><span class="sxs-lookup"><span data-stu-id="c858b-122">The state.</span></span>|
|<span data-ttu-id="c858b-123">street</span><span class="sxs-lookup"><span data-stu-id="c858b-123">street</span></span>|<span data-ttu-id="c858b-124">String</span><span class="sxs-lookup"><span data-stu-id="c858b-124">String</span></span>|<span data-ttu-id="c858b-125">Улица.</span><span class="sxs-lookup"><span data-stu-id="c858b-125">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c858b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c858b-126">JSON representation</span></span>

<span data-ttu-id="c858b-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c858b-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

