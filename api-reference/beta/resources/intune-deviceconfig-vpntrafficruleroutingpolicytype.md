---
title: Тип перечисления vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутизации для правила трафика через VPN.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b44a2b58cc42e9f3f88964d79473327f4ca2b74
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855323"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="e57d6-103">Тип перечисления vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="e57d6-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="e57d6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e57d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e57d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e57d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e57d6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e57d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e57d6-107">Указывает политику маршрутизации для правила трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="e57d6-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="e57d6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e57d6-108">Members</span></span>
|<span data-ttu-id="e57d6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e57d6-109">Member</span></span>|<span data-ttu-id="e57d6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e57d6-110">Value</span></span>|<span data-ttu-id="e57d6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e57d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e57d6-112">Нет</span><span class="sxs-lookup"><span data-stu-id="e57d6-112">none</span></span>|<span data-ttu-id="e57d6-113">0</span><span class="sxs-lookup"><span data-stu-id="e57d6-113">0</span></span>|<span data-ttu-id="e57d6-114">Маршрутизация политика не указан.</span><span class="sxs-lookup"><span data-stu-id="e57d6-114">No routing policy specified.</span></span>|
|<span data-ttu-id="e57d6-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="e57d6-115">splitTunnel</span></span>|<span data-ttu-id="e57d6-116">1</span><span class="sxs-lookup"><span data-stu-id="e57d6-116">1</span></span>|<span data-ttu-id="e57d6-117">Сетевой трафик для указанного приложения будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="e57d6-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="e57d6-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="e57d6-118">forceTunnel</span></span>|<span data-ttu-id="e57d6-119">2</span><span class="sxs-lookup"><span data-stu-id="e57d6-119">2</span></span>|<span data-ttu-id="e57d6-120">Сетевой трафик будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="e57d6-120">All network traffic will be routed through the VPN.</span></span>|





