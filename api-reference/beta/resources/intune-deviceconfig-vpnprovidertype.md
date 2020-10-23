---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f20433a7e2bbb0dd134471476fd96fe3e49b9ecd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728330"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="d62c4-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="d62c4-103">vpnProviderType enum type</span></span>

<span data-ttu-id="d62c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d62c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d62c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d62c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d62c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d62c4-107">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="d62c4-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="d62c4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d62c4-108">Members</span></span>
|<span data-ttu-id="d62c4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d62c4-109">Member</span></span>|<span data-ttu-id="d62c4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d62c4-110">Value</span></span>|<span data-ttu-id="d62c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d62c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d62c4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d62c4-112">notConfigured</span></span>|<span data-ttu-id="d62c4-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d62c4-113">0</span></span>|<span data-ttu-id="d62c4-114">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="d62c4-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="d62c4-115">апппрокси</span><span class="sxs-lookup"><span data-stu-id="d62c4-115">appProxy</span></span>|<span data-ttu-id="d62c4-116">1,1</span><span class="sxs-lookup"><span data-stu-id="d62c4-116">1</span></span>|<span data-ttu-id="d62c4-117">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="d62c4-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="d62c4-118">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="d62c4-118">packetTunnel</span></span>|<span data-ttu-id="d62c4-119">2</span><span class="sxs-lookup"><span data-stu-id="d62c4-119">2</span></span>|<span data-ttu-id="d62c4-120">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="d62c4-120">Tunnel traffic at the IP layer.</span></span>|





