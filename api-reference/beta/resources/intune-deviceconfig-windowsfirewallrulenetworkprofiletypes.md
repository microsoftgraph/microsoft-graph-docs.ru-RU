---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ab45603b91740ffbdef4379413a89c9fa21b929c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692375"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="83a61-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="83a61-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="83a61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83a61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83a61-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83a61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83a61-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83a61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83a61-107">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="83a61-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="83a61-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="83a61-108">Members</span></span>
|<span data-ttu-id="83a61-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="83a61-109">Member</span></span>|<span data-ttu-id="83a61-110">Значение</span><span class="sxs-lookup"><span data-stu-id="83a61-110">Value</span></span>|<span data-ttu-id="83a61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="83a61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83a61-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="83a61-112">notConfigured</span></span>|<span data-ttu-id="83a61-113">нуль</span><span class="sxs-lookup"><span data-stu-id="83a61-113">0</span></span>|<span data-ttu-id="83a61-114">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="83a61-114">No flags set.</span></span>|
|<span data-ttu-id="83a61-115">domain</span><span class="sxs-lookup"><span data-stu-id="83a61-115">domain</span></span>|<span data-ttu-id="83a61-116">1,1</span><span class="sxs-lookup"><span data-stu-id="83a61-116">1</span></span>|<span data-ttu-id="83a61-117">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="83a61-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="83a61-118">закрытый</span><span class="sxs-lookup"><span data-stu-id="83a61-118">private</span></span>|<span data-ttu-id="83a61-119">2</span><span class="sxs-lookup"><span data-stu-id="83a61-119">2</span></span>|<span data-ttu-id="83a61-120">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="83a61-120">The profile for private networks.</span></span>|
|<span data-ttu-id="83a61-121">public</span><span class="sxs-lookup"><span data-stu-id="83a61-121">public</span></span>|<span data-ttu-id="83a61-122">4 </span><span class="sxs-lookup"><span data-stu-id="83a61-122">4</span></span>|<span data-ttu-id="83a61-123">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="83a61-123">The profile for public networks.</span></span>|





