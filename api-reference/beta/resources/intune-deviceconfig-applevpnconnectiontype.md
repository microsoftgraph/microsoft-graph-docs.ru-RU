---
title: Тип перечисления appleVpnConnectionType
description: Тип подключения Apple VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f40281934aa241f245772e0bc4c5cd5bbbd0ec33
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415679"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="ea15b-103">Тип перечисления appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ea15b-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="ea15b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea15b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea15b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea15b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea15b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea15b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea15b-107">Тип подключения Apple VPN.</span><span class="sxs-lookup"><span data-stu-id="ea15b-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="ea15b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ea15b-108">Members</span></span>
|<span data-ttu-id="ea15b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ea15b-109">Member</span></span>|<span data-ttu-id="ea15b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ea15b-110">Value</span></span>|<span data-ttu-id="ea15b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea15b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea15b-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="ea15b-112">ciscoAnyConnect</span></span>|<span data-ttu-id="ea15b-113">0</span><span class="sxs-lookup"><span data-stu-id="ea15b-113">0</span></span>|<span data-ttu-id="ea15b-114">Cisco AnyConnect.</span><span class="sxs-lookup"><span data-stu-id="ea15b-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="ea15b-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="ea15b-115">pulseSecure</span></span>|<span data-ttu-id="ea15b-116">1</span><span class="sxs-lookup"><span data-stu-id="ea15b-116">1</span></span>|<span data-ttu-id="ea15b-117">Обеспечение безопасной Pulse.</span><span class="sxs-lookup"><span data-stu-id="ea15b-117">Pulse Secure.</span></span>|
|<span data-ttu-id="ea15b-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="ea15b-118">f5EdgeClient</span></span>|<span data-ttu-id="ea15b-119">2</span><span class="sxs-lookup"><span data-stu-id="ea15b-119">2</span></span>|<span data-ttu-id="ea15b-120">F5 Клиент пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="ea15b-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="ea15b-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="ea15b-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="ea15b-122">3</span><span class="sxs-lookup"><span data-stu-id="ea15b-122">3</span></span>|<span data-ttu-id="ea15b-123">Подключение мобильного устройства SonicWALL Dell.</span><span class="sxs-lookup"><span data-stu-id="ea15b-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="ea15b-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="ea15b-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="ea15b-125">4</span><span class="sxs-lookup"><span data-stu-id="ea15b-125">4</span></span>|<span data-ttu-id="ea15b-126">Проверьте точку капсула VPN.</span><span class="sxs-lookup"><span data-stu-id="ea15b-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ea15b-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="ea15b-127">customVpn</span></span>|<span data-ttu-id="ea15b-128">5</span><span class="sxs-lookup"><span data-stu-id="ea15b-128">5</span></span>|<span data-ttu-id="ea15b-129">Настройка сети VPN.</span><span class="sxs-lookup"><span data-stu-id="ea15b-129">Custom VPN.</span></span>|
|<span data-ttu-id="ea15b-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="ea15b-130">ciscoIPSec</span></span>|<span data-ttu-id="ea15b-131">6</span><span class="sxs-lookup"><span data-stu-id="ea15b-131">6</span></span>|<span data-ttu-id="ea15b-132">Cisco (IP IPSec).</span><span class="sxs-lookup"><span data-stu-id="ea15b-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="ea15b-133">Citrix</span><span class="sxs-lookup"><span data-stu-id="ea15b-133">citrix</span></span>|<span data-ttu-id="ea15b-134">7</span><span class="sxs-lookup"><span data-stu-id="ea15b-134">7</span></span>|<span data-ttu-id="ea15b-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="ea15b-135">Citrix.</span></span>|
|<span data-ttu-id="ea15b-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="ea15b-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="ea15b-137">8</span><span class="sxs-lookup"><span data-stu-id="ea15b-137">8</span></span>|<span data-ttu-id="ea15b-138">Cisco AnyConnect версии 2.</span><span class="sxs-lookup"><span data-stu-id="ea15b-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="ea15b-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="ea15b-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="ea15b-140">9</span><span class="sxs-lookup"><span data-stu-id="ea15b-140">9</span></span>|<span data-ttu-id="ea15b-141">GlobalProtect Пало сети компьютер.</span><span class="sxs-lookup"><span data-stu-id="ea15b-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="ea15b-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="ea15b-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="ea15b-143">10</span><span class="sxs-lookup"><span data-stu-id="ea15b-143">10</span></span>|<span data-ttu-id="ea15b-144">Zscaler доступ Private.</span><span class="sxs-lookup"><span data-stu-id="ea15b-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="ea15b-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="ea15b-145">f5Access2018</span></span>|<span data-ttu-id="ea15b-146">11</span><span class="sxs-lookup"><span data-stu-id="ea15b-146">11</span></span>|<span data-ttu-id="ea15b-147">F5 2018 доступа.</span><span class="sxs-lookup"><span data-stu-id="ea15b-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="ea15b-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="ea15b-148">citrixSso</span></span>|<span data-ttu-id="ea15b-149">12</span><span class="sxs-lookup"><span data-stu-id="ea15b-149">12</span></span>|<span data-ttu-id="ea15b-150">Citrix единого входа.</span><span class="sxs-lookup"><span data-stu-id="ea15b-150">Citrix Sso.</span></span>|
|<span data-ttu-id="ea15b-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="ea15b-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="ea15b-152">13</span><span class="sxs-lookup"><span data-stu-id="ea15b-152">13</span></span>|<span data-ttu-id="ea15b-153">Компьютер Пало сетей GlobalProtect версии 2.</span><span class="sxs-lookup"><span data-stu-id="ea15b-153">Palo Alto Networks GlobalProtect V2.</span></span>|




