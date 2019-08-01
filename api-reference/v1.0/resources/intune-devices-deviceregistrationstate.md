---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 933ea7cf16421ecadd9bb23b4594d8ca0f5e767b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030732"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="ef324-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ef324-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="ef324-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef324-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef324-105">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef324-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="ef324-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ef324-106">Members</span></span>
|<span data-ttu-id="ef324-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ef324-107">Member</span></span>|<span data-ttu-id="ef324-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ef324-108">Value</span></span>|<span data-ttu-id="ef324-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ef324-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef324-110">Нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="ef324-110">notRegistered</span></span>|<span data-ttu-id="ef324-111">нуль</span><span class="sxs-lookup"><span data-stu-id="ef324-111">0</span></span>|<span data-ttu-id="ef324-112">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="ef324-112">The device is not registered.</span></span>|
|<span data-ttu-id="ef324-113">охраняем</span><span class="sxs-lookup"><span data-stu-id="ef324-113">registered</span></span>|<span data-ttu-id="ef324-114">2</span><span class="sxs-lookup"><span data-stu-id="ef324-114">2</span></span>|<span data-ttu-id="ef324-115">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="ef324-115">The device is registered.</span></span>|
|<span data-ttu-id="ef324-116">отозван</span><span class="sxs-lookup"><span data-stu-id="ef324-116">revoked</span></span>|<span data-ttu-id="ef324-117">4</span><span class="sxs-lookup"><span data-stu-id="ef324-117">3</span></span>|<span data-ttu-id="ef324-118">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="ef324-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="ef324-119">Кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="ef324-119">keyConflict</span></span>|<span data-ttu-id="ef324-120">SP4</span><span class="sxs-lookup"><span data-stu-id="ef324-120">4</span></span>|<span data-ttu-id="ef324-121">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="ef324-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="ef324-122">Аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="ef324-122">approvalPending</span></span>|<span data-ttu-id="ef324-123">17:00</span><span class="sxs-lookup"><span data-stu-id="ef324-123">5</span></span>|<span data-ttu-id="ef324-124">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="ef324-124">The device is pending approval.</span></span>|
|<span data-ttu-id="ef324-125">Цертификатересет</span><span class="sxs-lookup"><span data-stu-id="ef324-125">certificateReset</span></span>|<span data-ttu-id="ef324-126">6 </span><span class="sxs-lookup"><span data-stu-id="ef324-126">6</span></span>|<span data-ttu-id="ef324-127">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="ef324-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="ef324-128">Нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="ef324-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="ef324-129">7 </span><span class="sxs-lookup"><span data-stu-id="ef324-129">7</span></span>|<span data-ttu-id="ef324-130">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="ef324-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="ef324-131">unknown</span><span class="sxs-lookup"><span data-stu-id="ef324-131">unknown</span></span>|<span data-ttu-id="ef324-132">8 </span><span class="sxs-lookup"><span data-stu-id="ef324-132">8</span></span>|<span data-ttu-id="ef324-133">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="ef324-133">The device registration status is unknown.</span></span>|



