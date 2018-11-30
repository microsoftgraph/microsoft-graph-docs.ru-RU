---
title: Тип ресурса networkInterface
description: Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075513"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="a454d-103">Тип ресурса networkInterface</span><span class="sxs-lookup"><span data-stu-id="a454d-103">networkInterface resource type</span></span>

<span data-ttu-id="a454d-104">Представляет сетевой интерфейс карточки Интерфейсная плата связанного с этим узлом.</span><span class="sxs-lookup"><span data-stu-id="a454d-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="a454d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a454d-105">Properties</span></span>

| <span data-ttu-id="a454d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a454d-106">Property</span></span>   | <span data-ttu-id="a454d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a454d-107">Type</span></span> |<span data-ttu-id="a454d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a454d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a454d-109">описание</span><span class="sxs-lookup"><span data-stu-id="a454d-109">description</span></span>|<span data-ttu-id="a454d-110">String</span><span class="sxs-lookup"><span data-stu-id="a454d-110">String</span></span>|<span data-ttu-id="a454d-111">Описание сетевого Адаптера (например Ethernet-адаптер, беспроводной Сетевой адаптер подключение по локальной сети \* <> # д.).</span><span class="sxs-lookup"><span data-stu-id="a454d-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="a454d-112">IPv4-адрес</span><span class="sxs-lookup"><span data-stu-id="a454d-112">ipV4Address</span></span>|<span data-ttu-id="a454d-113">String</span><span class="sxs-lookup"><span data-stu-id="a454d-113">String</span></span>|<span data-ttu-id="a454d-114">Последний IPv4-адрес, связанный с этой сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="a454d-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="a454d-115">IPv6-адрес</span><span class="sxs-lookup"><span data-stu-id="a454d-115">ipV6Address</span></span>|<span data-ttu-id="a454d-116">String</span><span class="sxs-lookup"><span data-stu-id="a454d-116">String</span></span>|<span data-ttu-id="a454d-117">Последний общедоступных (также называемого глобальные) IPv6 адрес, связанный с этой сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="a454d-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="a454d-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="a454d-118">localIpV6Address</span></span>|<span data-ttu-id="a454d-119">String</span><span class="sxs-lookup"><span data-stu-id="a454d-119">String</span></span>|<span data-ttu-id="a454d-120">Последний локального (локальной связи или локального сайта) IPv6 адрес, связанный с этой сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="a454d-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="a454d-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="a454d-121">macAddress</span></span>|<span data-ttu-id="a454d-122">String</span><span class="sxs-lookup"><span data-stu-id="a454d-122">String</span></span>|<span data-ttu-id="a454d-123">MAC-адрес сетевого Адаптера на этом узле.</span><span class="sxs-lookup"><span data-stu-id="a454d-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a454d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a454d-124">JSON representation</span></span>

<span data-ttu-id="a454d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a454d-125">The following is a JSON representation of the resource.</span></span>

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