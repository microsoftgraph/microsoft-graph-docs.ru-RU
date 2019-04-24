---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
ms.openlocfilehash: 2bbfc3f38d4d353d370b9c8ba859b06cc2e4398b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462468"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="d91ed-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d91ed-103">physicalAddress resource type</span></span>

<span data-ttu-id="d91ed-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="d91ed-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="d91ed-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d91ed-105">Properties</span></span>
| <span data-ttu-id="d91ed-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d91ed-106">Property</span></span>     | <span data-ttu-id="d91ed-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d91ed-107">Type</span></span>   |<span data-ttu-id="d91ed-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d91ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d91ed-109">city</span><span class="sxs-lookup"><span data-stu-id="d91ed-109">city</span></span>|<span data-ttu-id="d91ed-110">String</span><span class="sxs-lookup"><span data-stu-id="d91ed-110">String</span></span>|<span data-ttu-id="d91ed-111">Город.</span><span class="sxs-lookup"><span data-stu-id="d91ed-111">The city.</span></span>|
|<span data-ttu-id="d91ed-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="d91ed-112">countryOrRegion</span></span>|<span data-ttu-id="d91ed-113">String</span><span class="sxs-lookup"><span data-stu-id="d91ed-113">String</span></span>|<span data-ttu-id="d91ed-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="d91ed-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="d91ed-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="d91ed-116">postalCode</span></span>|<span data-ttu-id="d91ed-117">String</span><span class="sxs-lookup"><span data-stu-id="d91ed-117">String</span></span>|<span data-ttu-id="d91ed-118">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="d91ed-118">The postal code.</span></span>|
|<span data-ttu-id="d91ed-119">state</span><span class="sxs-lookup"><span data-stu-id="d91ed-119">state</span></span>|<span data-ttu-id="d91ed-120">String</span><span class="sxs-lookup"><span data-stu-id="d91ed-120">String</span></span>|<span data-ttu-id="d91ed-121">Штат.</span><span class="sxs-lookup"><span data-stu-id="d91ed-121">The state.</span></span>|
|<span data-ttu-id="d91ed-122">street</span><span class="sxs-lookup"><span data-stu-id="d91ed-122">street</span></span>|<span data-ttu-id="d91ed-123">String</span><span class="sxs-lookup"><span data-stu-id="d91ed-123">String</span></span>|<span data-ttu-id="d91ed-124">Улица.</span><span class="sxs-lookup"><span data-stu-id="d91ed-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d91ed-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d91ed-125">JSON representation</span></span>

<span data-ttu-id="d91ed-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d91ed-126">Here is a JSON representation of the resource</span></span>

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
