---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4d2a7a10936df83300c432ea9412790ba33ccc1c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786490"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="abb17-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="abb17-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="abb17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abb17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abb17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abb17-106">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="abb17-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="abb17-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="abb17-107">Members</span></span>
|<span data-ttu-id="abb17-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="abb17-108">Member</span></span>|<span data-ttu-id="abb17-109">Значение</span><span class="sxs-lookup"><span data-stu-id="abb17-109">Value</span></span>|<span data-ttu-id="abb17-110">Описание</span><span class="sxs-lookup"><span data-stu-id="abb17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abb17-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="abb17-111">notConfigured</span></span>|<span data-ttu-id="abb17-112">нуль</span><span class="sxs-lookup"><span data-stu-id="abb17-112">0</span></span>|<span data-ttu-id="abb17-113">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="abb17-113">No flags set.</span></span>|
|<span data-ttu-id="abb17-114">domain</span><span class="sxs-lookup"><span data-stu-id="abb17-114">domain</span></span>|<span data-ttu-id="abb17-115">1,1</span><span class="sxs-lookup"><span data-stu-id="abb17-115">1</span></span>|<span data-ttu-id="abb17-116">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="abb17-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="abb17-117">закрытый</span><span class="sxs-lookup"><span data-stu-id="abb17-117">private</span></span>|<span data-ttu-id="abb17-118">2</span><span class="sxs-lookup"><span data-stu-id="abb17-118">2</span></span>|<span data-ttu-id="abb17-119">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="abb17-119">The profile for private networks.</span></span>|
|<span data-ttu-id="abb17-120">public</span><span class="sxs-lookup"><span data-stu-id="abb17-120">public</span></span>|<span data-ttu-id="abb17-121">4 </span><span class="sxs-lookup"><span data-stu-id="abb17-121">4</span></span>|<span data-ttu-id="abb17-122">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="abb17-122">The profile for public networks.</span></span>|



