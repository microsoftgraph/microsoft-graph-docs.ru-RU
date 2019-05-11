---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8df940a3389d742224a2eca2c215135e751297
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944056"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="558d3-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="558d3-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="558d3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="558d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="558d3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="558d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="558d3-106">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="558d3-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="558d3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="558d3-107">Members</span></span>
|<span data-ttu-id="558d3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="558d3-108">Member</span></span>|<span data-ttu-id="558d3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="558d3-109">Value</span></span>|<span data-ttu-id="558d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="558d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558d3-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="558d3-111">notConfigured</span></span>|<span data-ttu-id="558d3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="558d3-112">0</span></span>|<span data-ttu-id="558d3-113">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="558d3-113">No flags set.</span></span>|
|<span data-ttu-id="558d3-114">domain</span><span class="sxs-lookup"><span data-stu-id="558d3-114">domain</span></span>|<span data-ttu-id="558d3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="558d3-115">1</span></span>|<span data-ttu-id="558d3-116">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="558d3-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="558d3-117">закрытый</span><span class="sxs-lookup"><span data-stu-id="558d3-117">private</span></span>|<span data-ttu-id="558d3-118">2</span><span class="sxs-lookup"><span data-stu-id="558d3-118">2</span></span>|<span data-ttu-id="558d3-119">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="558d3-119">The profile for private networks.</span></span>|
|<span data-ttu-id="558d3-120">public</span><span class="sxs-lookup"><span data-stu-id="558d3-120">public</span></span>|<span data-ttu-id="558d3-121">SP4</span><span class="sxs-lookup"><span data-stu-id="558d3-121">4</span></span>|<span data-ttu-id="558d3-122">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="558d3-122">The profile for public networks.</span></span>|




