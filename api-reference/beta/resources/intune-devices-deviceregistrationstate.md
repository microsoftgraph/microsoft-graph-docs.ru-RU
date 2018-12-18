---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
ms.openlocfilehash: a622613bd4ca5e065c3d9eb0331c05c360c1837c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360545"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="e03bd-103">Тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="e03bd-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="e03bd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e03bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e03bd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e03bd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e03bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e03bd-107">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="e03bd-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="e03bd-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e03bd-108">Members</span></span>
|<span data-ttu-id="e03bd-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e03bd-109">Member</span></span>|<span data-ttu-id="e03bd-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e03bd-110">Value</span></span>|<span data-ttu-id="e03bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e03bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e03bd-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="e03bd-112">notRegistered</span></span>|<span data-ttu-id="e03bd-113">0</span><span class="sxs-lookup"><span data-stu-id="e03bd-113">0</span></span>|<span data-ttu-id="e03bd-114">Устройство не зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="e03bd-114">The device is not registered.</span></span>|
|<span data-ttu-id="e03bd-115">зарегистрирована</span><span class="sxs-lookup"><span data-stu-id="e03bd-115">registered</span></span>|<span data-ttu-id="e03bd-116">2</span><span class="sxs-lookup"><span data-stu-id="e03bd-116">2</span></span>|<span data-ttu-id="e03bd-117">Зарегистрированные устройства.</span><span class="sxs-lookup"><span data-stu-id="e03bd-117">The device is registered.</span></span>|
|<span data-ttu-id="e03bd-118">отменено</span><span class="sxs-lookup"><span data-stu-id="e03bd-118">revoked</span></span>|<span data-ttu-id="e03bd-119">3</span><span class="sxs-lookup"><span data-stu-id="e03bd-119">3</span></span>|<span data-ttu-id="e03bd-120">Устройства был заблокирован, очистить или не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03bd-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="e03bd-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="e03bd-121">keyConflict</span></span>|<span data-ttu-id="e03bd-122">4</span><span class="sxs-lookup"><span data-stu-id="e03bd-122">4</span></span>|<span data-ttu-id="e03bd-123">Устройство имеет конфликты ключа.</span><span class="sxs-lookup"><span data-stu-id="e03bd-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="e03bd-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="e03bd-124">approvalPending</span></span>|<span data-ttu-id="e03bd-125">5</span><span class="sxs-lookup"><span data-stu-id="e03bd-125">5</span></span>|<span data-ttu-id="e03bd-126">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="e03bd-126">The device is pending approval.</span></span>|
|<span data-ttu-id="e03bd-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="e03bd-127">certificateReset</span></span>|<span data-ttu-id="e03bd-128">6</span><span class="sxs-lookup"><span data-stu-id="e03bd-128">6</span></span>|<span data-ttu-id="e03bd-129">Устройство сертификат был изменен.</span><span class="sxs-lookup"><span data-stu-id="e03bd-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="e03bd-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="e03bd-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="e03bd-131">7</span><span class="sxs-lookup"><span data-stu-id="e03bd-131">7</span></span>|<span data-ttu-id="e03bd-132">Устройства не зарегистрирована и ожидающие заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="e03bd-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="e03bd-133">unknown</span><span class="sxs-lookup"><span data-stu-id="e03bd-133">unknown</span></span>|<span data-ttu-id="e03bd-134">8</span><span class="sxs-lookup"><span data-stu-id="e03bd-134">8</span></span>|<span data-ttu-id="e03bd-135">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="e03bd-135">The device registration status is unknown.</span></span>|





