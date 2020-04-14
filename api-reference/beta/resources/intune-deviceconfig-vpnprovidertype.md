---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2809f0297ba952d1c302bc0597ab3e00bb33ab95
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412040"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="52ca9-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="52ca9-103">vpnProviderType enum type</span></span>

<span data-ttu-id="52ca9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52ca9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52ca9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52ca9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52ca9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52ca9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52ca9-107">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="52ca9-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="52ca9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="52ca9-108">Members</span></span>
|<span data-ttu-id="52ca9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="52ca9-109">Member</span></span>|<span data-ttu-id="52ca9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="52ca9-110">Value</span></span>|<span data-ttu-id="52ca9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52ca9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52ca9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="52ca9-112">notConfigured</span></span>|<span data-ttu-id="52ca9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="52ca9-113">0</span></span>|<span data-ttu-id="52ca9-114">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="52ca9-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="52ca9-115">апппрокси</span><span class="sxs-lookup"><span data-stu-id="52ca9-115">appProxy</span></span>|<span data-ttu-id="52ca9-116">1,1</span><span class="sxs-lookup"><span data-stu-id="52ca9-116">1</span></span>|<span data-ttu-id="52ca9-117">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="52ca9-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="52ca9-118">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="52ca9-118">packetTunnel</span></span>|<span data-ttu-id="52ca9-119">2</span><span class="sxs-lookup"><span data-stu-id="52ca9-119">2</span></span>|<span data-ttu-id="52ca9-120">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="52ca9-120">Tunnel traffic at the IP layer.</span></span>|



