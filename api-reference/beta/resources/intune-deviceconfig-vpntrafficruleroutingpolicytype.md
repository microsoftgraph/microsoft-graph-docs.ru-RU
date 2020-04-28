---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f7e28ef548ec11f14db4913020f1b17fc25f5c6e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358996"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="78e90-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="78e90-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="78e90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78e90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78e90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78e90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e90-107">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="78e90-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="78e90-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="78e90-108">Members</span></span>
|<span data-ttu-id="78e90-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="78e90-109">Member</span></span>|<span data-ttu-id="78e90-110">Значение</span><span class="sxs-lookup"><span data-stu-id="78e90-110">Value</span></span>|<span data-ttu-id="78e90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78e90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e90-112">Нет</span><span class="sxs-lookup"><span data-stu-id="78e90-112">none</span></span>|<span data-ttu-id="78e90-113">нуль</span><span class="sxs-lookup"><span data-stu-id="78e90-113">0</span></span>|<span data-ttu-id="78e90-114">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="78e90-114">No routing policy specified.</span></span>|
|<span data-ttu-id="78e90-115">сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="78e90-115">splitTunnel</span></span>|<span data-ttu-id="78e90-116">1,1</span><span class="sxs-lookup"><span data-stu-id="78e90-116">1</span></span>|<span data-ttu-id="78e90-117">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="78e90-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="78e90-118">форцетуннел</span><span class="sxs-lookup"><span data-stu-id="78e90-118">forceTunnel</span></span>|<span data-ttu-id="78e90-119">2</span><span class="sxs-lookup"><span data-stu-id="78e90-119">2</span></span>|<span data-ttu-id="78e90-120">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="78e90-120">All network traffic will be routed through the VPN.</span></span>|



