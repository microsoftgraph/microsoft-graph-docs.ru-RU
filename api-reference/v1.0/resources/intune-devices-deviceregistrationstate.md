---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b0048385930166de3329ef9d407f5ddd19efc77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911898"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="6c468-103">Тип перечисления deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6c468-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="6c468-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6c468-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c468-105">Состояние регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="6c468-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="6c468-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="6c468-106">Members</span></span>
|<span data-ttu-id="6c468-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="6c468-107">Member</span></span>|<span data-ttu-id="6c468-108">Значение</span><span class="sxs-lookup"><span data-stu-id="6c468-108">Value</span></span>|<span data-ttu-id="6c468-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6c468-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c468-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="6c468-110">notRegistered</span></span>|<span data-ttu-id="6c468-111">0</span><span class="sxs-lookup"><span data-stu-id="6c468-111">0</span></span>|<span data-ttu-id="6c468-112">Устройство не зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="6c468-112">The device is not registered.</span></span>|
|<span data-ttu-id="6c468-113">зарегистрирована</span><span class="sxs-lookup"><span data-stu-id="6c468-113">registered</span></span>|<span data-ttu-id="6c468-114">2</span><span class="sxs-lookup"><span data-stu-id="6c468-114">2</span></span>|<span data-ttu-id="6c468-115">Зарегистрированные устройства.</span><span class="sxs-lookup"><span data-stu-id="6c468-115">The device is registered.</span></span>|
|<span data-ttu-id="6c468-116">отменено</span><span class="sxs-lookup"><span data-stu-id="6c468-116">revoked</span></span>|<span data-ttu-id="6c468-117">3</span><span class="sxs-lookup"><span data-stu-id="6c468-117">3</span></span>|<span data-ttu-id="6c468-118">Устройства был заблокирован, очистить или не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c468-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="6c468-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="6c468-119">keyConflict</span></span>|<span data-ttu-id="6c468-120">4</span><span class="sxs-lookup"><span data-stu-id="6c468-120">4</span></span>|<span data-ttu-id="6c468-121">Устройство имеет конфликты ключа.</span><span class="sxs-lookup"><span data-stu-id="6c468-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="6c468-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="6c468-122">approvalPending</span></span>|<span data-ttu-id="6c468-123">5</span><span class="sxs-lookup"><span data-stu-id="6c468-123">5</span></span>|<span data-ttu-id="6c468-124">Устройство ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="6c468-124">The device is pending approval.</span></span>|
|<span data-ttu-id="6c468-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="6c468-125">certificateReset</span></span>|<span data-ttu-id="6c468-126">6</span><span class="sxs-lookup"><span data-stu-id="6c468-126">6</span></span>|<span data-ttu-id="6c468-127">Устройство сертификат был изменен.</span><span class="sxs-lookup"><span data-stu-id="6c468-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="6c468-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="6c468-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="6c468-129">7</span><span class="sxs-lookup"><span data-stu-id="6c468-129">7</span></span>|<span data-ttu-id="6c468-130">Устройства не зарегистрирована и ожидающие заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="6c468-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="6c468-131">unknown</span><span class="sxs-lookup"><span data-stu-id="6c468-131">unknown</span></span>|<span data-ttu-id="6c468-132">8</span><span class="sxs-lookup"><span data-stu-id="6c468-132">8</span></span>|<span data-ttu-id="6c468-133">Состояние регистрации устройства неизвестно.</span><span class="sxs-lookup"><span data-stu-id="6c468-133">The device registration status is unknown.</span></span>|



