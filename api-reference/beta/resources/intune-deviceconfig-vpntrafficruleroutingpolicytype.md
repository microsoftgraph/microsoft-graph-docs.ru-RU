---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fb72b606633356fc2de5cc0c41862a49517b416
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963396"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="142d2-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="142d2-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="142d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="142d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="142d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="142d2-106">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="142d2-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="142d2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="142d2-107">Members</span></span>
|<span data-ttu-id="142d2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="142d2-108">Member</span></span>|<span data-ttu-id="142d2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="142d2-109">Value</span></span>|<span data-ttu-id="142d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="142d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="142d2-111">none</span><span class="sxs-lookup"><span data-stu-id="142d2-111">none</span></span>|<span data-ttu-id="142d2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="142d2-112">0</span></span>|<span data-ttu-id="142d2-113">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="142d2-113">No routing policy specified.</span></span>|
|<span data-ttu-id="142d2-114">Сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="142d2-114">splitTunnel</span></span>|<span data-ttu-id="142d2-115">1,1</span><span class="sxs-lookup"><span data-stu-id="142d2-115">1</span></span>|<span data-ttu-id="142d2-116">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="142d2-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="142d2-117">Форцетуннел</span><span class="sxs-lookup"><span data-stu-id="142d2-117">forceTunnel</span></span>|<span data-ttu-id="142d2-118">2</span><span class="sxs-lookup"><span data-stu-id="142d2-118">2</span></span>|<span data-ttu-id="142d2-119">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="142d2-119">All network traffic will be routed through the VPN.</span></span>|





