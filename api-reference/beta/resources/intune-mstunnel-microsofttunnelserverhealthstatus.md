---
title: тип перечисления Микрософттуннелсерверхеалсстатус
description: Перечисление возможных типов состояния работоспособности Микрософттуннелсервер
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5c9c00812d0b1e4e3173c981cdaa92c9c0bafec2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302020"
---
# <a name="microsofttunnelserverhealthstatus-enum-type"></a><span data-ttu-id="3daed-103">тип перечисления Микрософттуннелсерверхеалсстатус</span><span class="sxs-lookup"><span data-stu-id="3daed-103">microsoftTunnelServerHealthStatus enum type</span></span>

<span data-ttu-id="3daed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3daed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3daed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3daed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3daed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3daed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3daed-107">Перечисление возможных типов состояния работоспособности Микрософттуннелсервер</span><span class="sxs-lookup"><span data-stu-id="3daed-107">Enum of possible MicrosoftTunnelServer health status types</span></span>

## <a name="members"></a><span data-ttu-id="3daed-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3daed-108">Members</span></span>
|<span data-ttu-id="3daed-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3daed-109">Member</span></span>|<span data-ttu-id="3daed-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3daed-110">Value</span></span>|<span data-ttu-id="3daed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3daed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3daed-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3daed-112">unknown</span></span>|<span data-ttu-id="3daed-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3daed-113">0</span></span>|<span data-ttu-id="3daed-114">Состояние неизвестно</span><span class="sxs-lookup"><span data-stu-id="3daed-114">The state is unknown</span></span>|
|<span data-ttu-id="3daed-115">рабочее</span><span class="sxs-lookup"><span data-stu-id="3daed-115">healthy</span></span>|<span data-ttu-id="3daed-116">1,1</span><span class="sxs-lookup"><span data-stu-id="3daed-116">1</span></span>|<span data-ttu-id="3daed-117">Состояние является работоспособным</span><span class="sxs-lookup"><span data-stu-id="3daed-117">The state is healthy</span></span>|
|<span data-ttu-id="3daed-118">неисправности</span><span class="sxs-lookup"><span data-stu-id="3daed-118">unhealthy</span></span>|<span data-ttu-id="3daed-119">2</span><span class="sxs-lookup"><span data-stu-id="3daed-119">2</span></span>|<span data-ttu-id="3daed-120">Неисправность состояния</span><span class="sxs-lookup"><span data-stu-id="3daed-120">The state is unhealthy</span></span>|
|<span data-ttu-id="3daed-121">warning</span><span class="sxs-lookup"><span data-stu-id="3daed-121">warning</span></span>|<span data-ttu-id="3daed-122">4</span><span class="sxs-lookup"><span data-stu-id="3daed-122">3</span></span>|<span data-ttu-id="3daed-123">Состояние — предупреждение</span><span class="sxs-lookup"><span data-stu-id="3daed-123">The state is warning</span></span>|
|<span data-ttu-id="3daed-124">содержание</span><span class="sxs-lookup"><span data-stu-id="3daed-124">offline</span></span>|<span data-ttu-id="3daed-125">4 </span><span class="sxs-lookup"><span data-stu-id="3daed-125">4</span></span>|<span data-ttu-id="3daed-126">Состояние находится в автономном режиме</span><span class="sxs-lookup"><span data-stu-id="3daed-126">The state is offline</span></span>|
|<span data-ttu-id="3daed-127">упградеинпрогресс</span><span class="sxs-lookup"><span data-stu-id="3daed-127">upgradeInProgress</span></span>|<span data-ttu-id="3daed-128">5 </span><span class="sxs-lookup"><span data-stu-id="3daed-128">5</span></span>|<span data-ttu-id="3daed-129">Состояние — Упградеинпрогресс</span><span class="sxs-lookup"><span data-stu-id="3daed-129">The state is upgradeInProgress</span></span>|
|<span data-ttu-id="3daed-130">упградефаилед</span><span class="sxs-lookup"><span data-stu-id="3daed-130">upgradeFailed</span></span>|<span data-ttu-id="3daed-131">6 </span><span class="sxs-lookup"><span data-stu-id="3daed-131">6</span></span>|<span data-ttu-id="3daed-132">Состояние — Упградефаилед</span><span class="sxs-lookup"><span data-stu-id="3daed-132">The state is upgradeFailed</span></span>|




