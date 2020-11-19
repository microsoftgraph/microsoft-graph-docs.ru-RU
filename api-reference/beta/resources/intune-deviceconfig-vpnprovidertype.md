---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb29fc6a77eb6db051279cdeb630dbf4104aa9af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279579"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="186ed-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="186ed-103">vpnProviderType enum type</span></span>

<span data-ttu-id="186ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="186ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="186ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="186ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="186ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="186ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="186ed-107">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="186ed-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="186ed-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="186ed-108">Members</span></span>
|<span data-ttu-id="186ed-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="186ed-109">Member</span></span>|<span data-ttu-id="186ed-110">Значение</span><span class="sxs-lookup"><span data-stu-id="186ed-110">Value</span></span>|<span data-ttu-id="186ed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="186ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186ed-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="186ed-112">notConfigured</span></span>|<span data-ttu-id="186ed-113">нуль</span><span class="sxs-lookup"><span data-stu-id="186ed-113">0</span></span>|<span data-ttu-id="186ed-114">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="186ed-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="186ed-115">апппрокси</span><span class="sxs-lookup"><span data-stu-id="186ed-115">appProxy</span></span>|<span data-ttu-id="186ed-116">1,1</span><span class="sxs-lookup"><span data-stu-id="186ed-116">1</span></span>|<span data-ttu-id="186ed-117">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="186ed-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="186ed-118">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="186ed-118">packetTunnel</span></span>|<span data-ttu-id="186ed-119">2</span><span class="sxs-lookup"><span data-stu-id="186ed-119">2</span></span>|<span data-ttu-id="186ed-120">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="186ed-120">Tunnel traffic at the IP layer.</span></span>|




