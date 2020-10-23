---
title: тип перечисления Макосконтенткачингклиентполици
description: Определяет, какие клиенты будут обслуживать кэш контента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c6900fbc3f1e5c76fb11eed68a349438ead24f48
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735836"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a><span data-ttu-id="045da-103">тип перечисления Макосконтенткачингклиентполици</span><span class="sxs-lookup"><span data-stu-id="045da-103">macOSContentCachingClientPolicy enum type</span></span>

<span data-ttu-id="045da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="045da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="045da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="045da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="045da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="045da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="045da-107">Определяет, какие клиенты будут обслуживать кэш контента.</span><span class="sxs-lookup"><span data-stu-id="045da-107">Determines which clients a content cache will serve.</span></span>

## <a name="members"></a><span data-ttu-id="045da-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="045da-108">Members</span></span>
|<span data-ttu-id="045da-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="045da-109">Member</span></span>|<span data-ttu-id="045da-110">Значение</span><span class="sxs-lookup"><span data-stu-id="045da-110">Value</span></span>|<span data-ttu-id="045da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="045da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="045da-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="045da-112">notConfigured</span></span>|<span data-ttu-id="045da-113">нуль</span><span class="sxs-lookup"><span data-stu-id="045da-113">0</span></span>|<span data-ttu-id="045da-114">По умолчанию используется значение Clients в локальной сети.</span><span class="sxs-lookup"><span data-stu-id="045da-114">Defaults to clients in local network.</span></span>|
|<span data-ttu-id="045da-115">клиентсинлокалнетворк</span><span class="sxs-lookup"><span data-stu-id="045da-115">clientsInLocalNetwork</span></span>|<span data-ttu-id="045da-116">1,1</span><span class="sxs-lookup"><span data-stu-id="045da-116">1</span></span>|<span data-ttu-id="045da-117">Кэши контента будут предоставлять контент только для устройств в непосредственных локальных сетях.</span><span class="sxs-lookup"><span data-stu-id="045da-117">Content caches will provide content to devices only in their immediate local network.</span></span>|
|<span data-ttu-id="045da-118">клиентсвиссамепублиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="045da-118">clientsWithSamePublicIpAddress</span></span>|<span data-ttu-id="045da-119">2</span><span class="sxs-lookup"><span data-stu-id="045da-119">2</span></span>|<span data-ttu-id="045da-120">Кэши контента будут предоставлять контент для устройств, использующих один общий IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="045da-120">Content caches will provide content to devices that share the same public IP address.</span></span>|
|<span data-ttu-id="045da-121">клиентсинкустомлокалнетворкс</span><span class="sxs-lookup"><span data-stu-id="045da-121">clientsInCustomLocalNetworks</span></span>|<span data-ttu-id="045da-122">4</span><span class="sxs-lookup"><span data-stu-id="045da-122">3</span></span>|<span data-ttu-id="045da-123">Кэши контента будут предоставлять контент для устройств в Контенткачингклиентлистенранжес.</span><span class="sxs-lookup"><span data-stu-id="045da-123">Content caches will provide content to devices in contentCachingClientListenRanges.</span></span>|
|<span data-ttu-id="045da-124">клиентсинкустомлокалнетворксвисфаллбакк</span><span class="sxs-lookup"><span data-stu-id="045da-124">clientsInCustomLocalNetworksWithFallback</span></span>|<span data-ttu-id="045da-125">4 </span><span class="sxs-lookup"><span data-stu-id="045da-125">4</span></span>|<span data-ttu-id="045da-126">Кэши контента будут предоставлять контент для устройств в Контенткачингклиентлистенранжес, Контенткачингпирлистенранжес и Контенткачингпарентс.</span><span class="sxs-lookup"><span data-stu-id="045da-126">Content caches will provide content to devices in contentCachingClientListenRanges, contentCachingPeerListenRanges, and contentCachingParents.</span></span>|





