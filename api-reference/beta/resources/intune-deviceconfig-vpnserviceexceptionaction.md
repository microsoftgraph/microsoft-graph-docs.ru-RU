---
title: тип перечисления Впнсервицеексцептионактион
description: Действие VPN, выполняемое для определенной службы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 079342d93ea96add59885079b4c6448145dbbe37
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736228"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="927f9-103">тип перечисления Впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="927f9-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="927f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="927f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="927f9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="927f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="927f9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="927f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="927f9-107">Действие VPN, выполняемое для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="927f9-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="927f9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="927f9-108">Members</span></span>
|<span data-ttu-id="927f9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="927f9-109">Member</span></span>|<span data-ttu-id="927f9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="927f9-110">Value</span></span>|<span data-ttu-id="927f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="927f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="927f9-112">форцетраффиквиавпн</span><span class="sxs-lookup"><span data-stu-id="927f9-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="927f9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="927f9-113">0</span></span>|<span data-ttu-id="927f9-114">Весь трафик, поступающий от этой службы, будет проходить через VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="927f9-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="927f9-115">алловтраффикаутсиде</span><span class="sxs-lookup"><span data-stu-id="927f9-115">allowTrafficOutside</span></span>|<span data-ttu-id="927f9-116">1,1</span><span class="sxs-lookup"><span data-stu-id="927f9-116">1</span></span>|<span data-ttu-id="927f9-117">Разрешить службу вне сети VPN</span><span class="sxs-lookup"><span data-stu-id="927f9-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="927f9-118">дроптраффик</span><span class="sxs-lookup"><span data-stu-id="927f9-118">dropTraffic</span></span>|<span data-ttu-id="927f9-119">2</span><span class="sxs-lookup"><span data-stu-id="927f9-119">2</span></span>|<span data-ttu-id="927f9-120">Удаление всего трафика из службы</span><span class="sxs-lookup"><span data-stu-id="927f9-120">Drop all traffic from the service</span></span>|





