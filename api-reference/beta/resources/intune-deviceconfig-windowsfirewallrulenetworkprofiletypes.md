---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c7e0f50a830134cea6b4bfc15c6e68b49b86d0a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371084"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="9d473-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="9d473-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="9d473-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d473-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d473-106">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="9d473-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="9d473-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9d473-107">Members</span></span>
|<span data-ttu-id="9d473-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9d473-108">Member</span></span>|<span data-ttu-id="9d473-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9d473-109">Value</span></span>|<span data-ttu-id="9d473-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d473-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d473-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9d473-111">notConfigured</span></span>|<span data-ttu-id="9d473-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9d473-112">0</span></span>|<span data-ttu-id="9d473-113">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="9d473-113">No flags set.</span></span>|
|<span data-ttu-id="9d473-114">domain</span><span class="sxs-lookup"><span data-stu-id="9d473-114">domain</span></span>|<span data-ttu-id="9d473-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9d473-115">1</span></span>|<span data-ttu-id="9d473-116">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="9d473-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="9d473-117">закрытый</span><span class="sxs-lookup"><span data-stu-id="9d473-117">private</span></span>|<span data-ttu-id="9d473-118">2</span><span class="sxs-lookup"><span data-stu-id="9d473-118">2</span></span>|<span data-ttu-id="9d473-119">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="9d473-119">The profile for private networks.</span></span>|
|<span data-ttu-id="9d473-120">public</span><span class="sxs-lookup"><span data-stu-id="9d473-120">public</span></span>|<span data-ttu-id="9d473-121">SP4</span><span class="sxs-lookup"><span data-stu-id="9d473-121">4</span></span>|<span data-ttu-id="9d473-122">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="9d473-122">The profile for public networks.</span></span>|



