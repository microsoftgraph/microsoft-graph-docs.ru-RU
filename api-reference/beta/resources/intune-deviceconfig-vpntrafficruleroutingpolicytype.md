---
title: тип перечисления Впнтраффикрулераутингполицитипе
description: Задает политику маршрутизации для правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cbbba22017a40ae2f7db41e25f497c09156a2f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969375"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="f93eb-103">тип перечисления Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="f93eb-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="f93eb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f93eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f93eb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f93eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f93eb-106">Задает политику маршрутизации для правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="f93eb-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="f93eb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f93eb-107">Members</span></span>
|<span data-ttu-id="f93eb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f93eb-108">Member</span></span>|<span data-ttu-id="f93eb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f93eb-109">Value</span></span>|<span data-ttu-id="f93eb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f93eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93eb-111">none</span><span class="sxs-lookup"><span data-stu-id="f93eb-111">none</span></span>|<span data-ttu-id="f93eb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f93eb-112">0</span></span>|<span data-ttu-id="f93eb-113">Политика маршрутизации не указана.</span><span class="sxs-lookup"><span data-stu-id="f93eb-113">No routing policy specified.</span></span>|
|<span data-ttu-id="f93eb-114">Сплиттуннел</span><span class="sxs-lookup"><span data-stu-id="f93eb-114">splitTunnel</span></span>|<span data-ttu-id="f93eb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="f93eb-115">1</span></span>|<span data-ttu-id="f93eb-116">Сетевой трафик для указанного приложения будет перенаправлен через VPN.</span><span class="sxs-lookup"><span data-stu-id="f93eb-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="f93eb-117">Форцетуннел</span><span class="sxs-lookup"><span data-stu-id="f93eb-117">forceTunnel</span></span>|<span data-ttu-id="f93eb-118">2</span><span class="sxs-lookup"><span data-stu-id="f93eb-118">2</span></span>|<span data-ttu-id="f93eb-119">Весь сетевой трафик будет маршрутизироваться через VPN.</span><span class="sxs-lookup"><span data-stu-id="f93eb-119">All network traffic will be routed through the VPN.</span></span>|





