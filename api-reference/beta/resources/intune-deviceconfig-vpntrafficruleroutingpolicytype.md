---
title: Тип перечисления vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутизации для правила трафика через VPN.
ms.openlocfilehash: df51851ef0820f5982a6689421503364e9064c78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077572"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="2808b-103">Тип перечисления vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="2808b-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="2808b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2808b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2808b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2808b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2808b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2808b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2808b-107">Указывает политику маршрутизации для правила трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="2808b-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="2808b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2808b-108">Members</span></span>
|<span data-ttu-id="2808b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2808b-109">Member</span></span>|<span data-ttu-id="2808b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2808b-110">Value</span></span>|<span data-ttu-id="2808b-111">Description</span><span class="sxs-lookup"><span data-stu-id="2808b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2808b-112">Нет</span><span class="sxs-lookup"><span data-stu-id="2808b-112">none</span></span>|<span data-ttu-id="2808b-113">0</span><span class="sxs-lookup"><span data-stu-id="2808b-113">0</span></span>|<span data-ttu-id="2808b-114">Маршрутизация политика не указан.</span><span class="sxs-lookup"><span data-stu-id="2808b-114">No routing policy specified.</span></span>|
|<span data-ttu-id="2808b-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="2808b-115">splitTunnel</span></span>|<span data-ttu-id="2808b-116">1</span><span class="sxs-lookup"><span data-stu-id="2808b-116">1</span></span>|<span data-ttu-id="2808b-117">Сетевой трафик для указанного приложения будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="2808b-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="2808b-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="2808b-118">forceTunnel</span></span>|<span data-ttu-id="2808b-119">2</span><span class="sxs-lookup"><span data-stu-id="2808b-119">2</span></span>|<span data-ttu-id="2808b-120">Сетевой трафик будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="2808b-120">All network traffic will be routed through the VPN.</span></span>|





