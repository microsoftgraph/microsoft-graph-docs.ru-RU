---
title: тип перечисления Девицеенроллментфаилуререасон
description: Категории отказов верхнего уровня для регистрации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 623030bccfac9e023a0d1df2dff7ea317b503485
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571837"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="d106c-103">тип перечисления Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="d106c-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="d106c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d106c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d106c-105">Категории отказов верхнего уровня для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d106c-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="d106c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d106c-106">Members</span></span>
|<span data-ttu-id="d106c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d106c-107">Member</span></span>|<span data-ttu-id="d106c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d106c-108">Value</span></span>|<span data-ttu-id="d106c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d106c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d106c-110">unknown</span><span class="sxs-lookup"><span data-stu-id="d106c-110">unknown</span></span>|<span data-ttu-id="d106c-111">нуль</span><span class="sxs-lookup"><span data-stu-id="d106c-111">0</span></span>|<span data-ttu-id="d106c-112">Значение по умолчанию, причина сбоя неизвестна.</span><span class="sxs-lookup"><span data-stu-id="d106c-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="d106c-113">проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="d106c-113">authentication</span></span>|<span data-ttu-id="d106c-114">1 </span><span class="sxs-lookup"><span data-stu-id="d106c-114">1</span></span>|<span data-ttu-id="d106c-115">Ошибка проверки поДлинности</span><span class="sxs-lookup"><span data-stu-id="d106c-115">Authentication failed</span></span>|
|<span data-ttu-id="d106c-116">проверке</span><span class="sxs-lookup"><span data-stu-id="d106c-116">authorization</span></span>|<span data-ttu-id="d106c-117">2 </span><span class="sxs-lookup"><span data-stu-id="d106c-117">2</span></span>|<span data-ttu-id="d106c-118">Вызов прошел проверку подлинности, но не авторизован для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d106c-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="d106c-119">Аккаунтвалидатион</span><span class="sxs-lookup"><span data-stu-id="d106c-119">accountValidation</span></span>|<span data-ttu-id="d106c-120">3 </span><span class="sxs-lookup"><span data-stu-id="d106c-120">3</span></span>|<span data-ttu-id="d106c-121">Не удалось проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d106c-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="d106c-122">(Учетная запись заблокирована, регистрация не включена)</span><span class="sxs-lookup"><span data-stu-id="d106c-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="d106c-123">Усервалидатион</span><span class="sxs-lookup"><span data-stu-id="d106c-123">userValidation</span></span>|<span data-ttu-id="d106c-124">4 </span><span class="sxs-lookup"><span data-stu-id="d106c-124">4</span></span>|<span data-ttu-id="d106c-125">Не удалось проверить пользователя.</span><span class="sxs-lookup"><span data-stu-id="d106c-125">User could not be validated.</span></span> <span data-ttu-id="d106c-126">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="d106c-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="d106c-127">Девиценотсуппортед</span><span class="sxs-lookup"><span data-stu-id="d106c-127">deviceNotSupported</span></span>|<span data-ttu-id="d106c-128">5 </span><span class="sxs-lookup"><span data-stu-id="d106c-128">5</span></span>|<span data-ttu-id="d106c-129">Устройство не поддерживается для управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="d106c-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="d106c-130">неОбслуживание</span><span class="sxs-lookup"><span data-stu-id="d106c-130">inMaintenance</span></span>|<span data-ttu-id="d106c-131">6 </span><span class="sxs-lookup"><span data-stu-id="d106c-131">6</span></span>|<span data-ttu-id="d106c-132">Учетная запись находится в состоянии обслуживания.</span><span class="sxs-lookup"><span data-stu-id="d106c-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="d106c-133">Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d106c-133">badRequest</span></span>|<span data-ttu-id="d106c-134">7 </span><span class="sxs-lookup"><span data-stu-id="d106c-134">7</span></span>|<span data-ttu-id="d106c-135">Клиент отправил запрос, который не распознаются или не поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="d106c-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="d106c-136">Феатуренотсуппортед</span><span class="sxs-lookup"><span data-stu-id="d106c-136">featureNotSupported</span></span>|<span data-ttu-id="d106c-137">8 </span><span class="sxs-lookup"><span data-stu-id="d106c-137">8</span></span>|<span data-ttu-id="d106c-138">Функции, используемые этой регистрацией, не поддерживаются для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d106c-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="d106c-139">Енроллментрестриктионсенфорцед</span><span class="sxs-lookup"><span data-stu-id="d106c-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="d106c-140">9 </span><span class="sxs-lookup"><span data-stu-id="d106c-140">9</span></span>|<span data-ttu-id="d106c-141">Ограничения на регистрацию, настроенные администратором, заблокировали эту регистрацию.</span><span class="sxs-lookup"><span data-stu-id="d106c-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="d106c-142">Клиентдисконнектед</span><span class="sxs-lookup"><span data-stu-id="d106c-142">clientDisconnected</span></span>|<span data-ttu-id="d106c-143">10 </span><span class="sxs-lookup"><span data-stu-id="d106c-143">10</span></span>|<span data-ttu-id="d106c-144">Превышено время ожидания клиента, или Регистрация прервана ендусер.</span><span class="sxs-lookup"><span data-stu-id="d106c-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="d106c-145">Усерабандонмент</span><span class="sxs-lookup"><span data-stu-id="d106c-145">userAbandonment</span></span>|<span data-ttu-id="d106c-146">11 </span><span class="sxs-lookup"><span data-stu-id="d106c-146">11</span></span>|<span data-ttu-id="d106c-147">Регистрация отменена ендусер.</span><span class="sxs-lookup"><span data-stu-id="d106c-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="d106c-148">(Ендусер запустил входящую миграцию, но не смог выполнить ее своевременно)</span><span class="sxs-lookup"><span data-stu-id="d106c-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

