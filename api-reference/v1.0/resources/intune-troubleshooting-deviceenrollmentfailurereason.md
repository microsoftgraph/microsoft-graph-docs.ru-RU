---
title: Тип перечисления deviceEnrollmentFailureReason
description: Категории верхнего уровня failure для регистрации.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efee4e4655d36e7575df9e0ddda508dbbcc473c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962074"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="99333-103">Тип перечисления deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="99333-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="99333-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99333-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99333-105">Категории верхнего уровня failure для регистрации.</span><span class="sxs-lookup"><span data-stu-id="99333-105">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="99333-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="99333-106">Members</span></span>
|<span data-ttu-id="99333-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="99333-107">Member</span></span>|<span data-ttu-id="99333-108">Значение</span><span class="sxs-lookup"><span data-stu-id="99333-108">Value</span></span>|<span data-ttu-id="99333-109">Описание</span><span class="sxs-lookup"><span data-stu-id="99333-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99333-110">unknown</span><span class="sxs-lookup"><span data-stu-id="99333-110">unknown</span></span>|<span data-ttu-id="99333-111">0</span><span class="sxs-lookup"><span data-stu-id="99333-111">0</span></span>|<span data-ttu-id="99333-112">Значение по умолчанию причина сбоя не известен.</span><span class="sxs-lookup"><span data-stu-id="99333-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="99333-113">проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="99333-113">authentication</span></span>|<span data-ttu-id="99333-114">1</span><span class="sxs-lookup"><span data-stu-id="99333-114">1</span></span>|<span data-ttu-id="99333-115">Ошибка проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="99333-115">Authentication failed</span></span>|
|<span data-ttu-id="99333-116">авторизация</span><span class="sxs-lookup"><span data-stu-id="99333-116">authorization</span></span>|<span data-ttu-id="99333-117">2</span><span class="sxs-lookup"><span data-stu-id="99333-117">2</span></span>|<span data-ttu-id="99333-118">Звонок был прошедшим проверку подлинности, но не разрешена для регистрации.</span><span class="sxs-lookup"><span data-stu-id="99333-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="99333-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="99333-119">accountValidation</span></span>|<span data-ttu-id="99333-120">3</span><span class="sxs-lookup"><span data-stu-id="99333-120">3</span></span>|<span data-ttu-id="99333-121">Не удается проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="99333-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="99333-122">(Учетная запись заблокирована, регистрации не включена)</span><span class="sxs-lookup"><span data-stu-id="99333-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="99333-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="99333-123">userValidation</span></span>|<span data-ttu-id="99333-124">4</span><span class="sxs-lookup"><span data-stu-id="99333-124">4</span></span>|<span data-ttu-id="99333-125">Пользователь не может быть проверен.</span><span class="sxs-lookup"><span data-stu-id="99333-125">User could not be validated.</span></span> <span data-ttu-id="99333-126">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="99333-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="99333-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="99333-127">deviceNotSupported</span></span>|<span data-ttu-id="99333-128">5</span><span class="sxs-lookup"><span data-stu-id="99333-128">5</span></span>|<span data-ttu-id="99333-129">Устройство не поддерживается для мобильных устройств management.</span><span class="sxs-lookup"><span data-stu-id="99333-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="99333-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="99333-130">inMaintenance</span></span>|<span data-ttu-id="99333-131">6</span><span class="sxs-lookup"><span data-stu-id="99333-131">6</span></span>|<span data-ttu-id="99333-132">Учетная запись является в режим обслуживания.</span><span class="sxs-lookup"><span data-stu-id="99333-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="99333-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="99333-133">badRequest</span></span>|<span data-ttu-id="99333-134">7</span><span class="sxs-lookup"><span data-stu-id="99333-134">7</span></span>|<span data-ttu-id="99333-135">Клиент отправил запрос, который не является поняты/поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="99333-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="99333-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="99333-136">featureNotSupported</span></span>|<span data-ttu-id="99333-137">8</span><span class="sxs-lookup"><span data-stu-id="99333-137">8</span></span>|<span data-ttu-id="99333-138">Компоненты, используемые в этом регистрации не поддерживается для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="99333-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="99333-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="99333-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="99333-140">9</span><span class="sxs-lookup"><span data-stu-id="99333-140">9</span></span>|<span data-ttu-id="99333-141">Ограничения для регистрации настроены администратором заблокированные этой регистрации.</span><span class="sxs-lookup"><span data-stu-id="99333-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="99333-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="99333-142">clientDisconnected</span></span>|<span data-ttu-id="99333-143">10</span><span class="sxs-lookup"><span data-stu-id="99333-143">10</span></span>|<span data-ttu-id="99333-144">Истекло время ожидания клиента или регистрации был прерван пользователем enduser.</span><span class="sxs-lookup"><span data-stu-id="99333-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="99333-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="99333-145">userAbandonment</span></span>|<span data-ttu-id="99333-146">11</span><span class="sxs-lookup"><span data-stu-id="99333-146">11</span></span>|<span data-ttu-id="99333-147">Регистрация отменена с enduser.</span><span class="sxs-lookup"><span data-stu-id="99333-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="99333-148">(Enduser работы адаптация новых сотрудников, но не удалось завершить своевременно)</span><span class="sxs-lookup"><span data-stu-id="99333-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
