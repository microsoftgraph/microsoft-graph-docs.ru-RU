---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264136"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="f6173-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f6173-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="f6173-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6173-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6173-105">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6173-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="f6173-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="f6173-106">Members</span></span>
|<span data-ttu-id="f6173-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="f6173-107">Member</span></span>|<span data-ttu-id="f6173-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f6173-108">Value</span></span>|<span data-ttu-id="f6173-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f6173-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6173-110">Нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="f6173-110">notRegistered</span></span>|<span data-ttu-id="f6173-111">нуль</span><span class="sxs-lookup"><span data-stu-id="f6173-111">0</span></span>|<span data-ttu-id="f6173-112">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="f6173-112">The device is not registered.</span></span>|
|<span data-ttu-id="f6173-113">охраняем</span><span class="sxs-lookup"><span data-stu-id="f6173-113">registered</span></span>|<span data-ttu-id="f6173-114">2</span><span class="sxs-lookup"><span data-stu-id="f6173-114">2</span></span>|<span data-ttu-id="f6173-115">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="f6173-115">The device is registered.</span></span>|
|<span data-ttu-id="f6173-116">отозван</span><span class="sxs-lookup"><span data-stu-id="f6173-116">revoked</span></span>|<span data-ttu-id="f6173-117">4</span><span class="sxs-lookup"><span data-stu-id="f6173-117">3</span></span>|<span data-ttu-id="f6173-118">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="f6173-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="f6173-119">Кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="f6173-119">keyConflict</span></span>|<span data-ttu-id="f6173-120">4</span><span class="sxs-lookup"><span data-stu-id="f6173-120">4</span></span>|<span data-ttu-id="f6173-121">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="f6173-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="f6173-122">Аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="f6173-122">approvalPending</span></span>|<span data-ttu-id="f6173-123">17:00</span><span class="sxs-lookup"><span data-stu-id="f6173-123">5</span></span>|<span data-ttu-id="f6173-124">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="f6173-124">The device is pending approval.</span></span>|
|<span data-ttu-id="f6173-125">Цертификатересет</span><span class="sxs-lookup"><span data-stu-id="f6173-125">certificateReset</span></span>|<span data-ttu-id="f6173-126">6</span><span class="sxs-lookup"><span data-stu-id="f6173-126">6</span></span>|<span data-ttu-id="f6173-127">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="f6173-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="f6173-128">Нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="f6173-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="f6173-129">7</span><span class="sxs-lookup"><span data-stu-id="f6173-129">7</span></span>|<span data-ttu-id="f6173-130">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="f6173-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="f6173-131">unknown</span><span class="sxs-lookup"><span data-stu-id="f6173-131">unknown</span></span>|<span data-ttu-id="f6173-132">8,5</span><span class="sxs-lookup"><span data-stu-id="f6173-132">8</span></span>|<span data-ttu-id="f6173-133">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="f6173-133">The device registration status is unknown.</span></span>|



