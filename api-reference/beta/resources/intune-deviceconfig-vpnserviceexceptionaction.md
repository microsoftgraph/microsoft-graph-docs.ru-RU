---
title: тип перечисления Впнсервицеексцептионактион
description: Действие VPN, выполняемое для определенной службы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba0ea4081ea958d4eb36d2506c4cc4cab5ef59a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985925"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="77043-103">тип перечисления Впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="77043-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="77043-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77043-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77043-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77043-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77043-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77043-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77043-107">Действие VPN, выполняемое для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="77043-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="77043-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="77043-108">Members</span></span>
|<span data-ttu-id="77043-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="77043-109">Member</span></span>|<span data-ttu-id="77043-110">Значение</span><span class="sxs-lookup"><span data-stu-id="77043-110">Value</span></span>|<span data-ttu-id="77043-111">Описание</span><span class="sxs-lookup"><span data-stu-id="77043-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77043-112">форцетраффиквиавпн</span><span class="sxs-lookup"><span data-stu-id="77043-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="77043-113">нуль</span><span class="sxs-lookup"><span data-stu-id="77043-113">0</span></span>|<span data-ttu-id="77043-114">Весь трафик, поступающий от этой службы, будет проходить через VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="77043-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="77043-115">алловтраффикаутсиде</span><span class="sxs-lookup"><span data-stu-id="77043-115">allowTrafficOutside</span></span>|<span data-ttu-id="77043-116">1 </span><span class="sxs-lookup"><span data-stu-id="77043-116">1</span></span>|<span data-ttu-id="77043-117">Разрешить службу вне сети VPN</span><span class="sxs-lookup"><span data-stu-id="77043-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="77043-118">дроптраффик</span><span class="sxs-lookup"><span data-stu-id="77043-118">dropTraffic</span></span>|<span data-ttu-id="77043-119">2 </span><span class="sxs-lookup"><span data-stu-id="77043-119">2</span></span>|<span data-ttu-id="77043-120">Удаление всего трафика из службы</span><span class="sxs-lookup"><span data-stu-id="77043-120">Drop all traffic from the service</span></span>|






