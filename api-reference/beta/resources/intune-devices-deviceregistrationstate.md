---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794017"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="d572e-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d572e-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="d572e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d572e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d572e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d572e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d572e-106">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="d572e-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="d572e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d572e-107">Members</span></span>
|<span data-ttu-id="d572e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d572e-108">Member</span></span>|<span data-ttu-id="d572e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d572e-109">Value</span></span>|<span data-ttu-id="d572e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d572e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d572e-111">Нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="d572e-111">notRegistered</span></span>|<span data-ttu-id="d572e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d572e-112">0</span></span>|<span data-ttu-id="d572e-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="d572e-113">The device is not registered.</span></span>|
|<span data-ttu-id="d572e-114">охраняем</span><span class="sxs-lookup"><span data-stu-id="d572e-114">registered</span></span>|<span data-ttu-id="d572e-115">2</span><span class="sxs-lookup"><span data-stu-id="d572e-115">2</span></span>|<span data-ttu-id="d572e-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="d572e-116">The device is registered.</span></span>|
|<span data-ttu-id="d572e-117">отозван</span><span class="sxs-lookup"><span data-stu-id="d572e-117">revoked</span></span>|<span data-ttu-id="d572e-118">4</span><span class="sxs-lookup"><span data-stu-id="d572e-118">3</span></span>|<span data-ttu-id="d572e-119">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="d572e-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="d572e-120">Кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="d572e-120">keyConflict</span></span>|<span data-ttu-id="d572e-121">SP4</span><span class="sxs-lookup"><span data-stu-id="d572e-121">4</span></span>|<span data-ttu-id="d572e-122">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="d572e-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="d572e-123">Аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="d572e-123">approvalPending</span></span>|<span data-ttu-id="d572e-124">17:00</span><span class="sxs-lookup"><span data-stu-id="d572e-124">5</span></span>|<span data-ttu-id="d572e-125">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="d572e-125">The device is pending approval.</span></span>|
|<span data-ttu-id="d572e-126">Цертификатересет</span><span class="sxs-lookup"><span data-stu-id="d572e-126">certificateReset</span></span>|<span data-ttu-id="d572e-127">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="d572e-127">6</span></span>|<span data-ttu-id="d572e-128">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="d572e-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="d572e-129">Нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="d572e-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="d572e-130">см</span><span class="sxs-lookup"><span data-stu-id="d572e-130">7</span></span>|<span data-ttu-id="d572e-131">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="d572e-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="d572e-132">unknown</span><span class="sxs-lookup"><span data-stu-id="d572e-132">unknown</span></span>|<span data-ttu-id="d572e-133">8,5</span><span class="sxs-lookup"><span data-stu-id="d572e-133">8</span></span>|<span data-ttu-id="d572e-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="d572e-134">The device registration status is unknown.</span></span>|





