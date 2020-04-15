---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b1974d8124c834185617332096d6b44429c7900a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472425"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="2d0ad-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="2d0ad-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="2d0ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d0ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d0ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d0ad-106">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="2d0ad-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d0ad-107">Members</span></span>
|<span data-ttu-id="2d0ad-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d0ad-108">Member</span></span>|<span data-ttu-id="2d0ad-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2d0ad-109">Value</span></span>|<span data-ttu-id="2d0ad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d0ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d0ad-111">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="2d0ad-111">notRegistered</span></span>|<span data-ttu-id="2d0ad-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2d0ad-112">0</span></span>|<span data-ttu-id="2d0ad-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-113">The device is not registered.</span></span>|
|<span data-ttu-id="2d0ad-114">охраняем</span><span class="sxs-lookup"><span data-stu-id="2d0ad-114">registered</span></span>|<span data-ttu-id="2d0ad-115">2</span><span class="sxs-lookup"><span data-stu-id="2d0ad-115">2</span></span>|<span data-ttu-id="2d0ad-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-116">The device is registered.</span></span>|
|<span data-ttu-id="2d0ad-117">отозван</span><span class="sxs-lookup"><span data-stu-id="2d0ad-117">revoked</span></span>|<span data-ttu-id="2d0ad-118">4</span><span class="sxs-lookup"><span data-stu-id="2d0ad-118">3</span></span>|<span data-ttu-id="2d0ad-119">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="2d0ad-120">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="2d0ad-120">keyConflict</span></span>|<span data-ttu-id="2d0ad-121">4 </span><span class="sxs-lookup"><span data-stu-id="2d0ad-121">4</span></span>|<span data-ttu-id="2d0ad-122">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="2d0ad-123">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="2d0ad-123">approvalPending</span></span>|<span data-ttu-id="2d0ad-124">5 </span><span class="sxs-lookup"><span data-stu-id="2d0ad-124">5</span></span>|<span data-ttu-id="2d0ad-125">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-125">The device is pending approval.</span></span>|
|<span data-ttu-id="2d0ad-126">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="2d0ad-126">certificateReset</span></span>|<span data-ttu-id="2d0ad-127">6 </span><span class="sxs-lookup"><span data-stu-id="2d0ad-127">6</span></span>|<span data-ttu-id="2d0ad-128">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="2d0ad-129">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="2d0ad-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="2d0ad-130">7 </span><span class="sxs-lookup"><span data-stu-id="2d0ad-130">7</span></span>|<span data-ttu-id="2d0ad-131">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="2d0ad-132">unknown</span><span class="sxs-lookup"><span data-stu-id="2d0ad-132">unknown</span></span>|<span data-ttu-id="2d0ad-133">8 </span><span class="sxs-lookup"><span data-stu-id="2d0ad-133">8</span></span>|<span data-ttu-id="2d0ad-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="2d0ad-134">The device registration status is unknown.</span></span>|







