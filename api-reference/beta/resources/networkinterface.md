---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d7b712c50d8cc19951f583cb8c9af7e185dba7ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029164"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="932dd-103">Тип ресурса Нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="932dd-103">networkInterface resource type</span></span>

<span data-ttu-id="932dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="932dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="932dd-105">Представляет сетевую карту (NIC), связанную с этим узлом.</span><span class="sxs-lookup"><span data-stu-id="932dd-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="932dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="932dd-106">Properties</span></span>

| <span data-ttu-id="932dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="932dd-107">Property</span></span>   | <span data-ttu-id="932dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="932dd-108">Type</span></span> |<span data-ttu-id="932dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="932dd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="932dd-110">description</span><span class="sxs-lookup"><span data-stu-id="932dd-110">description</span></span>|<span data-ttu-id="932dd-111">String</span><span class="sxs-lookup"><span data-stu-id="932dd-111">String</span></span>|<span data-ttu-id="932dd-112">Описание сетевого адаптера (например, Ethernet-адаптера, подключения по локальной сети для адаптера беспроводной сети \* < # > и т. д.).</span><span class="sxs-lookup"><span data-stu-id="932dd-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="932dd-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="932dd-113">ipV4Address</span></span>|<span data-ttu-id="932dd-114">String</span><span class="sxs-lookup"><span data-stu-id="932dd-114">String</span></span>|<span data-ttu-id="932dd-115">Последний IPv4-адрес, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="932dd-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="932dd-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="932dd-116">ipV6Address</span></span>|<span data-ttu-id="932dd-117">String</span><span class="sxs-lookup"><span data-stu-id="932dd-117">String</span></span>|<span data-ttu-id="932dd-118">Последний открытый (с нестандартным) IPv6-адрес, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="932dd-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="932dd-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="932dd-119">localIpV6Address</span></span>|<span data-ttu-id="932dd-120">String</span><span class="sxs-lookup"><span data-stu-id="932dd-120">String</span></span>|<span data-ttu-id="932dd-121">IPv6-адрес последней локальной локальной связи или локального сайта, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="932dd-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="932dd-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="932dd-122">macAddress</span></span>|<span data-ttu-id="932dd-123">String</span><span class="sxs-lookup"><span data-stu-id="932dd-123">String</span></span>|<span data-ttu-id="932dd-124">MAC-адрес сетевого адаптера на этом узле.</span><span class="sxs-lookup"><span data-stu-id="932dd-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="932dd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="932dd-125">JSON representation</span></span>

<span data-ttu-id="932dd-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="932dd-126">The following is a JSON representation of the resource.</span></span>

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


