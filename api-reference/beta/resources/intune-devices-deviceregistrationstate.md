---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396758"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="dc8b8-103">Тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="dc8b8-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="dc8b8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dc8b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc8b8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc8b8-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="dc8b8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dc8b8-108">Members</span></span>
|<span data-ttu-id="dc8b8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dc8b8-109">Member</span></span>|<span data-ttu-id="dc8b8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dc8b8-110">Value</span></span>|<span data-ttu-id="dc8b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc8b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc8b8-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="dc8b8-112">notRegistered</span></span>|<span data-ttu-id="dc8b8-113">0</span><span class="sxs-lookup"><span data-stu-id="dc8b8-113">0</span></span>|<span data-ttu-id="dc8b8-114">Устройство не зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-114">The device is not registered.</span></span>|
|<span data-ttu-id="dc8b8-115">зарегистрирована</span><span class="sxs-lookup"><span data-stu-id="dc8b8-115">registered</span></span>|<span data-ttu-id="dc8b8-116">2</span><span class="sxs-lookup"><span data-stu-id="dc8b8-116">2</span></span>|<span data-ttu-id="dc8b8-117">Зарегистрированные устройства.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-117">The device is registered.</span></span>|
|<span data-ttu-id="dc8b8-118">отменено</span><span class="sxs-lookup"><span data-stu-id="dc8b8-118">revoked</span></span>|<span data-ttu-id="dc8b8-119">3</span><span class="sxs-lookup"><span data-stu-id="dc8b8-119">3</span></span>|<span data-ttu-id="dc8b8-120">Устройства был заблокирован, очистить или не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="dc8b8-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="dc8b8-121">keyConflict</span></span>|<span data-ttu-id="dc8b8-122">4</span><span class="sxs-lookup"><span data-stu-id="dc8b8-122">4</span></span>|<span data-ttu-id="dc8b8-123">Устройство имеет конфликты ключа.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="dc8b8-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="dc8b8-124">approvalPending</span></span>|<span data-ttu-id="dc8b8-125">5</span><span class="sxs-lookup"><span data-stu-id="dc8b8-125">5</span></span>|<span data-ttu-id="dc8b8-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-126">The device is pending approval.</span></span>|
|<span data-ttu-id="dc8b8-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="dc8b8-127">certificateReset</span></span>|<span data-ttu-id="dc8b8-128">6</span><span class="sxs-lookup"><span data-stu-id="dc8b8-128">6</span></span>|<span data-ttu-id="dc8b8-129">Устройство сертификат был изменен.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="dc8b8-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="dc8b8-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="dc8b8-131">7</span><span class="sxs-lookup"><span data-stu-id="dc8b8-131">7</span></span>|<span data-ttu-id="dc8b8-132">Устройства не зарегистрирована и ожидающие заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="dc8b8-133">unknown</span><span class="sxs-lookup"><span data-stu-id="dc8b8-133">unknown</span></span>|<span data-ttu-id="dc8b8-134">8</span><span class="sxs-lookup"><span data-stu-id="dc8b8-134">8</span></span>|<span data-ttu-id="dc8b8-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="dc8b8-135">The device registration status is unknown.</span></span>|




