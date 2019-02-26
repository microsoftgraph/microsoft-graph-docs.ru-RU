---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04d8c0fddb966504675e3b4c677dfd0bbabe64c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144627"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="6710d-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6710d-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="6710d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6710d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6710d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6710d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6710d-106">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="6710d-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="6710d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6710d-107">Members</span></span>
|<span data-ttu-id="6710d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6710d-108">Member</span></span>|<span data-ttu-id="6710d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6710d-109">Value</span></span>|<span data-ttu-id="6710d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6710d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6710d-111">Нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="6710d-111">notRegistered</span></span>|<span data-ttu-id="6710d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6710d-112">0</span></span>|<span data-ttu-id="6710d-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="6710d-113">The device is not registered.</span></span>|
|<span data-ttu-id="6710d-114">охраняем</span><span class="sxs-lookup"><span data-stu-id="6710d-114">registered</span></span>|<span data-ttu-id="6710d-115">2</span><span class="sxs-lookup"><span data-stu-id="6710d-115">2</span></span>|<span data-ttu-id="6710d-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="6710d-116">The device is registered.</span></span>|
|<span data-ttu-id="6710d-117">отозван</span><span class="sxs-lookup"><span data-stu-id="6710d-117">revoked</span></span>|<span data-ttu-id="6710d-118">4</span><span class="sxs-lookup"><span data-stu-id="6710d-118">3</span></span>|<span data-ttu-id="6710d-119">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="6710d-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="6710d-120">Кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="6710d-120">keyConflict</span></span>|<span data-ttu-id="6710d-121">4</span><span class="sxs-lookup"><span data-stu-id="6710d-121">4</span></span>|<span data-ttu-id="6710d-122">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="6710d-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="6710d-123">Аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="6710d-123">approvalPending</span></span>|<span data-ttu-id="6710d-124">17:00</span><span class="sxs-lookup"><span data-stu-id="6710d-124">5</span></span>|<span data-ttu-id="6710d-125">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="6710d-125">The device is pending approval.</span></span>|
|<span data-ttu-id="6710d-126">Цертификатересет</span><span class="sxs-lookup"><span data-stu-id="6710d-126">certificateReset</span></span>|<span data-ttu-id="6710d-127">6</span><span class="sxs-lookup"><span data-stu-id="6710d-127">6</span></span>|<span data-ttu-id="6710d-128">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="6710d-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="6710d-129">Нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="6710d-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="6710d-130">7</span><span class="sxs-lookup"><span data-stu-id="6710d-130">7</span></span>|<span data-ttu-id="6710d-131">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="6710d-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="6710d-132">unknown</span><span class="sxs-lookup"><span data-stu-id="6710d-132">unknown</span></span>|<span data-ttu-id="6710d-133">8,5</span><span class="sxs-lookup"><span data-stu-id="6710d-133">8</span></span>|<span data-ttu-id="6710d-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="6710d-134">The device registration status is unknown.</span></span>|




