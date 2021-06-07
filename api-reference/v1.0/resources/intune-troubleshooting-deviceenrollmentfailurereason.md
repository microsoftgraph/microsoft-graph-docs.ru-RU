---
title: тип enum deviceEnrollmentFailureReason
description: Категории отказов верхнего уровня для регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ee798d2cd9c21038cff177320b3a3ae37d05f2e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732745"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="87a09-103">тип enum deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="87a09-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="87a09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87a09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87a09-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a09-106">Категории отказов верхнего уровня для регистрации.</span><span class="sxs-lookup"><span data-stu-id="87a09-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="87a09-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="87a09-107">Members</span></span>
|<span data-ttu-id="87a09-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="87a09-108">Member</span></span>|<span data-ttu-id="87a09-109">Значение</span><span class="sxs-lookup"><span data-stu-id="87a09-109">Value</span></span>|<span data-ttu-id="87a09-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87a09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a09-111">unknown</span><span class="sxs-lookup"><span data-stu-id="87a09-111">unknown</span></span>|<span data-ttu-id="87a09-112">0</span><span class="sxs-lookup"><span data-stu-id="87a09-112">0</span></span>|<span data-ttu-id="87a09-113">Значение по умолчанию, причина сбоя неизвестна.</span><span class="sxs-lookup"><span data-stu-id="87a09-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="87a09-114">проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="87a09-114">authentication</span></span>|<span data-ttu-id="87a09-115">1</span><span class="sxs-lookup"><span data-stu-id="87a09-115">1</span></span>|<span data-ttu-id="87a09-116">Сбой проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="87a09-116">Authentication failed</span></span>|
|<span data-ttu-id="87a09-117">авторизация</span><span class="sxs-lookup"><span data-stu-id="87a09-117">authorization</span></span>|<span data-ttu-id="87a09-118">2</span><span class="sxs-lookup"><span data-stu-id="87a09-118">2</span></span>|<span data-ttu-id="87a09-119">Вызов был аутентификацией, но не разрешен для регистрации.</span><span class="sxs-lookup"><span data-stu-id="87a09-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="87a09-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="87a09-120">accountValidation</span></span>|<span data-ttu-id="87a09-121">3</span><span class="sxs-lookup"><span data-stu-id="87a09-121">3</span></span>|<span data-ttu-id="87a09-122">Не удалось проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="87a09-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="87a09-123">(Учетная запись заблокирована, регистрация не включена)</span><span class="sxs-lookup"><span data-stu-id="87a09-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="87a09-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="87a09-124">userValidation</span></span>|<span data-ttu-id="87a09-125">4 </span><span class="sxs-lookup"><span data-stu-id="87a09-125">4</span></span>|<span data-ttu-id="87a09-126">Пользователь не может быть проверен.</span><span class="sxs-lookup"><span data-stu-id="87a09-126">User could not be validated.</span></span> <span data-ttu-id="87a09-127">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="87a09-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="87a09-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="87a09-128">deviceNotSupported</span></span>|<span data-ttu-id="87a09-129">5 </span><span class="sxs-lookup"><span data-stu-id="87a09-129">5</span></span>|<span data-ttu-id="87a09-130">Устройство не поддерживается для управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="87a09-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="87a09-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="87a09-131">inMaintenance</span></span>|<span data-ttu-id="87a09-132">6 </span><span class="sxs-lookup"><span data-stu-id="87a09-132">6</span></span>|<span data-ttu-id="87a09-133">Учетная запись находится в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="87a09-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="87a09-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="87a09-134">badRequest</span></span>|<span data-ttu-id="87a09-135">7 </span><span class="sxs-lookup"><span data-stu-id="87a09-135">7</span></span>|<span data-ttu-id="87a09-136">Клиент отправил запрос, который не понят или поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="87a09-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="87a09-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="87a09-137">featureNotSupported</span></span>|<span data-ttu-id="87a09-138">8 </span><span class="sxs-lookup"><span data-stu-id="87a09-138">8</span></span>|<span data-ttu-id="87a09-139">Функция(ы), используемая этой учетной записью, не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a09-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="87a09-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="87a09-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="87a09-141">9 </span><span class="sxs-lookup"><span data-stu-id="87a09-141">9</span></span>|<span data-ttu-id="87a09-142">Ограничения регистрации, настроенные администратором, заблокировали эту регистрацию.</span><span class="sxs-lookup"><span data-stu-id="87a09-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="87a09-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="87a09-143">clientDisconnected</span></span>|<span data-ttu-id="87a09-144">10 </span><span class="sxs-lookup"><span data-stu-id="87a09-144">10</span></span>|<span data-ttu-id="87a09-145">Клиент, отовремя отсев или регистрация, был прерван enduser.</span><span class="sxs-lookup"><span data-stu-id="87a09-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="87a09-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="87a09-146">userAbandonment</span></span>|<span data-ttu-id="87a09-147">11</span><span class="sxs-lookup"><span data-stu-id="87a09-147">11</span></span>|<span data-ttu-id="87a09-148">Регистрация была отменена enduser.</span><span class="sxs-lookup"><span data-stu-id="87a09-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="87a09-149">(Enduser начал работать на борту, но не удалось выполнить его своевременно)</span><span class="sxs-lookup"><span data-stu-id="87a09-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->







