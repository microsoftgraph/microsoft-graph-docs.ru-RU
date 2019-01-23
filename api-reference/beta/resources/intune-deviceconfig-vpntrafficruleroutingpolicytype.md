---
title: Тип перечисления vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутизации для правила трафика через VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 028e49085e4a1fa5f01ac59ff00fbafd8846dfb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415007"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="26aa3-103">Тип перечисления vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="26aa3-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="26aa3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26aa3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="26aa3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26aa3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26aa3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26aa3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26aa3-107">Указывает политику маршрутизации для правила трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="26aa3-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="26aa3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="26aa3-108">Members</span></span>
|<span data-ttu-id="26aa3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="26aa3-109">Member</span></span>|<span data-ttu-id="26aa3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="26aa3-110">Value</span></span>|<span data-ttu-id="26aa3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26aa3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26aa3-112">none</span><span class="sxs-lookup"><span data-stu-id="26aa3-112">none</span></span>|<span data-ttu-id="26aa3-113">0</span><span class="sxs-lookup"><span data-stu-id="26aa3-113">0</span></span>|<span data-ttu-id="26aa3-114">Маршрутизация политика не указан.</span><span class="sxs-lookup"><span data-stu-id="26aa3-114">No routing policy specified.</span></span>|
|<span data-ttu-id="26aa3-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="26aa3-115">splitTunnel</span></span>|<span data-ttu-id="26aa3-116">1</span><span class="sxs-lookup"><span data-stu-id="26aa3-116">1</span></span>|<span data-ttu-id="26aa3-117">Сетевой трафик для указанного приложения будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="26aa3-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="26aa3-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="26aa3-118">forceTunnel</span></span>|<span data-ttu-id="26aa3-119">2</span><span class="sxs-lookup"><span data-stu-id="26aa3-119">2</span></span>|<span data-ttu-id="26aa3-120">Сетевой трафик будут направляться через VPN-Подключение.</span><span class="sxs-lookup"><span data-stu-id="26aa3-120">All network traffic will be routed through the VPN.</span></span>|




