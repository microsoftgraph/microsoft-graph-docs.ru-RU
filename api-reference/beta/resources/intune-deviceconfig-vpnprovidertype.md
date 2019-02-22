---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a62436f56a210bbb71606ebb8f2586e5b48f8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163191"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="9d7f2-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="9d7f2-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="9d7f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d7f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d7f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d7f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d7f2-106">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="9d7f2-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="9d7f2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9d7f2-107">Members</span></span>
|<span data-ttu-id="9d7f2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9d7f2-108">Member</span></span>|<span data-ttu-id="9d7f2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9d7f2-109">Value</span></span>|<span data-ttu-id="9d7f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d7f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d7f2-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9d7f2-111">notConfigured</span></span>|<span data-ttu-id="9d7f2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9d7f2-112">0</span></span>|<span data-ttu-id="9d7f2-113">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="9d7f2-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="9d7f2-114">Апппрокси</span><span class="sxs-lookup"><span data-stu-id="9d7f2-114">appProxy</span></span>|<span data-ttu-id="9d7f2-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9d7f2-115">1</span></span>|<span data-ttu-id="9d7f2-116">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="9d7f2-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="9d7f2-117">Паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="9d7f2-117">packetTunnel</span></span>|<span data-ttu-id="9d7f2-118">2</span><span class="sxs-lookup"><span data-stu-id="9d7f2-118">2</span></span>|<span data-ttu-id="9d7f2-119">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="9d7f2-119">Tunnel traffic at the IP layer.</span></span>|




