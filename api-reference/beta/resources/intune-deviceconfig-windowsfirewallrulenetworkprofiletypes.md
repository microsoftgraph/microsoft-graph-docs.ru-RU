---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0562f36f46d3ae54621de61d1117144d91624d5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039939"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="278b0-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="278b0-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="278b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="278b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="278b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="278b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="278b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="278b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="278b0-107">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="278b0-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="278b0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="278b0-108">Members</span></span>
|<span data-ttu-id="278b0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="278b0-109">Member</span></span>|<span data-ttu-id="278b0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="278b0-110">Value</span></span>|<span data-ttu-id="278b0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="278b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="278b0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="278b0-112">notConfigured</span></span>|<span data-ttu-id="278b0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="278b0-113">0</span></span>|<span data-ttu-id="278b0-114">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="278b0-114">No flags set.</span></span>|
|<span data-ttu-id="278b0-115">domain</span><span class="sxs-lookup"><span data-stu-id="278b0-115">domain</span></span>|<span data-ttu-id="278b0-116">1 </span><span class="sxs-lookup"><span data-stu-id="278b0-116">1</span></span>|<span data-ttu-id="278b0-117">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="278b0-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="278b0-118">закрытый</span><span class="sxs-lookup"><span data-stu-id="278b0-118">private</span></span>|<span data-ttu-id="278b0-119">2 </span><span class="sxs-lookup"><span data-stu-id="278b0-119">2</span></span>|<span data-ttu-id="278b0-120">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="278b0-120">The profile for private networks.</span></span>|
|<span data-ttu-id="278b0-121">public</span><span class="sxs-lookup"><span data-stu-id="278b0-121">public</span></span>|<span data-ttu-id="278b0-122">4 </span><span class="sxs-lookup"><span data-stu-id="278b0-122">4</span></span>|<span data-ttu-id="278b0-123">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="278b0-123">The profile for public networks.</span></span>|






