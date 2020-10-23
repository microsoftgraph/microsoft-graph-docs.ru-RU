---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 030a1184fe9577a1a965ea65a90ad03f136858cc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697695"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="8ceb8-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="8ceb8-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="8ceb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ceb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ceb8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ceb8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ceb8-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="8ceb8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8ceb8-108">Members</span></span>
|<span data-ttu-id="8ceb8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8ceb8-109">Member</span></span>|<span data-ttu-id="8ceb8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8ceb8-110">Value</span></span>|<span data-ttu-id="8ceb8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ceb8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ceb8-112">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="8ceb8-112">notRegistered</span></span>|<span data-ttu-id="8ceb8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8ceb8-113">0</span></span>|<span data-ttu-id="8ceb8-114">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-114">The device is not registered.</span></span>|
|<span data-ttu-id="8ceb8-115">охраняем</span><span class="sxs-lookup"><span data-stu-id="8ceb8-115">registered</span></span>|<span data-ttu-id="8ceb8-116">2</span><span class="sxs-lookup"><span data-stu-id="8ceb8-116">2</span></span>|<span data-ttu-id="8ceb8-117">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-117">The device is registered.</span></span>|
|<span data-ttu-id="8ceb8-118">отозван</span><span class="sxs-lookup"><span data-stu-id="8ceb8-118">revoked</span></span>|<span data-ttu-id="8ceb8-119">4</span><span class="sxs-lookup"><span data-stu-id="8ceb8-119">3</span></span>|<span data-ttu-id="8ceb8-120">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="8ceb8-121">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="8ceb8-121">keyConflict</span></span>|<span data-ttu-id="8ceb8-122">4 </span><span class="sxs-lookup"><span data-stu-id="8ceb8-122">4</span></span>|<span data-ttu-id="8ceb8-123">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="8ceb8-124">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="8ceb8-124">approvalPending</span></span>|<span data-ttu-id="8ceb8-125">5 </span><span class="sxs-lookup"><span data-stu-id="8ceb8-125">5</span></span>|<span data-ttu-id="8ceb8-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-126">The device is pending approval.</span></span>|
|<span data-ttu-id="8ceb8-127">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="8ceb8-127">certificateReset</span></span>|<span data-ttu-id="8ceb8-128">6 </span><span class="sxs-lookup"><span data-stu-id="8ceb8-128">6</span></span>|<span data-ttu-id="8ceb8-129">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="8ceb8-130">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="8ceb8-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="8ceb8-131">7 </span><span class="sxs-lookup"><span data-stu-id="8ceb8-131">7</span></span>|<span data-ttu-id="8ceb8-132">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="8ceb8-133">unknown</span><span class="sxs-lookup"><span data-stu-id="8ceb8-133">unknown</span></span>|<span data-ttu-id="8ceb8-134">8 </span><span class="sxs-lookup"><span data-stu-id="8ceb8-134">8</span></span>|<span data-ttu-id="8ceb8-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="8ceb8-135">The device registration status is unknown.</span></span>|





