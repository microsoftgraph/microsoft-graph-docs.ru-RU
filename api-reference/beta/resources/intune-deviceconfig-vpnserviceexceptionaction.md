---
title: тип перечисления Впнсервицеексцептионактион
description: Действие VPN, выполняемое для определенной службы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1310d91da9a7ea8e3a6274acd48e8ebc1359cafd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636716"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="f12f1-103">тип перечисления Впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="f12f1-103">vpnServiceExceptionAction enum type</span></span>

> <span data-ttu-id="f12f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f12f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f12f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f12f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f12f1-106">Действие VPN, выполняемое для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="f12f1-106">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="f12f1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f12f1-107">Members</span></span>
|<span data-ttu-id="f12f1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f12f1-108">Member</span></span>|<span data-ttu-id="f12f1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f12f1-109">Value</span></span>|<span data-ttu-id="f12f1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f12f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f12f1-111">форцетраффиквиавпн</span><span class="sxs-lookup"><span data-stu-id="f12f1-111">forceTrafficViaVPN</span></span>|<span data-ttu-id="f12f1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f12f1-112">0</span></span>|<span data-ttu-id="f12f1-113">Весь трафик, поступающий от этой службы, будет проходить через VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f12f1-113">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="f12f1-114">алловтраффикаутсиде</span><span class="sxs-lookup"><span data-stu-id="f12f1-114">allowTrafficOutside</span></span>|<span data-ttu-id="f12f1-115">1 </span><span class="sxs-lookup"><span data-stu-id="f12f1-115">1</span></span>|<span data-ttu-id="f12f1-116">Разрешить службу вне сети VPN</span><span class="sxs-lookup"><span data-stu-id="f12f1-116">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="f12f1-117">дроптраффик</span><span class="sxs-lookup"><span data-stu-id="f12f1-117">dropTraffic</span></span>|<span data-ttu-id="f12f1-118">2 </span><span class="sxs-lookup"><span data-stu-id="f12f1-118">2</span></span>|<span data-ttu-id="f12f1-119">Удаление всего трафика из службы</span><span class="sxs-lookup"><span data-stu-id="f12f1-119">Drop all traffic from the service</span></span>|



