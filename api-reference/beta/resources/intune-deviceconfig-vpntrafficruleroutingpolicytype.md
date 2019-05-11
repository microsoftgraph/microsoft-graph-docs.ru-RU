---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0d699639d9af02b751ad701e4e6132bdc016911
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944504"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="6d2de-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="6d2de-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="6d2de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d2de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d2de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d2de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d2de-106">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="6d2de-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="6d2de-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6d2de-107">Members</span></span>
|<span data-ttu-id="6d2de-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6d2de-108">Member</span></span>|<span data-ttu-id="6d2de-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6d2de-109">Value</span></span>|<span data-ttu-id="6d2de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d2de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d2de-111">none</span><span class="sxs-lookup"><span data-stu-id="6d2de-111">none</span></span>|<span data-ttu-id="6d2de-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6d2de-112">0</span></span>|<span data-ttu-id="6d2de-113">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="6d2de-113">No routing policy specified.</span></span>|
|<span data-ttu-id="6d2de-114">Сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="6d2de-114">splitTunnel</span></span>|<span data-ttu-id="6d2de-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6d2de-115">1</span></span>|<span data-ttu-id="6d2de-116">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="6d2de-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="6d2de-117">Форцетуннел</span><span class="sxs-lookup"><span data-stu-id="6d2de-117">forceTunnel</span></span>|<span data-ttu-id="6d2de-118">2</span><span class="sxs-lookup"><span data-stu-id="6d2de-118">2</span></span>|<span data-ttu-id="6d2de-119">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="6d2de-119">All network traffic will be routed through the VPN.</span></span>|




