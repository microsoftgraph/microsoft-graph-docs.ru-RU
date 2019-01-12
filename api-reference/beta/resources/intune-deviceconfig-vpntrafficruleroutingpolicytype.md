---
title: Тип перечисления vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутизации для правила трафика через VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c8ec4303dc16c7cb0606e4b9cf86594446f571e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974954"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="09cc2-103">Тип перечисления vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="09cc2-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="09cc2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="09cc2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09cc2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09cc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09cc2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09cc2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09cc2-107">Указывает политику маршрутизации для правила трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="09cc2-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="09cc2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="09cc2-108">Members</span></span>
|<span data-ttu-id="09cc2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="09cc2-109">Member</span></span>|<span data-ttu-id="09cc2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="09cc2-110">Value</span></span>|<span data-ttu-id="09cc2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="09cc2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09cc2-112">Нет</span><span class="sxs-lookup"><span data-stu-id="09cc2-112">none</span></span>|<span data-ttu-id="09cc2-113">0</span><span class="sxs-lookup"><span data-stu-id="09cc2-113">0</span></span>|<span data-ttu-id="09cc2-114">Маршрутизация политика не указан.</span><span class="sxs-lookup"><span data-stu-id="09cc2-114">No routing policy specified.</span></span>|
|<span data-ttu-id="09cc2-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="09cc2-115">splitTunnel</span></span>|<span data-ttu-id="09cc2-116">1</span><span class="sxs-lookup"><span data-stu-id="09cc2-116">1</span></span>|<span data-ttu-id="09cc2-117">Сетевой трафик для указанного приложения будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="09cc2-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="09cc2-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="09cc2-118">forceTunnel</span></span>|<span data-ttu-id="09cc2-119">2</span><span class="sxs-lookup"><span data-stu-id="09cc2-119">2</span></span>|<span data-ttu-id="09cc2-120">Сетевой трафик будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="09cc2-120">All network traffic will be routed through the VPN.</span></span>|





