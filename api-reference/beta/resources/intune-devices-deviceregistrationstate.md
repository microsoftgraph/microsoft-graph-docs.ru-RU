---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908f38a2da8f5960eb9c5f1879b7b54374b806ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784135"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="ed645-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ed645-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="ed645-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed645-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed645-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed645-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed645-106">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed645-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="ed645-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ed645-107">Members</span></span>
|<span data-ttu-id="ed645-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ed645-108">Member</span></span>|<span data-ttu-id="ed645-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ed645-109">Value</span></span>|<span data-ttu-id="ed645-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed645-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed645-111">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="ed645-111">notRegistered</span></span>|<span data-ttu-id="ed645-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ed645-112">0</span></span>|<span data-ttu-id="ed645-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="ed645-113">The device is not registered.</span></span>|
|<span data-ttu-id="ed645-114">охраняем</span><span class="sxs-lookup"><span data-stu-id="ed645-114">registered</span></span>|<span data-ttu-id="ed645-115">2</span><span class="sxs-lookup"><span data-stu-id="ed645-115">2</span></span>|<span data-ttu-id="ed645-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="ed645-116">The device is registered.</span></span>|
|<span data-ttu-id="ed645-117">отозван</span><span class="sxs-lookup"><span data-stu-id="ed645-117">revoked</span></span>|<span data-ttu-id="ed645-118">4</span><span class="sxs-lookup"><span data-stu-id="ed645-118">3</span></span>|<span data-ttu-id="ed645-119">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="ed645-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="ed645-120">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="ed645-120">keyConflict</span></span>|<span data-ttu-id="ed645-121">4 </span><span class="sxs-lookup"><span data-stu-id="ed645-121">4</span></span>|<span data-ttu-id="ed645-122">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="ed645-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="ed645-123">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="ed645-123">approvalPending</span></span>|<span data-ttu-id="ed645-124">5 </span><span class="sxs-lookup"><span data-stu-id="ed645-124">5</span></span>|<span data-ttu-id="ed645-125">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="ed645-125">The device is pending approval.</span></span>|
|<span data-ttu-id="ed645-126">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="ed645-126">certificateReset</span></span>|<span data-ttu-id="ed645-127">6 </span><span class="sxs-lookup"><span data-stu-id="ed645-127">6</span></span>|<span data-ttu-id="ed645-128">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="ed645-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="ed645-129">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="ed645-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="ed645-130">7 </span><span class="sxs-lookup"><span data-stu-id="ed645-130">7</span></span>|<span data-ttu-id="ed645-131">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="ed645-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="ed645-132">unknown</span><span class="sxs-lookup"><span data-stu-id="ed645-132">unknown</span></span>|<span data-ttu-id="ed645-133">8 </span><span class="sxs-lookup"><span data-stu-id="ed645-133">8</span></span>|<span data-ttu-id="ed645-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="ed645-134">The device registration status is unknown.</span></span>|



