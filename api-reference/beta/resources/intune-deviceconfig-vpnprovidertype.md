---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df2fffa2c18ff21f342b2de0fdd8d7cd0d60ca64
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944553"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="bf0f3-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="bf0f3-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="bf0f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf0f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf0f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf0f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf0f3-106">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="bf0f3-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="bf0f3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf0f3-107">Members</span></span>
|<span data-ttu-id="bf0f3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf0f3-108">Member</span></span>|<span data-ttu-id="bf0f3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bf0f3-109">Value</span></span>|<span data-ttu-id="bf0f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf0f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf0f3-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bf0f3-111">notConfigured</span></span>|<span data-ttu-id="bf0f3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bf0f3-112">0</span></span>|<span data-ttu-id="bf0f3-113">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="bf0f3-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="bf0f3-114">Апппрокси</span><span class="sxs-lookup"><span data-stu-id="bf0f3-114">appProxy</span></span>|<span data-ttu-id="bf0f3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bf0f3-115">1</span></span>|<span data-ttu-id="bf0f3-116">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="bf0f3-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="bf0f3-117">Паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="bf0f3-117">packetTunnel</span></span>|<span data-ttu-id="bf0f3-118">2</span><span class="sxs-lookup"><span data-stu-id="bf0f3-118">2</span></span>|<span data-ttu-id="bf0f3-119">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="bf0f3-119">Tunnel traffic at the IP layer.</span></span>|




