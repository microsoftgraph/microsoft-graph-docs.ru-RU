---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5782555214897ec0513ab7293adf1d877ec5f96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042424"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="a107e-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="a107e-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="a107e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a107e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a107e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a107e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a107e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a107e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a107e-107">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="a107e-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="a107e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a107e-108">Members</span></span>
|<span data-ttu-id="a107e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a107e-109">Member</span></span>|<span data-ttu-id="a107e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a107e-110">Value</span></span>|<span data-ttu-id="a107e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a107e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a107e-112">Нет</span><span class="sxs-lookup"><span data-stu-id="a107e-112">none</span></span>|<span data-ttu-id="a107e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a107e-113">0</span></span>|<span data-ttu-id="a107e-114">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="a107e-114">No routing policy specified.</span></span>|
|<span data-ttu-id="a107e-115">сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="a107e-115">splitTunnel</span></span>|<span data-ttu-id="a107e-116">1 </span><span class="sxs-lookup"><span data-stu-id="a107e-116">1</span></span>|<span data-ttu-id="a107e-117">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="a107e-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="a107e-118">форцетуннел</span><span class="sxs-lookup"><span data-stu-id="a107e-118">forceTunnel</span></span>|<span data-ttu-id="a107e-119">2 </span><span class="sxs-lookup"><span data-stu-id="a107e-119">2</span></span>|<span data-ttu-id="a107e-120">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="a107e-120">All network traffic will be routed through the VPN.</span></span>|






