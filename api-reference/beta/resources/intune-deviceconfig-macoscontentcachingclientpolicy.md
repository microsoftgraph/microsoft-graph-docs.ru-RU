---
title: тип перечисления Макосконтенткачингклиентполици
description: Определяет, какие клиенты будут обслуживать кэш контента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ff1146d69fabdb8a9e734e0ae82747831e0a390
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026644"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a><span data-ttu-id="9b5d9-103">тип перечисления Макосконтенткачингклиентполици</span><span class="sxs-lookup"><span data-stu-id="9b5d9-103">macOSContentCachingClientPolicy enum type</span></span>

<span data-ttu-id="9b5d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b5d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b5d9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b5d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b5d9-107">Определяет, какие клиенты будут обслуживать кэш контента.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-107">Determines which clients a content cache will serve.</span></span>

## <a name="members"></a><span data-ttu-id="9b5d9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9b5d9-108">Members</span></span>
|<span data-ttu-id="9b5d9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9b5d9-109">Member</span></span>|<span data-ttu-id="9b5d9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9b5d9-110">Value</span></span>|<span data-ttu-id="9b5d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9b5d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b5d9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9b5d9-112">notConfigured</span></span>|<span data-ttu-id="9b5d9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9b5d9-113">0</span></span>|<span data-ttu-id="9b5d9-114">По умолчанию используется значение Clients в локальной сети.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-114">Defaults to clients in local network.</span></span>|
|<span data-ttu-id="9b5d9-115">клиентсинлокалнетворк</span><span class="sxs-lookup"><span data-stu-id="9b5d9-115">clientsInLocalNetwork</span></span>|<span data-ttu-id="9b5d9-116">1 </span><span class="sxs-lookup"><span data-stu-id="9b5d9-116">1</span></span>|<span data-ttu-id="9b5d9-117">Кэши контента будут предоставлять контент только для устройств в непосредственных локальных сетях.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-117">Content caches will provide content to devices only in their immediate local network.</span></span>|
|<span data-ttu-id="9b5d9-118">клиентсвиссамепублиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="9b5d9-118">clientsWithSamePublicIpAddress</span></span>|<span data-ttu-id="9b5d9-119">2 </span><span class="sxs-lookup"><span data-stu-id="9b5d9-119">2</span></span>|<span data-ttu-id="9b5d9-120">Кэши контента будут предоставлять контент для устройств, использующих один общий IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-120">Content caches will provide content to devices that share the same public IP address.</span></span>|
|<span data-ttu-id="9b5d9-121">клиентсинкустомлокалнетворкс</span><span class="sxs-lookup"><span data-stu-id="9b5d9-121">clientsInCustomLocalNetworks</span></span>|<span data-ttu-id="9b5d9-122">4</span><span class="sxs-lookup"><span data-stu-id="9b5d9-122">3</span></span>|<span data-ttu-id="9b5d9-123">Кэши контента будут предоставлять контент для устройств в Контенткачингклиентлистенранжес.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-123">Content caches will provide content to devices in contentCachingClientListenRanges.</span></span>|
|<span data-ttu-id="9b5d9-124">клиентсинкустомлокалнетворксвисфаллбакк</span><span class="sxs-lookup"><span data-stu-id="9b5d9-124">clientsInCustomLocalNetworksWithFallback</span></span>|<span data-ttu-id="9b5d9-125">4 </span><span class="sxs-lookup"><span data-stu-id="9b5d9-125">4</span></span>|<span data-ttu-id="9b5d9-126">Кэши контента будут предоставлять контент для устройств в Контенткачингклиентлистенранжес, Контенткачингпирлистенранжес и Контенткачингпарентс.</span><span class="sxs-lookup"><span data-stu-id="9b5d9-126">Content caches will provide content to devices in contentCachingClientListenRanges, contentCachingPeerListenRanges, and contentCachingParents.</span></span>|






