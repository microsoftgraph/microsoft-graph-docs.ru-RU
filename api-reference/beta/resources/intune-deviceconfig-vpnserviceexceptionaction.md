---
title: тип перечисления Впнсервицеексцептионактион
description: Действие VPN, выполняемое для определенной службы.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b0c952a14db65e836c2a3391cb44a871957e708
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787308"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="d849c-103">тип перечисления Впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="d849c-103">vpnServiceExceptionAction enum type</span></span>

> <span data-ttu-id="d849c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d849c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d849c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d849c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d849c-106">Действие VPN, выполняемое для определенной службы.</span><span class="sxs-lookup"><span data-stu-id="d849c-106">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="d849c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d849c-107">Members</span></span>
|<span data-ttu-id="d849c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d849c-108">Member</span></span>|<span data-ttu-id="d849c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d849c-109">Value</span></span>|<span data-ttu-id="d849c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d849c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d849c-111">форцетраффиквиавпн</span><span class="sxs-lookup"><span data-stu-id="d849c-111">forceTrafficViaVPN</span></span>|<span data-ttu-id="d849c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d849c-112">0</span></span>|<span data-ttu-id="d849c-113">Весь трафик, поступающий от этой службы, будет проходить через VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="d849c-113">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="d849c-114">алловтраффикаутсиде</span><span class="sxs-lookup"><span data-stu-id="d849c-114">allowTrafficOutside</span></span>|<span data-ttu-id="d849c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d849c-115">1</span></span>|<span data-ttu-id="d849c-116">Разрешить службу вне сети VPN</span><span class="sxs-lookup"><span data-stu-id="d849c-116">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="d849c-117">дроптраффик</span><span class="sxs-lookup"><span data-stu-id="d849c-117">dropTraffic</span></span>|<span data-ttu-id="d849c-118">2</span><span class="sxs-lookup"><span data-stu-id="d849c-118">2</span></span>|<span data-ttu-id="d849c-119">Удаление всего трафика из службы</span><span class="sxs-lookup"><span data-stu-id="d849c-119">Drop all traffic from the service</span></span>|



