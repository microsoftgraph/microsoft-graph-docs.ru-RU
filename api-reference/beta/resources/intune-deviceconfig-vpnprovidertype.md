---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7455e6a3f3d9887a36dd49e9c66a207da950c785
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529301"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="4179c-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="4179c-103">vpnProviderType enum type</span></span>

<span data-ttu-id="4179c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4179c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4179c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4179c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4179c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4179c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4179c-107">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="4179c-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="4179c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4179c-108">Members</span></span>
|<span data-ttu-id="4179c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4179c-109">Member</span></span>|<span data-ttu-id="4179c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4179c-110">Value</span></span>|<span data-ttu-id="4179c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4179c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4179c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4179c-112">notConfigured</span></span>|<span data-ttu-id="4179c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4179c-113">0</span></span>|<span data-ttu-id="4179c-114">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="4179c-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="4179c-115">апппрокси</span><span class="sxs-lookup"><span data-stu-id="4179c-115">appProxy</span></span>|<span data-ttu-id="4179c-116">1 </span><span class="sxs-lookup"><span data-stu-id="4179c-116">1</span></span>|<span data-ttu-id="4179c-117">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="4179c-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="4179c-118">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="4179c-118">packetTunnel</span></span>|<span data-ttu-id="4179c-119">2 </span><span class="sxs-lookup"><span data-stu-id="4179c-119">2</span></span>|<span data-ttu-id="4179c-120">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="4179c-120">Tunnel traffic at the IP layer.</span></span>|



