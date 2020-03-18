---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 577408b34b7483ebc313f761dfaf47e0e09cdd90
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787287"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="69405-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="69405-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="69405-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69405-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69405-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69405-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69405-106">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="69405-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="69405-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="69405-107">Members</span></span>
|<span data-ttu-id="69405-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="69405-108">Member</span></span>|<span data-ttu-id="69405-109">Значение</span><span class="sxs-lookup"><span data-stu-id="69405-109">Value</span></span>|<span data-ttu-id="69405-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69405-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69405-111">none</span><span class="sxs-lookup"><span data-stu-id="69405-111">none</span></span>|<span data-ttu-id="69405-112">нуль</span><span class="sxs-lookup"><span data-stu-id="69405-112">0</span></span>|<span data-ttu-id="69405-113">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="69405-113">No routing policy specified.</span></span>|
|<span data-ttu-id="69405-114">сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="69405-114">splitTunnel</span></span>|<span data-ttu-id="69405-115">1,1</span><span class="sxs-lookup"><span data-stu-id="69405-115">1</span></span>|<span data-ttu-id="69405-116">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="69405-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="69405-117">форцетуннел</span><span class="sxs-lookup"><span data-stu-id="69405-117">forceTunnel</span></span>|<span data-ttu-id="69405-118">2</span><span class="sxs-lookup"><span data-stu-id="69405-118">2</span></span>|<span data-ttu-id="69405-119">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="69405-119">All network traffic will be routed through the VPN.</span></span>|



