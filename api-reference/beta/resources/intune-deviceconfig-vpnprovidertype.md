---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b064c86413d84a06884de9728ccfa9cb83d61d2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787350"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="1769a-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="1769a-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="1769a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1769a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1769a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1769a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1769a-106">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="1769a-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="1769a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1769a-107">Members</span></span>
|<span data-ttu-id="1769a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1769a-108">Member</span></span>|<span data-ttu-id="1769a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1769a-109">Value</span></span>|<span data-ttu-id="1769a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1769a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1769a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1769a-111">notConfigured</span></span>|<span data-ttu-id="1769a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1769a-112">0</span></span>|<span data-ttu-id="1769a-113">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="1769a-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="1769a-114">апппрокси</span><span class="sxs-lookup"><span data-stu-id="1769a-114">appProxy</span></span>|<span data-ttu-id="1769a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1769a-115">1</span></span>|<span data-ttu-id="1769a-116">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="1769a-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="1769a-117">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="1769a-117">packetTunnel</span></span>|<span data-ttu-id="1769a-118">2</span><span class="sxs-lookup"><span data-stu-id="1769a-118">2</span></span>|<span data-ttu-id="1769a-119">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="1769a-119">Tunnel traffic at the IP layer.</span></span>|



