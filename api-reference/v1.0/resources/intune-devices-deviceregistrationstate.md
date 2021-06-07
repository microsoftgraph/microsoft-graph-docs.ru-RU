---
title: тип enum deviceRegistrationState
description: Состояние регистрации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 39a4c68f2a688564284fc6045f61b84e72b748ab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751694"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="4c5f1-103">тип enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4c5f1-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="4c5f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c5f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c5f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c5f1-106">Состояние регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="4c5f1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4c5f1-107">Members</span></span>
|<span data-ttu-id="4c5f1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4c5f1-108">Member</span></span>|<span data-ttu-id="4c5f1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4c5f1-109">Value</span></span>|<span data-ttu-id="4c5f1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c5f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c5f1-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="4c5f1-111">notRegistered</span></span>|<span data-ttu-id="4c5f1-112">0</span><span class="sxs-lookup"><span data-stu-id="4c5f1-112">0</span></span>|<span data-ttu-id="4c5f1-113">Устройство не зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-113">The device is not registered.</span></span>|
|<span data-ttu-id="4c5f1-114">зарегистрирована</span><span class="sxs-lookup"><span data-stu-id="4c5f1-114">registered</span></span>|<span data-ttu-id="4c5f1-115">2</span><span class="sxs-lookup"><span data-stu-id="4c5f1-115">2</span></span>|<span data-ttu-id="4c5f1-116">Устройство зарегистрировано.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-116">The device is registered.</span></span>|
|<span data-ttu-id="4c5f1-117">отменено</span><span class="sxs-lookup"><span data-stu-id="4c5f1-117">revoked</span></span>|<span data-ttu-id="4c5f1-118">3</span><span class="sxs-lookup"><span data-stu-id="4c5f1-118">3</span></span>|<span data-ttu-id="4c5f1-119">Устройство было заблокировано, вытерто или отошедо.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="4c5f1-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="4c5f1-120">keyConflict</span></span>|<span data-ttu-id="4c5f1-121">4 </span><span class="sxs-lookup"><span data-stu-id="4c5f1-121">4</span></span>|<span data-ttu-id="4c5f1-122">У устройства есть ключевой конфликт.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="4c5f1-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="4c5f1-123">approvalPending</span></span>|<span data-ttu-id="4c5f1-124">5 </span><span class="sxs-lookup"><span data-stu-id="4c5f1-124">5</span></span>|<span data-ttu-id="4c5f1-125">Устройство находится на стадии утверждения.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-125">The device is pending approval.</span></span>|
|<span data-ttu-id="4c5f1-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="4c5f1-126">certificateReset</span></span>|<span data-ttu-id="4c5f1-127">6 </span><span class="sxs-lookup"><span data-stu-id="4c5f1-127">6</span></span>|<span data-ttu-id="4c5f1-128">Сертификат устройства был сброшен.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="4c5f1-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="4c5f1-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="4c5f1-130">7 </span><span class="sxs-lookup"><span data-stu-id="4c5f1-130">7</span></span>|<span data-ttu-id="4c5f1-131">Устройство не регистрируется и не ожидает регистрации.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="4c5f1-132">unknown</span><span class="sxs-lookup"><span data-stu-id="4c5f1-132">unknown</span></span>|<span data-ttu-id="4c5f1-133">8 </span><span class="sxs-lookup"><span data-stu-id="4c5f1-133">8</span></span>|<span data-ttu-id="4c5f1-134">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="4c5f1-134">The device registration status is unknown.</span></span>|




