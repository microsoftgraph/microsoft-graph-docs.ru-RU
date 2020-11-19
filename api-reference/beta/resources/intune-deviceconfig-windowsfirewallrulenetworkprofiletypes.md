---
title: тип перечисления Виндовсфиреваллруленетворкпрофилетипес
description: Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e46fccf175483090bc78ae0c070112c7e3f18e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215333"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="d97d8-103">тип перечисления Виндовсфиреваллруленетворкпрофилетипес</span><span class="sxs-lookup"><span data-stu-id="d97d8-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="d97d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d97d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d97d8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d97d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d97d8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d97d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d97d8-107">Флаги, определяющие, какие типы профилей сети применяются к правилу брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="d97d8-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="d97d8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d97d8-108">Members</span></span>
|<span data-ttu-id="d97d8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d97d8-109">Member</span></span>|<span data-ttu-id="d97d8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d97d8-110">Value</span></span>|<span data-ttu-id="d97d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d97d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d97d8-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d97d8-112">notConfigured</span></span>|<span data-ttu-id="d97d8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d97d8-113">0</span></span>|<span data-ttu-id="d97d8-114">Флаги не заданы.</span><span class="sxs-lookup"><span data-stu-id="d97d8-114">No flags set.</span></span>|
|<span data-ttu-id="d97d8-115">domain</span><span class="sxs-lookup"><span data-stu-id="d97d8-115">domain</span></span>|<span data-ttu-id="d97d8-116">1,1</span><span class="sxs-lookup"><span data-stu-id="d97d8-116">1</span></span>|<span data-ttu-id="d97d8-117">Профиль для сетей, подключенных к доменам.</span><span class="sxs-lookup"><span data-stu-id="d97d8-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="d97d8-118">закрытый</span><span class="sxs-lookup"><span data-stu-id="d97d8-118">private</span></span>|<span data-ttu-id="d97d8-119">2</span><span class="sxs-lookup"><span data-stu-id="d97d8-119">2</span></span>|<span data-ttu-id="d97d8-120">Профиль для частных сетей.</span><span class="sxs-lookup"><span data-stu-id="d97d8-120">The profile for private networks.</span></span>|
|<span data-ttu-id="d97d8-121">public</span><span class="sxs-lookup"><span data-stu-id="d97d8-121">public</span></span>|<span data-ttu-id="d97d8-122">4 </span><span class="sxs-lookup"><span data-stu-id="d97d8-122">4</span></span>|<span data-ttu-id="d97d8-123">Профиль для общедоступных сетей.</span><span class="sxs-lookup"><span data-stu-id="d97d8-123">The profile for public networks.</span></span>|




