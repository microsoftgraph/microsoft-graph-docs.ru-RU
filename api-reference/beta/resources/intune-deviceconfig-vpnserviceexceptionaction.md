---
title: тип перечисления Впнсервицеексцептионактион
description: Действие VPN, выполняемое для определенной службы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a7c202c404d9d1db16e328f9c7d4c220ddd481e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525742"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="8d49d-103">тип перечисления Впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="8d49d-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="8d49d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8d49d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d49d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d49d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d49d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d49d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d49d-107">Действие VPN, выполняемое для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="8d49d-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="8d49d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8d49d-108">Members</span></span>
|<span data-ttu-id="8d49d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8d49d-109">Member</span></span>|<span data-ttu-id="8d49d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8d49d-110">Value</span></span>|<span data-ttu-id="8d49d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d49d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d49d-112">форцетраффиквиавпн</span><span class="sxs-lookup"><span data-stu-id="8d49d-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="8d49d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8d49d-113">0</span></span>|<span data-ttu-id="8d49d-114">Весь трафик, поступающий от этой службы, будет проходить через VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="8d49d-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="8d49d-115">алловтраффикаутсиде</span><span class="sxs-lookup"><span data-stu-id="8d49d-115">allowTrafficOutside</span></span>|<span data-ttu-id="8d49d-116">1 </span><span class="sxs-lookup"><span data-stu-id="8d49d-116">1</span></span>|<span data-ttu-id="8d49d-117">Разрешить службу вне сети VPN</span><span class="sxs-lookup"><span data-stu-id="8d49d-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="8d49d-118">дроптраффик</span><span class="sxs-lookup"><span data-stu-id="8d49d-118">dropTraffic</span></span>|<span data-ttu-id="8d49d-119">2 </span><span class="sxs-lookup"><span data-stu-id="8d49d-119">2</span></span>|<span data-ttu-id="8d49d-120">Удаление всего трафика из службы</span><span class="sxs-lookup"><span data-stu-id="8d49d-120">Drop all traffic from the service</span></span>|



