---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f999e393caab410ea3f7565ade25d189193cfc40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525028"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="17fbf-103">тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="17fbf-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="17fbf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="17fbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17fbf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17fbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17fbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17fbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17fbf-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="17fbf-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="17fbf-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="17fbf-108">Members</span></span>
|<span data-ttu-id="17fbf-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="17fbf-109">Member</span></span>|<span data-ttu-id="17fbf-110">Значение</span><span class="sxs-lookup"><span data-stu-id="17fbf-110">Value</span></span>|<span data-ttu-id="17fbf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="17fbf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17fbf-112">нотрегистеред</span><span class="sxs-lookup"><span data-stu-id="17fbf-112">notRegistered</span></span>|<span data-ttu-id="17fbf-113">нуль</span><span class="sxs-lookup"><span data-stu-id="17fbf-113">0</span></span>|<span data-ttu-id="17fbf-114">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="17fbf-114">The device is not registered.</span></span>|
|<span data-ttu-id="17fbf-115">охраняем</span><span class="sxs-lookup"><span data-stu-id="17fbf-115">registered</span></span>|<span data-ttu-id="17fbf-116">2 </span><span class="sxs-lookup"><span data-stu-id="17fbf-116">2</span></span>|<span data-ttu-id="17fbf-117">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="17fbf-117">The device is registered.</span></span>|
|<span data-ttu-id="17fbf-118">отозван</span><span class="sxs-lookup"><span data-stu-id="17fbf-118">revoked</span></span>|<span data-ttu-id="17fbf-119">3 </span><span class="sxs-lookup"><span data-stu-id="17fbf-119">3</span></span>|<span data-ttu-id="17fbf-120">Устройство заблокировано, очищено или снято.</span><span class="sxs-lookup"><span data-stu-id="17fbf-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="17fbf-121">кэйконфликт</span><span class="sxs-lookup"><span data-stu-id="17fbf-121">keyConflict</span></span>|<span data-ttu-id="17fbf-122">4 </span><span class="sxs-lookup"><span data-stu-id="17fbf-122">4</span></span>|<span data-ttu-id="17fbf-123">У устройства есть конфликт ключей.</span><span class="sxs-lookup"><span data-stu-id="17fbf-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="17fbf-124">аппровалпендинг</span><span class="sxs-lookup"><span data-stu-id="17fbf-124">approvalPending</span></span>|<span data-ttu-id="17fbf-125">5 </span><span class="sxs-lookup"><span data-stu-id="17fbf-125">5</span></span>|<span data-ttu-id="17fbf-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="17fbf-126">The device is pending approval.</span></span>|
|<span data-ttu-id="17fbf-127">цертификатересет</span><span class="sxs-lookup"><span data-stu-id="17fbf-127">certificateReset</span></span>|<span data-ttu-id="17fbf-128">6 </span><span class="sxs-lookup"><span data-stu-id="17fbf-128">6</span></span>|<span data-ttu-id="17fbf-129">Сертификат устройства сброшен.</span><span class="sxs-lookup"><span data-stu-id="17fbf-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="17fbf-130">нотрегистередпендинженроллмент</span><span class="sxs-lookup"><span data-stu-id="17fbf-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="17fbf-131">7 </span><span class="sxs-lookup"><span data-stu-id="17fbf-131">7</span></span>|<span data-ttu-id="17fbf-132">Устройство не зарегистрировано и находится в состоянии ожидания регистрации.</span><span class="sxs-lookup"><span data-stu-id="17fbf-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="17fbf-133">unknown</span><span class="sxs-lookup"><span data-stu-id="17fbf-133">unknown</span></span>|<span data-ttu-id="17fbf-134">8 </span><span class="sxs-lookup"><span data-stu-id="17fbf-134">8</span></span>|<span data-ttu-id="17fbf-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="17fbf-135">The device registration status is unknown.</span></span>|



