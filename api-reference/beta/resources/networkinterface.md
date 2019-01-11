---
title: Тип ресурса networkInterface
description: Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823305"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="28d58-103">Тип ресурса networkInterface</span><span class="sxs-lookup"><span data-stu-id="28d58-103">networkInterface resource type</span></span>

<span data-ttu-id="28d58-104">Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.</span><span class="sxs-lookup"><span data-stu-id="28d58-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="28d58-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="28d58-105">Properties</span></span>

| <span data-ttu-id="28d58-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="28d58-106">Property</span></span>   | <span data-ttu-id="28d58-107">Тип</span><span class="sxs-lookup"><span data-stu-id="28d58-107">Type</span></span> |<span data-ttu-id="28d58-108">Описание</span><span class="sxs-lookup"><span data-stu-id="28d58-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28d58-109">описание</span><span class="sxs-lookup"><span data-stu-id="28d58-109">description</span></span>|<span data-ttu-id="28d58-110">Строка</span><span class="sxs-lookup"><span data-stu-id="28d58-110">String</span></span>|<span data-ttu-id="28d58-111">Описание сетевого Адаптера (например Ethernet-адаптер, беспроводной Сетевой адаптер подключение по локальной сети \* <> # д.).</span><span class="sxs-lookup"><span data-stu-id="28d58-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="28d58-112">IPv4-адрес</span><span class="sxs-lookup"><span data-stu-id="28d58-112">ipV4Address</span></span>|<span data-ttu-id="28d58-113">Строка</span><span class="sxs-lookup"><span data-stu-id="28d58-113">String</span></span>|<span data-ttu-id="28d58-114">Последний IPv4-адрес, связанный с этой сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="28d58-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="28d58-115">IPv6-адрес</span><span class="sxs-lookup"><span data-stu-id="28d58-115">ipV6Address</span></span>|<span data-ttu-id="28d58-116">Строка</span><span class="sxs-lookup"><span data-stu-id="28d58-116">String</span></span>|<span data-ttu-id="28d58-117">Последний общедоступных (также называемого глобальные) IPv6 адрес, связанный с этой сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="28d58-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="28d58-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="28d58-118">localIpV6Address</span></span>|<span data-ttu-id="28d58-119">Строка</span><span class="sxs-lookup"><span data-stu-id="28d58-119">String</span></span>|<span data-ttu-id="28d58-120">Последний локального (локальной связи или локального сайта) IPv6 адрес, связанный с этой сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="28d58-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="28d58-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="28d58-121">macAddress</span></span>|<span data-ttu-id="28d58-122">Строка</span><span class="sxs-lookup"><span data-stu-id="28d58-122">String</span></span>|<span data-ttu-id="28d58-123">MAC-адрес сетевого Адаптера на этом узле.</span><span class="sxs-lookup"><span data-stu-id="28d58-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28d58-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28d58-124">JSON representation</span></span>

<span data-ttu-id="28d58-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28d58-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
