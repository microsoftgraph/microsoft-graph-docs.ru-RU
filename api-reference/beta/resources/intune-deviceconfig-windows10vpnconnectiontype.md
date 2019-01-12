---
title: Тип перечисления windows10VpnConnectionType
description: Типы подключений VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 77b9fb91f86cfa29b13e58c9a4c1a4dff768c3a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937877"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="1de59-103">Тип перечисления windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1de59-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="1de59-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1de59-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1de59-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1de59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1de59-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1de59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1de59-107">Типы подключений VPN.</span><span class="sxs-lookup"><span data-stu-id="1de59-107">VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="1de59-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1de59-108">Members</span></span>
|<span data-ttu-id="1de59-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1de59-109">Member</span></span>|<span data-ttu-id="1de59-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1de59-110">Value</span></span>|<span data-ttu-id="1de59-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1de59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1de59-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="1de59-112">pulseSecure</span></span>|<span data-ttu-id="1de59-113">0</span><span class="sxs-lookup"><span data-stu-id="1de59-113">0</span></span>|<span data-ttu-id="1de59-114">Обеспечение безопасной Pulse.</span><span class="sxs-lookup"><span data-stu-id="1de59-114">Pulse Secure.</span></span>|
|<span data-ttu-id="1de59-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="1de59-115">f5EdgeClient</span></span>|<span data-ttu-id="1de59-116">1</span><span class="sxs-lookup"><span data-stu-id="1de59-116">1</span></span>|<span data-ttu-id="1de59-117">F5 Клиент пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="1de59-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="1de59-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="1de59-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="1de59-119">2</span><span class="sxs-lookup"><span data-stu-id="1de59-119">2</span></span>|<span data-ttu-id="1de59-120">Подключение мобильного устройства SonicWALL Dell.</span><span class="sxs-lookup"><span data-stu-id="1de59-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="1de59-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="1de59-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="1de59-122">3</span><span class="sxs-lookup"><span data-stu-id="1de59-122">3</span></span>|<span data-ttu-id="1de59-123">Проверьте точку капсула VPN.</span><span class="sxs-lookup"><span data-stu-id="1de59-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="1de59-124">Автоматически</span><span class="sxs-lookup"><span data-stu-id="1de59-124">automatic</span></span>|<span data-ttu-id="1de59-125">4</span><span class="sxs-lookup"><span data-stu-id="1de59-125">4</span></span>|<span data-ttu-id="1de59-126">Автоматически.</span><span class="sxs-lookup"><span data-stu-id="1de59-126">Automatic.</span></span>|
|<span data-ttu-id="1de59-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="1de59-127">ikEv2</span></span>|<span data-ttu-id="1de59-128">5</span><span class="sxs-lookup"><span data-stu-id="1de59-128">5</span></span>|<span data-ttu-id="1de59-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="1de59-129">IKEv2.</span></span>|
|<span data-ttu-id="1de59-130">L2TP</span><span class="sxs-lookup"><span data-stu-id="1de59-130">l2tp</span></span>|<span data-ttu-id="1de59-131">6</span><span class="sxs-lookup"><span data-stu-id="1de59-131">6</span></span>|<span data-ttu-id="1de59-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="1de59-132">L2TP.</span></span>|
|<span data-ttu-id="1de59-133">протокол PPTP</span><span class="sxs-lookup"><span data-stu-id="1de59-133">pptp</span></span>|<span data-ttu-id="1de59-134">7</span><span class="sxs-lookup"><span data-stu-id="1de59-134">7</span></span>|<span data-ttu-id="1de59-135">ПРОТОКОЛ PPTP.</span><span class="sxs-lookup"><span data-stu-id="1de59-135">PPTP.</span></span>|
|<span data-ttu-id="1de59-136">Citrix</span><span class="sxs-lookup"><span data-stu-id="1de59-136">citrix</span></span>|<span data-ttu-id="1de59-137">8</span><span class="sxs-lookup"><span data-stu-id="1de59-137">8</span></span>|<span data-ttu-id="1de59-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="1de59-138">Citrix.</span></span>|
|<span data-ttu-id="1de59-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="1de59-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="1de59-140">9</span><span class="sxs-lookup"><span data-stu-id="1de59-140">9</span></span>|<span data-ttu-id="1de59-141">GlobalProtect Пало сети компьютер.</span><span class="sxs-lookup"><span data-stu-id="1de59-141">Palo Alto Networks GlobalProtect.</span></span>|





