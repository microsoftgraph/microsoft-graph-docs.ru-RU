---
title: тип перечисления Впнсервицеексцептионактион
description: Действие VPN, выполняемое для определенной службы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 069b7dc910a7c4ce9e281235aefc52b498519351
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279439"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="1af11-103">тип перечисления Впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="1af11-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="1af11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1af11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1af11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1af11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1af11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af11-107">Действие VPN, выполняемое для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="1af11-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="1af11-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1af11-108">Members</span></span>
|<span data-ttu-id="1af11-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1af11-109">Member</span></span>|<span data-ttu-id="1af11-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1af11-110">Value</span></span>|<span data-ttu-id="1af11-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1af11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af11-112">форцетраффиквиавпн</span><span class="sxs-lookup"><span data-stu-id="1af11-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="1af11-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1af11-113">0</span></span>|<span data-ttu-id="1af11-114">Весь трафик, поступающий от этой службы, будет проходить через VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="1af11-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="1af11-115">алловтраффикаутсиде</span><span class="sxs-lookup"><span data-stu-id="1af11-115">allowTrafficOutside</span></span>|<span data-ttu-id="1af11-116">1,1</span><span class="sxs-lookup"><span data-stu-id="1af11-116">1</span></span>|<span data-ttu-id="1af11-117">Разрешить службу вне сети VPN</span><span class="sxs-lookup"><span data-stu-id="1af11-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="1af11-118">дроптраффик</span><span class="sxs-lookup"><span data-stu-id="1af11-118">dropTraffic</span></span>|<span data-ttu-id="1af11-119">2</span><span class="sxs-lookup"><span data-stu-id="1af11-119">2</span></span>|<span data-ttu-id="1af11-120">Удаление всего трафика из службы</span><span class="sxs-lookup"><span data-stu-id="1af11-120">Drop all traffic from the service</span></span>|




