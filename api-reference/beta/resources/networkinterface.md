---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5fd40bec964a73579863b8222cd4c90d58991502
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522577"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="ab7c7-103">Тип ресурса Нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="ab7c7-103">networkInterface resource type</span></span>

<span data-ttu-id="ab7c7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab7c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab7c7-105">Представляет сетевую карту (NIC), связанную с этим узлом.</span><span class="sxs-lookup"><span data-stu-id="ab7c7-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="ab7c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab7c7-106">Properties</span></span>

| <span data-ttu-id="ab7c7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab7c7-107">Property</span></span>   | <span data-ttu-id="ab7c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ab7c7-108">Type</span></span> |<span data-ttu-id="ab7c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ab7c7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab7c7-110">description</span><span class="sxs-lookup"><span data-stu-id="ab7c7-110">description</span></span>|<span data-ttu-id="ab7c7-111">String</span><span class="sxs-lookup"><span data-stu-id="ab7c7-111">String</span></span>|<span data-ttu-id="ab7c7-112">Описание сетевого адаптера (например, Ethernet-адаптера, подключения по локальной сети для адаптера беспроводной сети \* < # > и т. д.).</span><span class="sxs-lookup"><span data-stu-id="ab7c7-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="ab7c7-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="ab7c7-113">ipV4Address</span></span>|<span data-ttu-id="ab7c7-114">String</span><span class="sxs-lookup"><span data-stu-id="ab7c7-114">String</span></span>|<span data-ttu-id="ab7c7-115">Последний IPv4-адрес, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="ab7c7-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="ab7c7-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="ab7c7-116">ipV6Address</span></span>|<span data-ttu-id="ab7c7-117">String</span><span class="sxs-lookup"><span data-stu-id="ab7c7-117">String</span></span>|<span data-ttu-id="ab7c7-118">Последний открытый (с нестандартным) IPv6-адрес, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="ab7c7-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="ab7c7-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="ab7c7-119">localIpV6Address</span></span>|<span data-ttu-id="ab7c7-120">String</span><span class="sxs-lookup"><span data-stu-id="ab7c7-120">String</span></span>|<span data-ttu-id="ab7c7-121">IPv6-адрес последней локальной локальной связи или локального сайта, связанный с этим сетевым адаптером.</span><span class="sxs-lookup"><span data-stu-id="ab7c7-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="ab7c7-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="ab7c7-122">macAddress</span></span>|<span data-ttu-id="ab7c7-123">String</span><span class="sxs-lookup"><span data-stu-id="ab7c7-123">String</span></span>|<span data-ttu-id="ab7c7-124">MAC-адрес сетевого адаптера на этом узле.</span><span class="sxs-lookup"><span data-stu-id="ab7c7-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab7c7-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab7c7-125">JSON representation</span></span>

<span data-ttu-id="ab7c7-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab7c7-126">The following is a JSON representation of the resource.</span></span>

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
