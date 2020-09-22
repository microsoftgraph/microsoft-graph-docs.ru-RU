---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 43b962235cda6622ca0d7d10d7da57f9f5181471
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048997"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="71418-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="71418-103">vpnProviderType enum type</span></span>

<span data-ttu-id="71418-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71418-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71418-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71418-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71418-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71418-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71418-107">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="71418-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="71418-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="71418-108">Members</span></span>
|<span data-ttu-id="71418-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="71418-109">Member</span></span>|<span data-ttu-id="71418-110">Значение</span><span class="sxs-lookup"><span data-stu-id="71418-110">Value</span></span>|<span data-ttu-id="71418-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71418-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71418-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="71418-112">notConfigured</span></span>|<span data-ttu-id="71418-113">нуль</span><span class="sxs-lookup"><span data-stu-id="71418-113">0</span></span>|<span data-ttu-id="71418-114">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="71418-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="71418-115">апппрокси</span><span class="sxs-lookup"><span data-stu-id="71418-115">appProxy</span></span>|<span data-ttu-id="71418-116">1 </span><span class="sxs-lookup"><span data-stu-id="71418-116">1</span></span>|<span data-ttu-id="71418-117">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="71418-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="71418-118">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="71418-118">packetTunnel</span></span>|<span data-ttu-id="71418-119">2 </span><span class="sxs-lookup"><span data-stu-id="71418-119">2</span></span>|<span data-ttu-id="71418-120">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="71418-120">Tunnel traffic at the IP layer.</span></span>|






