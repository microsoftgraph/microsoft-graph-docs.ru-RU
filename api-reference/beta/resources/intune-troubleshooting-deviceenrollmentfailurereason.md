---
title: тип перечисления Девицеенроллментфаилуререасон
description: Категории отказов верхнего уровня для регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 02ddb083b7db03dd9eacc07ff35bec8c47b0a290
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728034"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="2139d-103">тип перечисления Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="2139d-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="2139d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2139d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2139d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2139d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2139d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2139d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2139d-107">Категории отказов верхнего уровня для регистрации.</span><span class="sxs-lookup"><span data-stu-id="2139d-107">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="2139d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2139d-108">Members</span></span>
|<span data-ttu-id="2139d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2139d-109">Member</span></span>|<span data-ttu-id="2139d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2139d-110">Value</span></span>|<span data-ttu-id="2139d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2139d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2139d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="2139d-112">unknown</span></span>|<span data-ttu-id="2139d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2139d-113">0</span></span>|<span data-ttu-id="2139d-114">Значение по умолчанию, причина сбоя неизвестна.</span><span class="sxs-lookup"><span data-stu-id="2139d-114">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="2139d-115">проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2139d-115">authentication</span></span>|<span data-ttu-id="2139d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="2139d-116">1</span></span>|<span data-ttu-id="2139d-117">Ошибка проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2139d-117">Authentication failed</span></span>|
|<span data-ttu-id="2139d-118">проверке</span><span class="sxs-lookup"><span data-stu-id="2139d-118">authorization</span></span>|<span data-ttu-id="2139d-119">2</span><span class="sxs-lookup"><span data-stu-id="2139d-119">2</span></span>|<span data-ttu-id="2139d-120">Вызов прошел проверку подлинности, но не авторизован для регистрации.</span><span class="sxs-lookup"><span data-stu-id="2139d-120">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="2139d-121">аккаунтвалидатион</span><span class="sxs-lookup"><span data-stu-id="2139d-121">accountValidation</span></span>|<span data-ttu-id="2139d-122">4</span><span class="sxs-lookup"><span data-stu-id="2139d-122">3</span></span>|<span data-ttu-id="2139d-123">Не удалось проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="2139d-123">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="2139d-124">(Учетная запись заблокирована, регистрация не включена)</span><span class="sxs-lookup"><span data-stu-id="2139d-124">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="2139d-125">усервалидатион</span><span class="sxs-lookup"><span data-stu-id="2139d-125">userValidation</span></span>|<span data-ttu-id="2139d-126">4 </span><span class="sxs-lookup"><span data-stu-id="2139d-126">4</span></span>|<span data-ttu-id="2139d-127">Не удалось проверить пользователя.</span><span class="sxs-lookup"><span data-stu-id="2139d-127">User could not be validated.</span></span> <span data-ttu-id="2139d-128">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="2139d-128">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="2139d-129">девиценотсуппортед</span><span class="sxs-lookup"><span data-stu-id="2139d-129">deviceNotSupported</span></span>|<span data-ttu-id="2139d-130">5 </span><span class="sxs-lookup"><span data-stu-id="2139d-130">5</span></span>|<span data-ttu-id="2139d-131">Устройство не поддерживается для управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="2139d-131">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="2139d-132">необслуживание</span><span class="sxs-lookup"><span data-stu-id="2139d-132">inMaintenance</span></span>|<span data-ttu-id="2139d-133">6 </span><span class="sxs-lookup"><span data-stu-id="2139d-133">6</span></span>|<span data-ttu-id="2139d-134">Учетная запись находится в состоянии обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2139d-134">Account is in maintenance.</span></span>|
|<span data-ttu-id="2139d-135">бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2139d-135">badRequest</span></span>|<span data-ttu-id="2139d-136">7 </span><span class="sxs-lookup"><span data-stu-id="2139d-136">7</span></span>|<span data-ttu-id="2139d-137">Клиент отправил запрос, который не распознаются или не поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="2139d-137">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="2139d-138">феатуренотсуппортед</span><span class="sxs-lookup"><span data-stu-id="2139d-138">featureNotSupported</span></span>|<span data-ttu-id="2139d-139">8 </span><span class="sxs-lookup"><span data-stu-id="2139d-139">8</span></span>|<span data-ttu-id="2139d-140">Функции, используемые этой регистрацией, не поддерживаются для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2139d-140">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="2139d-141">енроллментрестриктионсенфорцед</span><span class="sxs-lookup"><span data-stu-id="2139d-141">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="2139d-142">9 </span><span class="sxs-lookup"><span data-stu-id="2139d-142">9</span></span>|<span data-ttu-id="2139d-143">Ограничения на регистрацию, настроенные администратором, заблокировали эту регистрацию.</span><span class="sxs-lookup"><span data-stu-id="2139d-143">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="2139d-144">клиентдисконнектед</span><span class="sxs-lookup"><span data-stu-id="2139d-144">clientDisconnected</span></span>|<span data-ttu-id="2139d-145">10 </span><span class="sxs-lookup"><span data-stu-id="2139d-145">10</span></span>|<span data-ttu-id="2139d-146">Превышено время ожидания клиента, или Регистрация прервана ендусер.</span><span class="sxs-lookup"><span data-stu-id="2139d-146">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="2139d-147">усерабандонмент</span><span class="sxs-lookup"><span data-stu-id="2139d-147">userAbandonment</span></span>|<span data-ttu-id="2139d-148">-11:00</span><span class="sxs-lookup"><span data-stu-id="2139d-148">11</span></span>|<span data-ttu-id="2139d-149">Регистрация отменена ендусер.</span><span class="sxs-lookup"><span data-stu-id="2139d-149">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="2139d-150">(Ендусер запустил входящую миграцию, но не смог выполнить ее своевременно)</span><span class="sxs-lookup"><span data-stu-id="2139d-150">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|





