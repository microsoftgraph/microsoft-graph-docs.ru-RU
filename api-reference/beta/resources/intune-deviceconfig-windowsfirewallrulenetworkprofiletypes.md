---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cd5c501c50f74e53c0c00fcef2d3bb8a85cedf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570126"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="f1a91-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="f1a91-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="f1a91-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a91-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1a91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a91-106">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="f1a91-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="f1a91-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f1a91-107">Members</span></span>
|<span data-ttu-id="f1a91-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f1a91-108">Member</span></span>|<span data-ttu-id="f1a91-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a91-109">Value</span></span>|<span data-ttu-id="f1a91-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a91-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a91-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f1a91-111">notConfigured</span></span>|<span data-ttu-id="f1a91-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f1a91-112">0</span></span>|<span data-ttu-id="f1a91-113">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="f1a91-113">No flags set.</span></span>|
|<span data-ttu-id="f1a91-114">domain</span><span class="sxs-lookup"><span data-stu-id="f1a91-114">domain</span></span>|<span data-ttu-id="f1a91-115">1 </span><span class="sxs-lookup"><span data-stu-id="f1a91-115">1</span></span>|<span data-ttu-id="f1a91-116">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="f1a91-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="f1a91-117">закрытый</span><span class="sxs-lookup"><span data-stu-id="f1a91-117">private</span></span>|<span data-ttu-id="f1a91-118">2 </span><span class="sxs-lookup"><span data-stu-id="f1a91-118">2</span></span>|<span data-ttu-id="f1a91-119">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="f1a91-119">The profile for private networks.</span></span>|
|<span data-ttu-id="f1a91-120">public</span><span class="sxs-lookup"><span data-stu-id="f1a91-120">public</span></span>|<span data-ttu-id="f1a91-121">4 </span><span class="sxs-lookup"><span data-stu-id="f1a91-121">4</span></span>|<span data-ttu-id="f1a91-122">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="f1a91-122">The profile for public networks.</span></span>|





