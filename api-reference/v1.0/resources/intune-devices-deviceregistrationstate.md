---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
ms.openlocfilehash: 9f9ee23d385ce4a7fca73e2d296c3f34063fc218
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024783"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="4bb08-103">Тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4bb08-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="4bb08-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4bb08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bb08-105">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bb08-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="4bb08-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="4bb08-106">Members</span></span>
|<span data-ttu-id="4bb08-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="4bb08-107">Member</span></span>|<span data-ttu-id="4bb08-108">Значение</span><span class="sxs-lookup"><span data-stu-id="4bb08-108">Value</span></span>|<span data-ttu-id="4bb08-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb08-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb08-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="4bb08-110">notRegistered</span></span>|<span data-ttu-id="4bb08-111">0</span><span class="sxs-lookup"><span data-stu-id="4bb08-111">0</span></span>|<span data-ttu-id="4bb08-112">Устройство не зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="4bb08-112">The device is not registered.</span></span>|
|<span data-ttu-id="4bb08-113">зарегистрирована</span><span class="sxs-lookup"><span data-stu-id="4bb08-113">registered</span></span>|<span data-ttu-id="4bb08-114">2</span><span class="sxs-lookup"><span data-stu-id="4bb08-114">2</span></span>|<span data-ttu-id="4bb08-115">Зарегистрированные устройства.</span><span class="sxs-lookup"><span data-stu-id="4bb08-115">The device is registered.</span></span>|
|<span data-ttu-id="4bb08-116">отменено</span><span class="sxs-lookup"><span data-stu-id="4bb08-116">revoked</span></span>|<span data-ttu-id="4bb08-117">3</span><span class="sxs-lookup"><span data-stu-id="4bb08-117">3</span></span>|<span data-ttu-id="4bb08-118">Устройства был заблокирован, очистить или не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb08-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="4bb08-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="4bb08-119">keyConflict</span></span>|<span data-ttu-id="4bb08-120">4</span><span class="sxs-lookup"><span data-stu-id="4bb08-120">4</span></span>|<span data-ttu-id="4bb08-121">Устройство имеет конфликты ключа.</span><span class="sxs-lookup"><span data-stu-id="4bb08-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="4bb08-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="4bb08-122">approvalPending</span></span>|<span data-ttu-id="4bb08-123">5</span><span class="sxs-lookup"><span data-stu-id="4bb08-123">5</span></span>|<span data-ttu-id="4bb08-124">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="4bb08-124">The device is pending approval.</span></span>|
|<span data-ttu-id="4bb08-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="4bb08-125">certificateReset</span></span>|<span data-ttu-id="4bb08-126">6</span><span class="sxs-lookup"><span data-stu-id="4bb08-126">6</span></span>|<span data-ttu-id="4bb08-127">Устройство сертификат был изменен.</span><span class="sxs-lookup"><span data-stu-id="4bb08-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="4bb08-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="4bb08-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="4bb08-129">7</span><span class="sxs-lookup"><span data-stu-id="4bb08-129">7</span></span>|<span data-ttu-id="4bb08-130">Устройства не зарегистрирована и ожидающие заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="4bb08-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="4bb08-131">unknown</span><span class="sxs-lookup"><span data-stu-id="4bb08-131">unknown</span></span>|<span data-ttu-id="4bb08-132">8</span><span class="sxs-lookup"><span data-stu-id="4bb08-132">8</span></span>|<span data-ttu-id="4bb08-133">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="4bb08-133">The device registration status is unknown.</span></span>|



