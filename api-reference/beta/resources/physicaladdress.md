---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
ms.openlocfilehash: 819240be3eb9a088fde43390fbb1d1d4af1fd30c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081409"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="37b9c-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="37b9c-103">physicalAddress resource type</span></span>

<span data-ttu-id="37b9c-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="37b9c-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="37b9c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="37b9c-105">Properties</span></span>
| <span data-ttu-id="37b9c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="37b9c-106">Property</span></span>     | <span data-ttu-id="37b9c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="37b9c-107">Type</span></span>   |<span data-ttu-id="37b9c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="37b9c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37b9c-109">type</span><span class="sxs-lookup"><span data-stu-id="37b9c-109">type</span></span>|<span data-ttu-id="37b9c-110">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-110">String</span></span>|<span data-ttu-id="37b9c-111">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="37b9c-111">The type of address.</span></span> <span data-ttu-id="37b9c-112">Возможные значения: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="37b9c-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="37b9c-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="37b9c-113">postOfficeBox</span></span>|<span data-ttu-id="37b9c-114">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-114">String</span></span>|<span data-ttu-id="37b9c-115">Номер абонентского ящика.</span><span class="sxs-lookup"><span data-stu-id="37b9c-115">The post office box number.</span></span>|
|<span data-ttu-id="37b9c-116">city</span><span class="sxs-lookup"><span data-stu-id="37b9c-116">city</span></span>|<span data-ttu-id="37b9c-117">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-117">String</span></span>|<span data-ttu-id="37b9c-118">Город.</span><span class="sxs-lookup"><span data-stu-id="37b9c-118">The city.</span></span>|
|<span data-ttu-id="37b9c-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="37b9c-119">countryOrRegion</span></span>|<span data-ttu-id="37b9c-120">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-120">String</span></span>|<span data-ttu-id="37b9c-p102">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="37b9c-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="37b9c-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="37b9c-123">postalCode</span></span>|<span data-ttu-id="37b9c-124">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-124">String</span></span>|<span data-ttu-id="37b9c-125">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="37b9c-125">The postal code.</span></span>|
|<span data-ttu-id="37b9c-126">state</span><span class="sxs-lookup"><span data-stu-id="37b9c-126">state</span></span>|<span data-ttu-id="37b9c-127">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-127">String</span></span>|<span data-ttu-id="37b9c-128">Штат.</span><span class="sxs-lookup"><span data-stu-id="37b9c-128">The state.</span></span>|
|<span data-ttu-id="37b9c-129">street</span><span class="sxs-lookup"><span data-stu-id="37b9c-129">street</span></span>|<span data-ttu-id="37b9c-130">String</span><span class="sxs-lookup"><span data-stu-id="37b9c-130">String</span></span>|<span data-ttu-id="37b9c-131">Улица.</span><span class="sxs-lookup"><span data-stu-id="37b9c-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37b9c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37b9c-132">JSON representation</span></span>

<span data-ttu-id="37b9c-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37b9c-133">Here is a JSON representation of the resource</span></span>

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
