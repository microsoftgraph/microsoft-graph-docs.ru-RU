---
title: Тип ресурса Нетворкинтерфаце
description: Представляет сетевую карту (NIC), связанную с этим узлом.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457069"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="a12d7-103">Тип ресурса Нетворкинтерфаце</span><span class="sxs-lookup"><span data-stu-id="a12d7-103">networkInterface resource type</span></span>

<span data-ttu-id="a12d7-104">Представляет сетевую карту (NIC), связанную с этим узлом.</span><span class="sxs-lookup"><span data-stu-id="a12d7-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="a12d7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a12d7-105">Properties</span></span>

| <span data-ttu-id="a12d7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a12d7-106">Property</span></span>   | <span data-ttu-id="a12d7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a12d7-107">Type</span></span> |<span data-ttu-id="a12d7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a12d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a12d7-109">description</span><span class="sxs-lookup"><span data-stu-id="a12d7-109">description</span></span>|<span data-ttu-id="a12d7-110">String</span><span class="sxs-lookup"><span data-stu-id="a12d7-110">String</span></span>|<span data-ttu-id="a12d7-111">Описание сетевого адаптера (например, Ethernet-адаптера, подключения по локальной сети для адаптера беспроводной сети \* _Лт_ # _Гт_ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="a12d7-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="a12d7-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="a12d7-112">ipV4Address</span></span>|<span data-ttu-id="a12d7-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a12d7-113">String</span></span>|<span data-ttu-id="a12d7-114">Последний IPv4-адрес, связанный с этим СЕТЕВЫМ АДАПТЕРом.</span><span class="sxs-lookup"><span data-stu-id="a12d7-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="a12d7-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="a12d7-115">ipV6Address</span></span>|<span data-ttu-id="a12d7-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a12d7-116">String</span></span>|<span data-ttu-id="a12d7-117">Последний открытый (с нестандартным) IPv6-адрес, связанный с этим СЕТЕВЫМ АДАПТЕРом.</span><span class="sxs-lookup"><span data-stu-id="a12d7-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="a12d7-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="a12d7-118">localIpV6Address</span></span>|<span data-ttu-id="a12d7-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a12d7-119">String</span></span>|<span data-ttu-id="a12d7-120">IPv6-адрес последней локальной локальной связи или локального сайта, связанный с этим СЕТЕВЫМ АДАПТЕРом.</span><span class="sxs-lookup"><span data-stu-id="a12d7-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="a12d7-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="a12d7-121">macAddress</span></span>|<span data-ttu-id="a12d7-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a12d7-122">String</span></span>|<span data-ttu-id="a12d7-123">MAC-адрес сетевого адаптера на этом узле.</span><span class="sxs-lookup"><span data-stu-id="a12d7-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a12d7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a12d7-124">JSON representation</span></span>

<span data-ttu-id="a12d7-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a12d7-125">The following is a JSON representation of the resource.</span></span>

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
