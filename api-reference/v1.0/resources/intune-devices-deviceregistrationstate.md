---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580976"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="70066-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="70066-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="70066-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70066-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70066-105">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="70066-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="70066-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="70066-106">Members</span></span>
|<span data-ttu-id="70066-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="70066-107">Member</span></span>|<span data-ttu-id="70066-108">Значение</span><span class="sxs-lookup"><span data-stu-id="70066-108">Value</span></span>|<span data-ttu-id="70066-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70066-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70066-110">Нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="70066-110">notRegistered</span></span>|<span data-ttu-id="70066-111">нуль</span><span class="sxs-lookup"><span data-stu-id="70066-111">0</span></span>|<span data-ttu-id="70066-112">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="70066-112">The device is not registered.</span></span>|
|<span data-ttu-id="70066-113">охраняем</span><span class="sxs-lookup"><span data-stu-id="70066-113">registered</span></span>|<span data-ttu-id="70066-114">2 </span><span class="sxs-lookup"><span data-stu-id="70066-114">2</span></span>|<span data-ttu-id="70066-115">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="70066-115">The device is registered.</span></span>|
|<span data-ttu-id="70066-116">отозван</span><span class="sxs-lookup"><span data-stu-id="70066-116">revoked</span></span>|<span data-ttu-id="70066-117">3 </span><span class="sxs-lookup"><span data-stu-id="70066-117">3</span></span>|<span data-ttu-id="70066-118">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="70066-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="70066-119">Кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="70066-119">keyConflict</span></span>|<span data-ttu-id="70066-120">4 </span><span class="sxs-lookup"><span data-stu-id="70066-120">4</span></span>|<span data-ttu-id="70066-121">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="70066-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="70066-122">Аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="70066-122">approvalPending</span></span>|<span data-ttu-id="70066-123">5 </span><span class="sxs-lookup"><span data-stu-id="70066-123">5</span></span>|<span data-ttu-id="70066-124">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="70066-124">The device is pending approval.</span></span>|
|<span data-ttu-id="70066-125">Цертификатересет</span><span class="sxs-lookup"><span data-stu-id="70066-125">certificateReset</span></span>|<span data-ttu-id="70066-126">6 </span><span class="sxs-lookup"><span data-stu-id="70066-126">6</span></span>|<span data-ttu-id="70066-127">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="70066-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="70066-128">Нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="70066-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="70066-129">7 </span><span class="sxs-lookup"><span data-stu-id="70066-129">7</span></span>|<span data-ttu-id="70066-130">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="70066-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="70066-131">unknown</span><span class="sxs-lookup"><span data-stu-id="70066-131">unknown</span></span>|<span data-ttu-id="70066-132">8 </span><span class="sxs-lookup"><span data-stu-id="70066-132">8</span></span>|<span data-ttu-id="70066-133">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="70066-133">The device registration status is unknown.</span></span>|



