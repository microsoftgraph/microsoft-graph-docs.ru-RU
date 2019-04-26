---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e47f4d20cb843b62928c6c66e468d00f5a4f743
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561917"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="2ddab-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="2ddab-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="2ddab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ddab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ddab-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ddab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ddab-106">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="2ddab-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="2ddab-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2ddab-107">Members</span></span>
|<span data-ttu-id="2ddab-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2ddab-108">Member</span></span>|<span data-ttu-id="2ddab-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2ddab-109">Value</span></span>|<span data-ttu-id="2ddab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ddab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ddab-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2ddab-111">notConfigured</span></span>|<span data-ttu-id="2ddab-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2ddab-112">0</span></span>|<span data-ttu-id="2ddab-113">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="2ddab-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="2ddab-114">Апппрокси</span><span class="sxs-lookup"><span data-stu-id="2ddab-114">appProxy</span></span>|<span data-ttu-id="2ddab-115">1 </span><span class="sxs-lookup"><span data-stu-id="2ddab-115">1</span></span>|<span data-ttu-id="2ddab-116">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="2ddab-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="2ddab-117">Паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="2ddab-117">packetTunnel</span></span>|<span data-ttu-id="2ddab-118">2 </span><span class="sxs-lookup"><span data-stu-id="2ddab-118">2</span></span>|<span data-ttu-id="2ddab-119">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="2ddab-119">Tunnel traffic at the IP layer.</span></span>|





