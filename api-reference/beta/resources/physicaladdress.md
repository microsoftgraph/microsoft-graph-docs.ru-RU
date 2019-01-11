---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
ms.openlocfilehash: 3a656046cc23394fc8cff9100eb5ad2289050b25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823585"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="14640-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="14640-103">physicalAddress resource type</span></span>

<span data-ttu-id="14640-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="14640-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="14640-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="14640-105">Properties</span></span>
| <span data-ttu-id="14640-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="14640-106">Property</span></span>     | <span data-ttu-id="14640-107">Тип</span><span class="sxs-lookup"><span data-stu-id="14640-107">Type</span></span>   |<span data-ttu-id="14640-108">Описание</span><span class="sxs-lookup"><span data-stu-id="14640-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14640-109">type</span><span class="sxs-lookup"><span data-stu-id="14640-109">type</span></span>|<span data-ttu-id="14640-110">Строка</span><span class="sxs-lookup"><span data-stu-id="14640-110">String</span></span>|<span data-ttu-id="14640-111">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="14640-111">The type of address.</span></span> <span data-ttu-id="14640-112">Возможные значения: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="14640-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="14640-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="14640-113">postOfficeBox</span></span>|<span data-ttu-id="14640-114">Строка</span><span class="sxs-lookup"><span data-stu-id="14640-114">String</span></span>|<span data-ttu-id="14640-115">Номер абонентского ящика.</span><span class="sxs-lookup"><span data-stu-id="14640-115">The post office box number.</span></span>|
|<span data-ttu-id="14640-116">city</span><span class="sxs-lookup"><span data-stu-id="14640-116">city</span></span>|<span data-ttu-id="14640-117">String</span><span class="sxs-lookup"><span data-stu-id="14640-117">String</span></span>|<span data-ttu-id="14640-118">Город.</span><span class="sxs-lookup"><span data-stu-id="14640-118">The city.</span></span>|
|<span data-ttu-id="14640-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="14640-119">countryOrRegion</span></span>|<span data-ttu-id="14640-120">String</span><span class="sxs-lookup"><span data-stu-id="14640-120">String</span></span>|<span data-ttu-id="14640-p102">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="14640-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="14640-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="14640-123">postalCode</span></span>|<span data-ttu-id="14640-124">String</span><span class="sxs-lookup"><span data-stu-id="14640-124">String</span></span>|<span data-ttu-id="14640-125">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="14640-125">The postal code.</span></span>|
|<span data-ttu-id="14640-126">state</span><span class="sxs-lookup"><span data-stu-id="14640-126">state</span></span>|<span data-ttu-id="14640-127">String</span><span class="sxs-lookup"><span data-stu-id="14640-127">String</span></span>|<span data-ttu-id="14640-128">Штат.</span><span class="sxs-lookup"><span data-stu-id="14640-128">The state.</span></span>|
|<span data-ttu-id="14640-129">street</span><span class="sxs-lookup"><span data-stu-id="14640-129">street</span></span>|<span data-ttu-id="14640-130">String</span><span class="sxs-lookup"><span data-stu-id="14640-130">String</span></span>|<span data-ttu-id="14640-131">Улица.</span><span class="sxs-lookup"><span data-stu-id="14640-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14640-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14640-132">JSON representation</span></span>

<span data-ttu-id="14640-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14640-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
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
