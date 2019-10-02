---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2543f1a7d874a8443424fa1161187e7ccd771f7b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356921"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="98e12-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="98e12-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="98e12-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98e12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98e12-105">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="98e12-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="98e12-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="98e12-106">Members</span></span>
|<span data-ttu-id="98e12-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="98e12-107">Member</span></span>|<span data-ttu-id="98e12-108">Значение</span><span class="sxs-lookup"><span data-stu-id="98e12-108">Value</span></span>|<span data-ttu-id="98e12-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98e12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98e12-110">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="98e12-110">notRegistered</span></span>|<span data-ttu-id="98e12-111">нуль</span><span class="sxs-lookup"><span data-stu-id="98e12-111">0</span></span>|<span data-ttu-id="98e12-112">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="98e12-112">The device is not registered.</span></span>|
|<span data-ttu-id="98e12-113">охраняем</span><span class="sxs-lookup"><span data-stu-id="98e12-113">registered</span></span>|<span data-ttu-id="98e12-114">2</span><span class="sxs-lookup"><span data-stu-id="98e12-114">2</span></span>|<span data-ttu-id="98e12-115">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="98e12-115">The device is registered.</span></span>|
|<span data-ttu-id="98e12-116">отозван</span><span class="sxs-lookup"><span data-stu-id="98e12-116">revoked</span></span>|<span data-ttu-id="98e12-117">4</span><span class="sxs-lookup"><span data-stu-id="98e12-117">3</span></span>|<span data-ttu-id="98e12-118">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="98e12-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="98e12-119">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="98e12-119">keyConflict</span></span>|<span data-ttu-id="98e12-120">SP4</span><span class="sxs-lookup"><span data-stu-id="98e12-120">4</span></span>|<span data-ttu-id="98e12-121">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="98e12-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="98e12-122">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="98e12-122">approvalPending</span></span>|<span data-ttu-id="98e12-123">17:00</span><span class="sxs-lookup"><span data-stu-id="98e12-123">5</span></span>|<span data-ttu-id="98e12-124">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="98e12-124">The device is pending approval.</span></span>|
|<span data-ttu-id="98e12-125">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="98e12-125">certificateReset</span></span>|<span data-ttu-id="98e12-126">6 </span><span class="sxs-lookup"><span data-stu-id="98e12-126">6</span></span>|<span data-ttu-id="98e12-127">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="98e12-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="98e12-128">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="98e12-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="98e12-129">7 </span><span class="sxs-lookup"><span data-stu-id="98e12-129">7</span></span>|<span data-ttu-id="98e12-130">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="98e12-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="98e12-131">unknown</span><span class="sxs-lookup"><span data-stu-id="98e12-131">unknown</span></span>|<span data-ttu-id="98e12-132">8 </span><span class="sxs-lookup"><span data-stu-id="98e12-132">8</span></span>|<span data-ttu-id="98e12-133">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="98e12-133">The device registration status is unknown.</span></span>|




