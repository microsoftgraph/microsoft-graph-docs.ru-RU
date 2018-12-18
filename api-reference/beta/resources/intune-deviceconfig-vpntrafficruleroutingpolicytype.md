---
title: Тип перечисления vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутизации для правила трафика через VPN.
author: tfitzmac
ms.openlocfilehash: 5aa3f44f0e4ccf177154f97e9849093c52728b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343423"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="bf0a1-103">Тип перечисления vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="bf0a1-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="bf0a1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf0a1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf0a1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf0a1-107">Указывает политику маршрутизации для правила трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="bf0a1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf0a1-108">Members</span></span>
|<span data-ttu-id="bf0a1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf0a1-109">Member</span></span>|<span data-ttu-id="bf0a1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bf0a1-110">Value</span></span>|<span data-ttu-id="bf0a1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf0a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf0a1-112">none</span><span class="sxs-lookup"><span data-stu-id="bf0a1-112">none</span></span>|<span data-ttu-id="bf0a1-113">0</span><span class="sxs-lookup"><span data-stu-id="bf0a1-113">0</span></span>|<span data-ttu-id="bf0a1-114">Маршрутизация политика не указан.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-114">No routing policy specified.</span></span>|
|<span data-ttu-id="bf0a1-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="bf0a1-115">splitTunnel</span></span>|<span data-ttu-id="bf0a1-116">1</span><span class="sxs-lookup"><span data-stu-id="bf0a1-116">1</span></span>|<span data-ttu-id="bf0a1-117">Сетевой трафик для указанного приложения будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="bf0a1-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="bf0a1-118">forceTunnel</span></span>|<span data-ttu-id="bf0a1-119">2</span><span class="sxs-lookup"><span data-stu-id="bf0a1-119">2</span></span>|<span data-ttu-id="bf0a1-120">Сетевой трафик будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="bf0a1-120">All network traffic will be routed through the VPN.</span></span>|





