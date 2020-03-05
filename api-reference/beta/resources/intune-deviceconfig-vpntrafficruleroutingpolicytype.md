---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d26e9c84f21fb952d4db58ef5faf28d1b696454
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529273"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="a2f0d-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="a2f0d-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="a2f0d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2f0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2f0d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2f0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2f0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2f0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2f0d-107">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="a2f0d-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="a2f0d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a2f0d-108">Members</span></span>
|<span data-ttu-id="a2f0d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a2f0d-109">Member</span></span>|<span data-ttu-id="a2f0d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a2f0d-110">Value</span></span>|<span data-ttu-id="a2f0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a2f0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f0d-112">нет</span><span class="sxs-lookup"><span data-stu-id="a2f0d-112">none</span></span>|<span data-ttu-id="a2f0d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a2f0d-113">0</span></span>|<span data-ttu-id="a2f0d-114">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="a2f0d-114">No routing policy specified.</span></span>|
|<span data-ttu-id="a2f0d-115">сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="a2f0d-115">splitTunnel</span></span>|<span data-ttu-id="a2f0d-116">1 </span><span class="sxs-lookup"><span data-stu-id="a2f0d-116">1</span></span>|<span data-ttu-id="a2f0d-117">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="a2f0d-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="a2f0d-118">форцетуннел</span><span class="sxs-lookup"><span data-stu-id="a2f0d-118">forceTunnel</span></span>|<span data-ttu-id="a2f0d-119">2 </span><span class="sxs-lookup"><span data-stu-id="a2f0d-119">2</span></span>|<span data-ttu-id="a2f0d-120">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="a2f0d-120">All network traffic will be routed through the VPN.</span></span>|



