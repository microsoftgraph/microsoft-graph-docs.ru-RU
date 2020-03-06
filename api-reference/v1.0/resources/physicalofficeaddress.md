---
title: Тип ресурса Фисикалоффицеаддресс
description: Представляет рабочий адрес ресурса, например контакт или событие.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c7b0280d8b9e7d62357985b88ead034b015aef1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534059"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="b5b88-103">Тип ресурса Фисикалоффицеаддресс</span><span class="sxs-lookup"><span data-stu-id="b5b88-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="b5b88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5b88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5b88-105">Представляет рабочий адрес ресурса, например контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="b5b88-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="b5b88-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5b88-106">Properties</span></span>

| <span data-ttu-id="b5b88-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5b88-107">Property</span></span>     | <span data-ttu-id="b5b88-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b5b88-108">Type</span></span>   |<span data-ttu-id="b5b88-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b5b88-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5b88-110">city</span><span class="sxs-lookup"><span data-stu-id="b5b88-110">city</span></span>|<span data-ttu-id="b5b88-111">Строка</span><span class="sxs-lookup"><span data-stu-id="b5b88-111">String</span></span>|<span data-ttu-id="b5b88-112">Город.</span><span class="sxs-lookup"><span data-stu-id="b5b88-112">The city.</span></span>|
|<span data-ttu-id="b5b88-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b5b88-113">countryOrRegion</span></span>|<span data-ttu-id="b5b88-114">String</span><span class="sxs-lookup"><span data-stu-id="b5b88-114">String</span></span>|<span data-ttu-id="b5b88-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="b5b88-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="b5b88-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b5b88-117">officeLocation</span></span>  | <span data-ttu-id="b5b88-118">Строка</span><span class="sxs-lookup"><span data-stu-id="b5b88-118">String</span></span> | <span data-ttu-id="b5b88-119">Местоположение Office, например здание и номер офиса для контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="b5b88-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="b5b88-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="b5b88-120">postalCode</span></span>|<span data-ttu-id="b5b88-121">Строка</span><span class="sxs-lookup"><span data-stu-id="b5b88-121">String</span></span>|<span data-ttu-id="b5b88-122">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="b5b88-122">The postal code.</span></span>|
|<span data-ttu-id="b5b88-123">state</span><span class="sxs-lookup"><span data-stu-id="b5b88-123">state</span></span>|<span data-ttu-id="b5b88-124">String</span><span class="sxs-lookup"><span data-stu-id="b5b88-124">String</span></span>|<span data-ttu-id="b5b88-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="b5b88-125">The state.</span></span>|
|<span data-ttu-id="b5b88-126">street</span><span class="sxs-lookup"><span data-stu-id="b5b88-126">street</span></span>|<span data-ttu-id="b5b88-127">String</span><span class="sxs-lookup"><span data-stu-id="b5b88-127">String</span></span>|<span data-ttu-id="b5b88-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="b5b88-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5b88-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5b88-129">JSON representation</span></span>

<span data-ttu-id="b5b88-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5b88-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
