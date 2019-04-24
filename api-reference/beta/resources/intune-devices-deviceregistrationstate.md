---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522386"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="5a742-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5a742-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="5a742-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a742-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a742-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a742-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a742-106">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a742-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="5a742-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5a742-107">Members</span></span>
|<span data-ttu-id="5a742-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5a742-108">Member</span></span>|<span data-ttu-id="5a742-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5a742-109">Value</span></span>|<span data-ttu-id="5a742-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a742-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a742-111">Нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="5a742-111">notRegistered</span></span>|<span data-ttu-id="5a742-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5a742-112">0</span></span>|<span data-ttu-id="5a742-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="5a742-113">The device is not registered.</span></span>|
|<span data-ttu-id="5a742-114">охраняем</span><span class="sxs-lookup"><span data-stu-id="5a742-114">registered</span></span>|<span data-ttu-id="5a742-115">2 </span><span class="sxs-lookup"><span data-stu-id="5a742-115">2</span></span>|<span data-ttu-id="5a742-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="5a742-116">The device is registered.</span></span>|
|<span data-ttu-id="5a742-117">отозван</span><span class="sxs-lookup"><span data-stu-id="5a742-117">revoked</span></span>|<span data-ttu-id="5a742-118">3 </span><span class="sxs-lookup"><span data-stu-id="5a742-118">3</span></span>|<span data-ttu-id="5a742-119">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="5a742-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="5a742-120">Кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="5a742-120">keyConflict</span></span>|<span data-ttu-id="5a742-121">4 </span><span class="sxs-lookup"><span data-stu-id="5a742-121">4</span></span>|<span data-ttu-id="5a742-122">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="5a742-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="5a742-123">Аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="5a742-123">approvalPending</span></span>|<span data-ttu-id="5a742-124">5 </span><span class="sxs-lookup"><span data-stu-id="5a742-124">5</span></span>|<span data-ttu-id="5a742-125">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="5a742-125">The device is pending approval.</span></span>|
|<span data-ttu-id="5a742-126">Цертификатересет</span><span class="sxs-lookup"><span data-stu-id="5a742-126">certificateReset</span></span>|<span data-ttu-id="5a742-127">6 </span><span class="sxs-lookup"><span data-stu-id="5a742-127">6</span></span>|<span data-ttu-id="5a742-128">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="5a742-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="5a742-129">Нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="5a742-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="5a742-130">7 </span><span class="sxs-lookup"><span data-stu-id="5a742-130">7</span></span>|<span data-ttu-id="5a742-131">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="5a742-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="5a742-132">unknown</span><span class="sxs-lookup"><span data-stu-id="5a742-132">unknown</span></span>|<span data-ttu-id="5a742-133">8 </span><span class="sxs-lookup"><span data-stu-id="5a742-133">8</span></span>|<span data-ttu-id="5a742-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="5a742-134">The device registration status is unknown.</span></span>|





