---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 628d4c6c253349e54747d4fce836a2b4c8f4579f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081428"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="c0f8b-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c0f8b-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="c0f8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0f8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0f8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0f8b-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="c0f8b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c0f8b-108">Members</span></span>
|<span data-ttu-id="c0f8b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c0f8b-109">Member</span></span>|<span data-ttu-id="c0f8b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c0f8b-110">Value</span></span>|<span data-ttu-id="c0f8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f8b-112">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="c0f8b-112">notRegistered</span></span>|<span data-ttu-id="c0f8b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c0f8b-113">0</span></span>|<span data-ttu-id="c0f8b-114">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-114">The device is not registered.</span></span>|
|<span data-ttu-id="c0f8b-115">охраняем</span><span class="sxs-lookup"><span data-stu-id="c0f8b-115">registered</span></span>|<span data-ttu-id="c0f8b-116">2 </span><span class="sxs-lookup"><span data-stu-id="c0f8b-116">2</span></span>|<span data-ttu-id="c0f8b-117">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-117">The device is registered.</span></span>|
|<span data-ttu-id="c0f8b-118">отозван</span><span class="sxs-lookup"><span data-stu-id="c0f8b-118">revoked</span></span>|<span data-ttu-id="c0f8b-119">4</span><span class="sxs-lookup"><span data-stu-id="c0f8b-119">3</span></span>|<span data-ttu-id="c0f8b-120">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="c0f8b-121">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="c0f8b-121">keyConflict</span></span>|<span data-ttu-id="c0f8b-122">4 </span><span class="sxs-lookup"><span data-stu-id="c0f8b-122">4</span></span>|<span data-ttu-id="c0f8b-123">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="c0f8b-124">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="c0f8b-124">approvalPending</span></span>|<span data-ttu-id="c0f8b-125">5 </span><span class="sxs-lookup"><span data-stu-id="c0f8b-125">5</span></span>|<span data-ttu-id="c0f8b-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-126">The device is pending approval.</span></span>|
|<span data-ttu-id="c0f8b-127">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="c0f8b-127">certificateReset</span></span>|<span data-ttu-id="c0f8b-128">6 </span><span class="sxs-lookup"><span data-stu-id="c0f8b-128">6</span></span>|<span data-ttu-id="c0f8b-129">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="c0f8b-130">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="c0f8b-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="c0f8b-131">7 </span><span class="sxs-lookup"><span data-stu-id="c0f8b-131">7</span></span>|<span data-ttu-id="c0f8b-132">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="c0f8b-133">unknown</span><span class="sxs-lookup"><span data-stu-id="c0f8b-133">unknown</span></span>|<span data-ttu-id="c0f8b-134">8 </span><span class="sxs-lookup"><span data-stu-id="c0f8b-134">8</span></span>|<span data-ttu-id="c0f8b-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="c0f8b-135">The device registration status is unknown.</span></span>|






