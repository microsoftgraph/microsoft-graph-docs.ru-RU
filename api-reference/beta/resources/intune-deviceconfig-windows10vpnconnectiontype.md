---
title: Тип перечисления windows10VpnConnectionType
description: Типы подключений VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b3114c5d608cfed786fab8d2734d723682670ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395939"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="a3efd-103">Тип перечисления windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a3efd-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="a3efd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3efd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3efd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3efd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3efd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3efd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3efd-107">Типы подключений VPN.</span><span class="sxs-lookup"><span data-stu-id="a3efd-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="a3efd-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3efd-108">Members</span></span>
|<span data-ttu-id="a3efd-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3efd-109">Member</span></span>|<span data-ttu-id="a3efd-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a3efd-110">Value</span></span>|<span data-ttu-id="a3efd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3efd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3efd-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="a3efd-112">pulseSecure</span></span>|<span data-ttu-id="a3efd-113">0</span><span class="sxs-lookup"><span data-stu-id="a3efd-113">0</span></span>|<span data-ttu-id="a3efd-114">Обеспечение безопасной Pulse.</span><span class="sxs-lookup"><span data-stu-id="a3efd-114">Pulse Secure.</span></span>|
|<span data-ttu-id="a3efd-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="a3efd-115">f5EdgeClient</span></span>|<span data-ttu-id="a3efd-116">1</span><span class="sxs-lookup"><span data-stu-id="a3efd-116">1</span></span>|<span data-ttu-id="a3efd-117">F5 Клиент пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="a3efd-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="a3efd-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="a3efd-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="a3efd-119">2</span><span class="sxs-lookup"><span data-stu-id="a3efd-119">2</span></span>|<span data-ttu-id="a3efd-120">Подключение мобильного устройства SonicWALL Dell.</span><span class="sxs-lookup"><span data-stu-id="a3efd-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a3efd-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="a3efd-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="a3efd-122">3</span><span class="sxs-lookup"><span data-stu-id="a3efd-122">3</span></span>|<span data-ttu-id="a3efd-123">Проверьте точку капсула VPN.</span><span class="sxs-lookup"><span data-stu-id="a3efd-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="a3efd-124">Автоматически</span><span class="sxs-lookup"><span data-stu-id="a3efd-124">automatic</span></span>|<span data-ttu-id="a3efd-125">4</span><span class="sxs-lookup"><span data-stu-id="a3efd-125">4</span></span>|<span data-ttu-id="a3efd-126">Автоматически.</span><span class="sxs-lookup"><span data-stu-id="a3efd-126">Automatic.</span></span>|
|<span data-ttu-id="a3efd-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="a3efd-127">ikEv2</span></span>|<span data-ttu-id="a3efd-128">5</span><span class="sxs-lookup"><span data-stu-id="a3efd-128">5</span></span>|<span data-ttu-id="a3efd-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="a3efd-129">IKEv2.</span></span>|
|<span data-ttu-id="a3efd-130">L2TP</span><span class="sxs-lookup"><span data-stu-id="a3efd-130">l2tp</span></span>|<span data-ttu-id="a3efd-131">6</span><span class="sxs-lookup"><span data-stu-id="a3efd-131">6</span></span>|<span data-ttu-id="a3efd-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="a3efd-132">L2TP.</span></span>|
|<span data-ttu-id="a3efd-133">протокол PPTP</span><span class="sxs-lookup"><span data-stu-id="a3efd-133">pptp</span></span>|<span data-ttu-id="a3efd-134">7</span><span class="sxs-lookup"><span data-stu-id="a3efd-134">7</span></span>|<span data-ttu-id="a3efd-135">ПРОТОКОЛ PPTP.</span><span class="sxs-lookup"><span data-stu-id="a3efd-135">PPTP.</span></span>|
|<span data-ttu-id="a3efd-136">Citrix</span><span class="sxs-lookup"><span data-stu-id="a3efd-136">citrix</span></span>|<span data-ttu-id="a3efd-137">8</span><span class="sxs-lookup"><span data-stu-id="a3efd-137">8</span></span>|<span data-ttu-id="a3efd-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="a3efd-138">Citrix.</span></span>|
|<span data-ttu-id="a3efd-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="a3efd-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="a3efd-140">9</span><span class="sxs-lookup"><span data-stu-id="a3efd-140">9</span></span>|<span data-ttu-id="a3efd-141">GlobalProtect Пало сети компьютер.</span><span class="sxs-lookup"><span data-stu-id="a3efd-141">Palo Alto Networks GlobalProtect.</span></span>|




