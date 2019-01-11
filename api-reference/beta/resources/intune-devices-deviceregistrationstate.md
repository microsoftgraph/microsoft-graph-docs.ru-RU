---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7633419ebeeb5c5865cd1a80c251effbf314b018
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829766"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="5668a-103">Тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5668a-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="5668a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5668a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5668a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5668a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5668a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5668a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5668a-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="5668a-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="5668a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5668a-108">Members</span></span>
|<span data-ttu-id="5668a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5668a-109">Member</span></span>|<span data-ttu-id="5668a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5668a-110">Value</span></span>|<span data-ttu-id="5668a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5668a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5668a-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="5668a-112">notRegistered</span></span>|<span data-ttu-id="5668a-113">0</span><span class="sxs-lookup"><span data-stu-id="5668a-113">0</span></span>|<span data-ttu-id="5668a-114">Устройство не зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="5668a-114">The device is not registered.</span></span>|
|<span data-ttu-id="5668a-115">зарегистрирована</span><span class="sxs-lookup"><span data-stu-id="5668a-115">registered</span></span>|<span data-ttu-id="5668a-116">2</span><span class="sxs-lookup"><span data-stu-id="5668a-116">2</span></span>|<span data-ttu-id="5668a-117">Зарегистрированные устройства.</span><span class="sxs-lookup"><span data-stu-id="5668a-117">The device is registered.</span></span>|
|<span data-ttu-id="5668a-118">отменено</span><span class="sxs-lookup"><span data-stu-id="5668a-118">revoked</span></span>|<span data-ttu-id="5668a-119">3</span><span class="sxs-lookup"><span data-stu-id="5668a-119">3</span></span>|<span data-ttu-id="5668a-120">Устройства был заблокирован, очистить или не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5668a-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="5668a-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="5668a-121">keyConflict</span></span>|<span data-ttu-id="5668a-122">4</span><span class="sxs-lookup"><span data-stu-id="5668a-122">4</span></span>|<span data-ttu-id="5668a-123">Устройство имеет конфликты ключа.</span><span class="sxs-lookup"><span data-stu-id="5668a-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="5668a-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="5668a-124">approvalPending</span></span>|<span data-ttu-id="5668a-125">5</span><span class="sxs-lookup"><span data-stu-id="5668a-125">5</span></span>|<span data-ttu-id="5668a-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="5668a-126">The device is pending approval.</span></span>|
|<span data-ttu-id="5668a-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="5668a-127">certificateReset</span></span>|<span data-ttu-id="5668a-128">6</span><span class="sxs-lookup"><span data-stu-id="5668a-128">6</span></span>|<span data-ttu-id="5668a-129">Устройство сертификат был изменен.</span><span class="sxs-lookup"><span data-stu-id="5668a-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="5668a-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="5668a-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="5668a-131">7</span><span class="sxs-lookup"><span data-stu-id="5668a-131">7</span></span>|<span data-ttu-id="5668a-132">Устройства не зарегистрирована и ожидающие заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="5668a-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="5668a-133">unknown</span><span class="sxs-lookup"><span data-stu-id="5668a-133">unknown</span></span>|<span data-ttu-id="5668a-134">8</span><span class="sxs-lookup"><span data-stu-id="5668a-134">8</span></span>|<span data-ttu-id="5668a-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="5668a-135">The device registration status is unknown.</span></span>|





