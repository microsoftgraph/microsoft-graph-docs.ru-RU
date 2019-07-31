---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef932729149ea21580ff5a8f1cc3f52e253bfc50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009617"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="6b998-103">Тип ресурса Нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="6b998-103">networkInterface resource type</span></span>

<span data-ttu-id="6b998-104">Представляет сетевую карту (NIC), связанную с этим узлом.</span><span class="sxs-lookup"><span data-stu-id="6b998-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="6b998-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b998-105">Properties</span></span>

| <span data-ttu-id="6b998-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b998-106">Property</span></span>   | <span data-ttu-id="6b998-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6b998-107">Type</span></span> |<span data-ttu-id="6b998-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6b998-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b998-109">description</span><span class="sxs-lookup"><span data-stu-id="6b998-109">description</span></span>|<span data-ttu-id="6b998-110">String</span><span class="sxs-lookup"><span data-stu-id="6b998-110">String</span></span>|<span data-ttu-id="6b998-111">Описание сетевого адаптера (например, Ethernet-адаптера, подключения по локальной сети для адаптера беспроводной сети \* < # > и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6b998-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="6b998-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="6b998-112">ipV4Address</span></span>|<span data-ttu-id="6b998-113">String</span><span class="sxs-lookup"><span data-stu-id="6b998-113">String</span></span>|<span data-ttu-id="6b998-114">Последний IPv4-адрес, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="6b998-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="6b998-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="6b998-115">ipV6Address</span></span>|<span data-ttu-id="6b998-116">String</span><span class="sxs-lookup"><span data-stu-id="6b998-116">String</span></span>|<span data-ttu-id="6b998-117">Последний открытый (с нестандартным) IPv6-адрес, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="6b998-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="6b998-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="6b998-118">localIpV6Address</span></span>|<span data-ttu-id="6b998-119">String</span><span class="sxs-lookup"><span data-stu-id="6b998-119">String</span></span>|<span data-ttu-id="6b998-120">IPv6-адрес последней локальной локальной связи или локального сайта, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="6b998-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="6b998-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="6b998-121">macAddress</span></span>|<span data-ttu-id="6b998-122">String</span><span class="sxs-lookup"><span data-stu-id="6b998-122">String</span></span>|<span data-ttu-id="6b998-123">MAC-адрес сетевого адаптера на этом узле.</span><span class="sxs-lookup"><span data-stu-id="6b998-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b998-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b998-124">JSON representation</span></span>

<span data-ttu-id="6b998-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b998-125">The following is a JSON representation of the resource.</span></span>

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
