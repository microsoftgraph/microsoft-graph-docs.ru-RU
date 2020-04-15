---
title: тип перечисления Девицеенроллментфаилуререасон
description: Категории отказов верхнего уровня для регистрации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fefe8adf226f99a239bd9a04331596861237c0ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445555"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="b4d15-103">тип перечисления Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="b4d15-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="b4d15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4d15-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4d15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d15-106">Категории отказов верхнего уровня для регистрации.</span><span class="sxs-lookup"><span data-stu-id="b4d15-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="b4d15-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b4d15-107">Members</span></span>
|<span data-ttu-id="b4d15-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b4d15-108">Member</span></span>|<span data-ttu-id="b4d15-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b4d15-109">Value</span></span>|<span data-ttu-id="b4d15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4d15-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d15-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b4d15-111">unknown</span></span>|<span data-ttu-id="b4d15-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b4d15-112">0</span></span>|<span data-ttu-id="b4d15-113">Значение по умолчанию, причина сбоя неизвестна.</span><span class="sxs-lookup"><span data-stu-id="b4d15-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="b4d15-114">проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b4d15-114">authentication</span></span>|<span data-ttu-id="b4d15-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b4d15-115">1</span></span>|<span data-ttu-id="b4d15-116">Ошибка проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b4d15-116">Authentication failed</span></span>|
|<span data-ttu-id="b4d15-117">проверке</span><span class="sxs-lookup"><span data-stu-id="b4d15-117">authorization</span></span>|<span data-ttu-id="b4d15-118">2</span><span class="sxs-lookup"><span data-stu-id="b4d15-118">2</span></span>|<span data-ttu-id="b4d15-119">Вызов прошел проверку подлинности, но не авторизован для регистрации.</span><span class="sxs-lookup"><span data-stu-id="b4d15-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="b4d15-120">аккаунтвалидатион</span><span class="sxs-lookup"><span data-stu-id="b4d15-120">accountValidation</span></span>|<span data-ttu-id="b4d15-121">4</span><span class="sxs-lookup"><span data-stu-id="b4d15-121">3</span></span>|<span data-ttu-id="b4d15-122">Не удалось проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="b4d15-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="b4d15-123">(Учетная запись заблокирована, регистрация не включена)</span><span class="sxs-lookup"><span data-stu-id="b4d15-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="b4d15-124">усервалидатион</span><span class="sxs-lookup"><span data-stu-id="b4d15-124">userValidation</span></span>|<span data-ttu-id="b4d15-125">4 </span><span class="sxs-lookup"><span data-stu-id="b4d15-125">4</span></span>|<span data-ttu-id="b4d15-126">Не удалось проверить пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4d15-126">User could not be validated.</span></span> <span data-ttu-id="b4d15-127">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="b4d15-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="b4d15-128">девиценотсуппортед</span><span class="sxs-lookup"><span data-stu-id="b4d15-128">deviceNotSupported</span></span>|<span data-ttu-id="b4d15-129">5 </span><span class="sxs-lookup"><span data-stu-id="b4d15-129">5</span></span>|<span data-ttu-id="b4d15-130">Устройство не поддерживается для управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="b4d15-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="b4d15-131">необслуживание</span><span class="sxs-lookup"><span data-stu-id="b4d15-131">inMaintenance</span></span>|<span data-ttu-id="b4d15-132">6 </span><span class="sxs-lookup"><span data-stu-id="b4d15-132">6</span></span>|<span data-ttu-id="b4d15-133">Учетная запись находится в состоянии обслуживания.</span><span class="sxs-lookup"><span data-stu-id="b4d15-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="b4d15-134">бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b4d15-134">badRequest</span></span>|<span data-ttu-id="b4d15-135">7 </span><span class="sxs-lookup"><span data-stu-id="b4d15-135">7</span></span>|<span data-ttu-id="b4d15-136">Клиент отправил запрос, который не распознаются или не поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="b4d15-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="b4d15-137">феатуренотсуппортед</span><span class="sxs-lookup"><span data-stu-id="b4d15-137">featureNotSupported</span></span>|<span data-ttu-id="b4d15-138">8 </span><span class="sxs-lookup"><span data-stu-id="b4d15-138">8</span></span>|<span data-ttu-id="b4d15-139">Функции, используемые этой регистрацией, не поддерживаются для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b4d15-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="b4d15-140">енроллментрестриктионсенфорцед</span><span class="sxs-lookup"><span data-stu-id="b4d15-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="b4d15-141">9 </span><span class="sxs-lookup"><span data-stu-id="b4d15-141">9</span></span>|<span data-ttu-id="b4d15-142">Ограничения на регистрацию, настроенные администратором, заблокировали эту регистрацию.</span><span class="sxs-lookup"><span data-stu-id="b4d15-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="b4d15-143">клиентдисконнектед</span><span class="sxs-lookup"><span data-stu-id="b4d15-143">clientDisconnected</span></span>|<span data-ttu-id="b4d15-144">10 </span><span class="sxs-lookup"><span data-stu-id="b4d15-144">10</span></span>|<span data-ttu-id="b4d15-145">Превышено время ожидания клиента, или Регистрация прервана ендусер.</span><span class="sxs-lookup"><span data-stu-id="b4d15-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="b4d15-146">усерабандонмент</span><span class="sxs-lookup"><span data-stu-id="b4d15-146">userAbandonment</span></span>|<span data-ttu-id="b4d15-147">-11:00</span><span class="sxs-lookup"><span data-stu-id="b4d15-147">11</span></span>|<span data-ttu-id="b4d15-148">Регистрация отменена ендусер.</span><span class="sxs-lookup"><span data-stu-id="b4d15-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="b4d15-149">(Ендусер запустил входящую миграцию, но не смог выполнить ее своевременно)</span><span class="sxs-lookup"><span data-stu-id="b4d15-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->





