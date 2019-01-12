---
title: Тип перечисления appleVpnConnectionType
description: Тип подключения Apple VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94b39d6804a304cf84e6dbefa3ef715f837b55af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912696"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="0d0f2-103">Тип перечисления appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0d0f2-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="0d0f2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d0f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d0f2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d0f2-107">Тип подключения Apple VPN.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="0d0f2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0d0f2-108">Members</span></span>
|<span data-ttu-id="0d0f2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0d0f2-109">Member</span></span>|<span data-ttu-id="0d0f2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0d0f2-110">Value</span></span>|<span data-ttu-id="0d0f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d0f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d0f2-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="0d0f2-112">ciscoAnyConnect</span></span>|<span data-ttu-id="0d0f2-113">0</span><span class="sxs-lookup"><span data-stu-id="0d0f2-113">0</span></span>|<span data-ttu-id="0d0f2-114">Cisco AnyConnect.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="0d0f2-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="0d0f2-115">pulseSecure</span></span>|<span data-ttu-id="0d0f2-116">1</span><span class="sxs-lookup"><span data-stu-id="0d0f2-116">1</span></span>|<span data-ttu-id="0d0f2-117">Обеспечение безопасной Pulse.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-117">Pulse Secure.</span></span>|
|<span data-ttu-id="0d0f2-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="0d0f2-118">f5EdgeClient</span></span>|<span data-ttu-id="0d0f2-119">2</span><span class="sxs-lookup"><span data-stu-id="0d0f2-119">2</span></span>|<span data-ttu-id="0d0f2-120">F5 Клиент пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="0d0f2-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="0d0f2-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="0d0f2-122">3</span><span class="sxs-lookup"><span data-stu-id="0d0f2-122">3</span></span>|<span data-ttu-id="0d0f2-123">Подключение мобильного устройства SonicWALL Dell.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="0d0f2-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="0d0f2-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="0d0f2-125">4</span><span class="sxs-lookup"><span data-stu-id="0d0f2-125">4</span></span>|<span data-ttu-id="0d0f2-126">Проверьте точку капсула VPN.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="0d0f2-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="0d0f2-127">customVpn</span></span>|<span data-ttu-id="0d0f2-128">5</span><span class="sxs-lookup"><span data-stu-id="0d0f2-128">5</span></span>|<span data-ttu-id="0d0f2-129">Настройка сети VPN.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-129">Custom VPN.</span></span>|
|<span data-ttu-id="0d0f2-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="0d0f2-130">ciscoIPSec</span></span>|<span data-ttu-id="0d0f2-131">6</span><span class="sxs-lookup"><span data-stu-id="0d0f2-131">6</span></span>|<span data-ttu-id="0d0f2-132">Cisco (IP IPSec).</span><span class="sxs-lookup"><span data-stu-id="0d0f2-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="0d0f2-133">Citrix</span><span class="sxs-lookup"><span data-stu-id="0d0f2-133">citrix</span></span>|<span data-ttu-id="0d0f2-134">7</span><span class="sxs-lookup"><span data-stu-id="0d0f2-134">7</span></span>|<span data-ttu-id="0d0f2-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-135">Citrix.</span></span>|
|<span data-ttu-id="0d0f2-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="0d0f2-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="0d0f2-137">8</span><span class="sxs-lookup"><span data-stu-id="0d0f2-137">8</span></span>|<span data-ttu-id="0d0f2-138">Cisco AnyConnect версии 2.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="0d0f2-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="0d0f2-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="0d0f2-140">9</span><span class="sxs-lookup"><span data-stu-id="0d0f2-140">9</span></span>|<span data-ttu-id="0d0f2-141">GlobalProtect Пало сети компьютер.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="0d0f2-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="0d0f2-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="0d0f2-143">10</span><span class="sxs-lookup"><span data-stu-id="0d0f2-143">10</span></span>|<span data-ttu-id="0d0f2-144">Zscaler доступ Private.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="0d0f2-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="0d0f2-145">f5Access2018</span></span>|<span data-ttu-id="0d0f2-146">11</span><span class="sxs-lookup"><span data-stu-id="0d0f2-146">11</span></span>|<span data-ttu-id="0d0f2-147">F5 2018 доступа.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="0d0f2-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="0d0f2-148">citrixSso</span></span>|<span data-ttu-id="0d0f2-149">12</span><span class="sxs-lookup"><span data-stu-id="0d0f2-149">12</span></span>|<span data-ttu-id="0d0f2-150">Citrix единого входа.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-150">Citrix Sso.</span></span>|
|<span data-ttu-id="0d0f2-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="0d0f2-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="0d0f2-152">13</span><span class="sxs-lookup"><span data-stu-id="0d0f2-152">13</span></span>|<span data-ttu-id="0d0f2-153">Компьютер Пало сетей GlobalProtect версии 2.</span><span class="sxs-lookup"><span data-stu-id="0d0f2-153">Palo Alto Networks GlobalProtect V2.</span></span>|





