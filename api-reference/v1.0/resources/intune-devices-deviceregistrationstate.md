---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89be71ded6aa970a5b1b598fe75488423b2b7de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532203"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a7ef9-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a7ef9-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="a7ef9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7ef9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7ef9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7ef9-106">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="a7ef9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a7ef9-107">Members</span></span>
|<span data-ttu-id="a7ef9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a7ef9-108">Member</span></span>|<span data-ttu-id="a7ef9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a7ef9-109">Value</span></span>|<span data-ttu-id="a7ef9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ef9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7ef9-111">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="a7ef9-111">notRegistered</span></span>|<span data-ttu-id="a7ef9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a7ef9-112">0</span></span>|<span data-ttu-id="a7ef9-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-113">The device is not registered.</span></span>|
|<span data-ttu-id="a7ef9-114">охраняем</span><span class="sxs-lookup"><span data-stu-id="a7ef9-114">registered</span></span>|<span data-ttu-id="a7ef9-115">2 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-115">2</span></span>|<span data-ttu-id="a7ef9-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-116">The device is registered.</span></span>|
|<span data-ttu-id="a7ef9-117">отозван</span><span class="sxs-lookup"><span data-stu-id="a7ef9-117">revoked</span></span>|<span data-ttu-id="a7ef9-118">3 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-118">3</span></span>|<span data-ttu-id="a7ef9-119">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a7ef9-120">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="a7ef9-120">keyConflict</span></span>|<span data-ttu-id="a7ef9-121">4 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-121">4</span></span>|<span data-ttu-id="a7ef9-122">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="a7ef9-123">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="a7ef9-123">approvalPending</span></span>|<span data-ttu-id="a7ef9-124">5 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-124">5</span></span>|<span data-ttu-id="a7ef9-125">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-125">The device is pending approval.</span></span>|
|<span data-ttu-id="a7ef9-126">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="a7ef9-126">certificateReset</span></span>|<span data-ttu-id="a7ef9-127">6 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-127">6</span></span>|<span data-ttu-id="a7ef9-128">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a7ef9-129">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="a7ef9-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a7ef9-130">7 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-130">7</span></span>|<span data-ttu-id="a7ef9-131">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a7ef9-132">unknown</span><span class="sxs-lookup"><span data-stu-id="a7ef9-132">unknown</span></span>|<span data-ttu-id="a7ef9-133">8 </span><span class="sxs-lookup"><span data-stu-id="a7ef9-133">8</span></span>|<span data-ttu-id="a7ef9-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="a7ef9-134">The device registration status is unknown.</span></span>|




