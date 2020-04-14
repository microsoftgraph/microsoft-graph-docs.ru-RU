---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e0d1a24d1da6d34ae501e08e0460d98f1969d03
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383245"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="1517d-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="1517d-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="1517d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1517d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1517d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1517d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1517d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1517d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1517d-107">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="1517d-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="1517d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1517d-108">Members</span></span>
|<span data-ttu-id="1517d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1517d-109">Member</span></span>|<span data-ttu-id="1517d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1517d-110">Value</span></span>|<span data-ttu-id="1517d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1517d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1517d-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1517d-112">notConfigured</span></span>|<span data-ttu-id="1517d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1517d-113">0</span></span>|<span data-ttu-id="1517d-114">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="1517d-114">No flags set.</span></span>|
|<span data-ttu-id="1517d-115">domain</span><span class="sxs-lookup"><span data-stu-id="1517d-115">domain</span></span>|<span data-ttu-id="1517d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="1517d-116">1</span></span>|<span data-ttu-id="1517d-117">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="1517d-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="1517d-118">закрытый</span><span class="sxs-lookup"><span data-stu-id="1517d-118">private</span></span>|<span data-ttu-id="1517d-119">2</span><span class="sxs-lookup"><span data-stu-id="1517d-119">2</span></span>|<span data-ttu-id="1517d-120">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="1517d-120">The profile for private networks.</span></span>|
|<span data-ttu-id="1517d-121">public</span><span class="sxs-lookup"><span data-stu-id="1517d-121">public</span></span>|<span data-ttu-id="1517d-122">4 </span><span class="sxs-lookup"><span data-stu-id="1517d-122">4</span></span>|<span data-ttu-id="1517d-123">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="1517d-123">The profile for public networks.</span></span>|



