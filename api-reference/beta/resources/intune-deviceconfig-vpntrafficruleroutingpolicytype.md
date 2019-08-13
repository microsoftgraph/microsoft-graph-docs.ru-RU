---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 529c42722d8ce3827bb9daa4c0f158cfd92d8383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367521"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="d7446-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="d7446-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="d7446-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7446-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7446-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7446-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7446-106">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="d7446-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="d7446-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d7446-107">Members</span></span>
|<span data-ttu-id="d7446-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d7446-108">Member</span></span>|<span data-ttu-id="d7446-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d7446-109">Value</span></span>|<span data-ttu-id="d7446-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d7446-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7446-111">none</span><span class="sxs-lookup"><span data-stu-id="d7446-111">none</span></span>|<span data-ttu-id="d7446-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d7446-112">0</span></span>|<span data-ttu-id="d7446-113">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="d7446-113">No routing policy specified.</span></span>|
|<span data-ttu-id="d7446-114">сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="d7446-114">splitTunnel</span></span>|<span data-ttu-id="d7446-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d7446-115">1</span></span>|<span data-ttu-id="d7446-116">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="d7446-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="d7446-117">форцетуннел</span><span class="sxs-lookup"><span data-stu-id="d7446-117">forceTunnel</span></span>|<span data-ttu-id="d7446-118">2</span><span class="sxs-lookup"><span data-stu-id="d7446-118">2</span></span>|<span data-ttu-id="d7446-119">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="d7446-119">All network traffic will be routed through the VPN.</span></span>|



