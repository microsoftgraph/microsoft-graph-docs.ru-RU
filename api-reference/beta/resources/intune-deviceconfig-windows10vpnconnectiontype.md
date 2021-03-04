---
title: тип enum windows10VpnConnectionType
description: Типы VPN-подключений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0f9fb609ab1386105c3b80c060d6dbde35080d53
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444513"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="fe07c-103">тип enum windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="fe07c-103">windows10VpnConnectionType enum type</span></span>

<span data-ttu-id="fe07c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe07c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe07c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe07c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe07c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe07c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe07c-107">Типы VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="fe07c-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="fe07c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fe07c-108">Members</span></span>
|<span data-ttu-id="fe07c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fe07c-109">Member</span></span>|<span data-ttu-id="fe07c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fe07c-110">Value</span></span>|<span data-ttu-id="fe07c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe07c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe07c-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="fe07c-112">pulseSecure</span></span>|<span data-ttu-id="fe07c-113">0</span><span class="sxs-lookup"><span data-stu-id="fe07c-113">0</span></span>|<span data-ttu-id="fe07c-114">Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="fe07c-114">Pulse Secure.</span></span>|
|<span data-ttu-id="fe07c-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="fe07c-115">f5EdgeClient</span></span>|<span data-ttu-id="fe07c-116">1 </span><span class="sxs-lookup"><span data-stu-id="fe07c-116">1</span></span>|<span data-ttu-id="fe07c-117">Клиент F5 Edge.</span><span class="sxs-lookup"><span data-stu-id="fe07c-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="fe07c-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="fe07c-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="fe07c-119">2 </span><span class="sxs-lookup"><span data-stu-id="fe07c-119">2</span></span>|<span data-ttu-id="fe07c-120">Мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="fe07c-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="fe07c-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="fe07c-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="fe07c-122">3 </span><span class="sxs-lookup"><span data-stu-id="fe07c-122">3</span></span>|<span data-ttu-id="fe07c-123">Check Point Capsule VPN.</span><span class="sxs-lookup"><span data-stu-id="fe07c-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="fe07c-124">Автоматически</span><span class="sxs-lookup"><span data-stu-id="fe07c-124">automatic</span></span>|<span data-ttu-id="fe07c-125">4 </span><span class="sxs-lookup"><span data-stu-id="fe07c-125">4</span></span>|<span data-ttu-id="fe07c-126">Автоматически.</span><span class="sxs-lookup"><span data-stu-id="fe07c-126">Automatic.</span></span>|
|<span data-ttu-id="fe07c-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="fe07c-127">ikEv2</span></span>|<span data-ttu-id="fe07c-128">5 </span><span class="sxs-lookup"><span data-stu-id="fe07c-128">5</span></span>|<span data-ttu-id="fe07c-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="fe07c-129">IKEv2.</span></span>|
|<span data-ttu-id="fe07c-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="fe07c-130">l2tp</span></span>|<span data-ttu-id="fe07c-131">6 </span><span class="sxs-lookup"><span data-stu-id="fe07c-131">6</span></span>|<span data-ttu-id="fe07c-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="fe07c-132">L2TP.</span></span>|
|<span data-ttu-id="fe07c-133">pptp</span><span class="sxs-lookup"><span data-stu-id="fe07c-133">pptp</span></span>|<span data-ttu-id="fe07c-134">7 </span><span class="sxs-lookup"><span data-stu-id="fe07c-134">7</span></span>|<span data-ttu-id="fe07c-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="fe07c-135">PPTP.</span></span>|
|<span data-ttu-id="fe07c-136">citrix</span><span class="sxs-lookup"><span data-stu-id="fe07c-136">citrix</span></span>|<span data-ttu-id="fe07c-137">8 </span><span class="sxs-lookup"><span data-stu-id="fe07c-137">8</span></span>|<span data-ttu-id="fe07c-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="fe07c-138">Citrix.</span></span>|
|<span data-ttu-id="fe07c-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="fe07c-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="fe07c-140">9 </span><span class="sxs-lookup"><span data-stu-id="fe07c-140">9</span></span>|<span data-ttu-id="fe07c-141">Palo Alto Networks GlobalProtect.</span><span class="sxs-lookup"><span data-stu-id="fe07c-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="fe07c-142">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="fe07c-142">ciscoAnyConnect</span></span>|<span data-ttu-id="fe07c-143">10 </span><span class="sxs-lookup"><span data-stu-id="fe07c-143">10</span></span>|<span data-ttu-id="fe07c-144">Cisco AnyConnect</span><span class="sxs-lookup"><span data-stu-id="fe07c-144">Cisco AnyConnect</span></span>|




