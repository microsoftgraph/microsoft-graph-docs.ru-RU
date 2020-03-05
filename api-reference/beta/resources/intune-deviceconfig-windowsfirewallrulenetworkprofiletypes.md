---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0d57b5e52261ac720090921003665b05dd467ad1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525553"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="1218e-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="1218e-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="1218e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1218e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1218e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1218e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1218e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1218e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1218e-107">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="1218e-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="1218e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1218e-108">Members</span></span>
|<span data-ttu-id="1218e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1218e-109">Member</span></span>|<span data-ttu-id="1218e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1218e-110">Value</span></span>|<span data-ttu-id="1218e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1218e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1218e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1218e-112">notConfigured</span></span>|<span data-ttu-id="1218e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1218e-113">0</span></span>|<span data-ttu-id="1218e-114">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="1218e-114">No flags set.</span></span>|
|<span data-ttu-id="1218e-115">domain</span><span class="sxs-lookup"><span data-stu-id="1218e-115">domain</span></span>|<span data-ttu-id="1218e-116">1 </span><span class="sxs-lookup"><span data-stu-id="1218e-116">1</span></span>|<span data-ttu-id="1218e-117">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="1218e-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="1218e-118">закрытый</span><span class="sxs-lookup"><span data-stu-id="1218e-118">private</span></span>|<span data-ttu-id="1218e-119">2 </span><span class="sxs-lookup"><span data-stu-id="1218e-119">2</span></span>|<span data-ttu-id="1218e-120">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="1218e-120">The profile for private networks.</span></span>|
|<span data-ttu-id="1218e-121">public</span><span class="sxs-lookup"><span data-stu-id="1218e-121">public</span></span>|<span data-ttu-id="1218e-122">4 </span><span class="sxs-lookup"><span data-stu-id="1218e-122">4</span></span>|<span data-ttu-id="1218e-123">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="1218e-123">The profile for public networks.</span></span>|



