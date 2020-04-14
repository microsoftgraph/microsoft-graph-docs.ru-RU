---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb7e522159df19040fcc4da3870e76b7971c95c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470680"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="c1672-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c1672-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="c1672-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1672-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1672-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1672-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1672-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="c1672-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c1672-108">Members</span></span>
|<span data-ttu-id="c1672-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c1672-109">Member</span></span>|<span data-ttu-id="c1672-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c1672-110">Value</span></span>|<span data-ttu-id="c1672-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1672-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1672-112">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="c1672-112">notRegistered</span></span>|<span data-ttu-id="c1672-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c1672-113">0</span></span>|<span data-ttu-id="c1672-114">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="c1672-114">The device is not registered.</span></span>|
|<span data-ttu-id="c1672-115">охраняем</span><span class="sxs-lookup"><span data-stu-id="c1672-115">registered</span></span>|<span data-ttu-id="c1672-116">2</span><span class="sxs-lookup"><span data-stu-id="c1672-116">2</span></span>|<span data-ttu-id="c1672-117">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="c1672-117">The device is registered.</span></span>|
|<span data-ttu-id="c1672-118">отозван</span><span class="sxs-lookup"><span data-stu-id="c1672-118">revoked</span></span>|<span data-ttu-id="c1672-119">4</span><span class="sxs-lookup"><span data-stu-id="c1672-119">3</span></span>|<span data-ttu-id="c1672-120">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="c1672-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="c1672-121">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="c1672-121">keyConflict</span></span>|<span data-ttu-id="c1672-122">4 </span><span class="sxs-lookup"><span data-stu-id="c1672-122">4</span></span>|<span data-ttu-id="c1672-123">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="c1672-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="c1672-124">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="c1672-124">approvalPending</span></span>|<span data-ttu-id="c1672-125">5 </span><span class="sxs-lookup"><span data-stu-id="c1672-125">5</span></span>|<span data-ttu-id="c1672-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="c1672-126">The device is pending approval.</span></span>|
|<span data-ttu-id="c1672-127">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="c1672-127">certificateReset</span></span>|<span data-ttu-id="c1672-128">6 </span><span class="sxs-lookup"><span data-stu-id="c1672-128">6</span></span>|<span data-ttu-id="c1672-129">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="c1672-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="c1672-130">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="c1672-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="c1672-131">7 </span><span class="sxs-lookup"><span data-stu-id="c1672-131">7</span></span>|<span data-ttu-id="c1672-132">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="c1672-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="c1672-133">unknown</span><span class="sxs-lookup"><span data-stu-id="c1672-133">unknown</span></span>|<span data-ttu-id="c1672-134">8 </span><span class="sxs-lookup"><span data-stu-id="c1672-134">8</span></span>|<span data-ttu-id="c1672-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="c1672-135">The device registration status is unknown.</span></span>|



