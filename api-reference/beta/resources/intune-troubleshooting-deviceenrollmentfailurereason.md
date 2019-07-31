---
title: тип перечисления Девицеенроллментфаилуререасон
description: Категории отказов верхнего уровня для регистрации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a0721495a8eb217007c0ee1f18942009614696d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010317"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="a2bb6-103">тип перечисления Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="a2bb6-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="a2bb6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2bb6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2bb6-106">Категории отказов верхнего уровня для регистрации.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="a2bb6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a2bb6-107">Members</span></span>
|<span data-ttu-id="a2bb6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a2bb6-108">Member</span></span>|<span data-ttu-id="a2bb6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a2bb6-109">Value</span></span>|<span data-ttu-id="a2bb6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2bb6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2bb6-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a2bb6-111">unknown</span></span>|<span data-ttu-id="a2bb6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a2bb6-112">0</span></span>|<span data-ttu-id="a2bb6-113">Значение по умолчанию, причина сбоя неизвестна.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="a2bb6-114">проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a2bb6-114">authentication</span></span>|<span data-ttu-id="a2bb6-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a2bb6-115">1</span></span>|<span data-ttu-id="a2bb6-116">Ошибка проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a2bb6-116">Authentication failed</span></span>|
|<span data-ttu-id="a2bb6-117">проверке</span><span class="sxs-lookup"><span data-stu-id="a2bb6-117">authorization</span></span>|<span data-ttu-id="a2bb6-118">2</span><span class="sxs-lookup"><span data-stu-id="a2bb6-118">2</span></span>|<span data-ttu-id="a2bb6-119">Вызов прошел проверку подлинности, но не авторизован для регистрации.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="a2bb6-120">Аккаунтвалидатион</span><span class="sxs-lookup"><span data-stu-id="a2bb6-120">accountValidation</span></span>|<span data-ttu-id="a2bb6-121">4</span><span class="sxs-lookup"><span data-stu-id="a2bb6-121">3</span></span>|<span data-ttu-id="a2bb6-122">Не удалось проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="a2bb6-123">(Учетная запись заблокирована, регистрация не включена)</span><span class="sxs-lookup"><span data-stu-id="a2bb6-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="a2bb6-124">Усервалидатион</span><span class="sxs-lookup"><span data-stu-id="a2bb6-124">userValidation</span></span>|<span data-ttu-id="a2bb6-125">SP4</span><span class="sxs-lookup"><span data-stu-id="a2bb6-125">4</span></span>|<span data-ttu-id="a2bb6-126">Не удалось проверить пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-126">User could not be validated.</span></span> <span data-ttu-id="a2bb6-127">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="a2bb6-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="a2bb6-128">Девиценотсуппортед</span><span class="sxs-lookup"><span data-stu-id="a2bb6-128">deviceNotSupported</span></span>|<span data-ttu-id="a2bb6-129">17:00</span><span class="sxs-lookup"><span data-stu-id="a2bb6-129">5</span></span>|<span data-ttu-id="a2bb6-130">Устройство не поддерживается для управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="a2bb6-131">необслуживание</span><span class="sxs-lookup"><span data-stu-id="a2bb6-131">inMaintenance</span></span>|<span data-ttu-id="a2bb6-132">6 </span><span class="sxs-lookup"><span data-stu-id="a2bb6-132">6</span></span>|<span data-ttu-id="a2bb6-133">Учетная запись находится в состоянии обслуживания.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="a2bb6-134">Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a2bb6-134">badRequest</span></span>|<span data-ttu-id="a2bb6-135">7 </span><span class="sxs-lookup"><span data-stu-id="a2bb6-135">7</span></span>|<span data-ttu-id="a2bb6-136">Клиент отправил запрос, который не распознаются или не поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="a2bb6-137">Феатуренотсуппортед</span><span class="sxs-lookup"><span data-stu-id="a2bb6-137">featureNotSupported</span></span>|<span data-ttu-id="a2bb6-138">8 </span><span class="sxs-lookup"><span data-stu-id="a2bb6-138">8</span></span>|<span data-ttu-id="a2bb6-139">Функции, используемые этой регистрацией, не поддерживаются для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="a2bb6-140">Енроллментрестриктионсенфорцед</span><span class="sxs-lookup"><span data-stu-id="a2bb6-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="a2bb6-141">9 </span><span class="sxs-lookup"><span data-stu-id="a2bb6-141">9</span></span>|<span data-ttu-id="a2bb6-142">Ограничения на регистрацию, настроенные администратором, заблокировали эту регистрацию.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="a2bb6-143">Клиентдисконнектед</span><span class="sxs-lookup"><span data-stu-id="a2bb6-143">clientDisconnected</span></span>|<span data-ttu-id="a2bb6-144">10 </span><span class="sxs-lookup"><span data-stu-id="a2bb6-144">10</span></span>|<span data-ttu-id="a2bb6-145">Превышено время ожидания клиента, или Регистрация прервана ендусер.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="a2bb6-146">Усерабандонмент</span><span class="sxs-lookup"><span data-stu-id="a2bb6-146">userAbandonment</span></span>|<span data-ttu-id="a2bb6-147">-11:00</span><span class="sxs-lookup"><span data-stu-id="a2bb6-147">11</span></span>|<span data-ttu-id="a2bb6-148">Регистрация отменена ендусер.</span><span class="sxs-lookup"><span data-stu-id="a2bb6-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="a2bb6-149">(Ендусер запустил входящую миграцию, но не смог выполнить ее своевременно)</span><span class="sxs-lookup"><span data-stu-id="a2bb6-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|





