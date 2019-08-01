---
title: тип перечисления Девицеенроллментфаилуререасон
description: Категории отказов верхнего уровня для регистрации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 742c30da453a8de814dad0a70fae2be2946f1127
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036794"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="2d7c6-103">тип перечисления Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="2d7c6-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="2d7c6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d7c6-105">Категории отказов верхнего уровня для регистрации.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="2d7c6-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d7c6-106">Members</span></span>
|<span data-ttu-id="2d7c6-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d7c6-107">Member</span></span>|<span data-ttu-id="2d7c6-108">Значение</span><span class="sxs-lookup"><span data-stu-id="2d7c6-108">Value</span></span>|<span data-ttu-id="2d7c6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2d7c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d7c6-110">unknown</span><span class="sxs-lookup"><span data-stu-id="2d7c6-110">unknown</span></span>|<span data-ttu-id="2d7c6-111">нуль</span><span class="sxs-lookup"><span data-stu-id="2d7c6-111">0</span></span>|<span data-ttu-id="2d7c6-112">Значение по умолчанию, причина сбоя неизвестна.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="2d7c6-113">проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2d7c6-113">authentication</span></span>|<span data-ttu-id="2d7c6-114">1,1</span><span class="sxs-lookup"><span data-stu-id="2d7c6-114">1</span></span>|<span data-ttu-id="2d7c6-115">Ошибка проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2d7c6-115">Authentication failed</span></span>|
|<span data-ttu-id="2d7c6-116">проверке</span><span class="sxs-lookup"><span data-stu-id="2d7c6-116">authorization</span></span>|<span data-ttu-id="2d7c6-117">2</span><span class="sxs-lookup"><span data-stu-id="2d7c6-117">2</span></span>|<span data-ttu-id="2d7c6-118">Вызов прошел проверку подлинности, но не авторизован для регистрации.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="2d7c6-119">Аккаунтвалидатион</span><span class="sxs-lookup"><span data-stu-id="2d7c6-119">accountValidation</span></span>|<span data-ttu-id="2d7c6-120">4</span><span class="sxs-lookup"><span data-stu-id="2d7c6-120">3</span></span>|<span data-ttu-id="2d7c6-121">Не удалось проверить учетную запись для регистрации.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="2d7c6-122">(Учетная запись заблокирована, регистрация не включена)</span><span class="sxs-lookup"><span data-stu-id="2d7c6-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="2d7c6-123">Усервалидатион</span><span class="sxs-lookup"><span data-stu-id="2d7c6-123">userValidation</span></span>|<span data-ttu-id="2d7c6-124">SP4</span><span class="sxs-lookup"><span data-stu-id="2d7c6-124">4</span></span>|<span data-ttu-id="2d7c6-125">Не удалось проверить пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-125">User could not be validated.</span></span> <span data-ttu-id="2d7c6-126">(Пользователь не существует, отсутствует лицензия)</span><span class="sxs-lookup"><span data-stu-id="2d7c6-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="2d7c6-127">Девиценотсуппортед</span><span class="sxs-lookup"><span data-stu-id="2d7c6-127">deviceNotSupported</span></span>|<span data-ttu-id="2d7c6-128">17:00</span><span class="sxs-lookup"><span data-stu-id="2d7c6-128">5</span></span>|<span data-ttu-id="2d7c6-129">Устройство не поддерживается для управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="2d7c6-130">необслуживание</span><span class="sxs-lookup"><span data-stu-id="2d7c6-130">inMaintenance</span></span>|<span data-ttu-id="2d7c6-131">6 </span><span class="sxs-lookup"><span data-stu-id="2d7c6-131">6</span></span>|<span data-ttu-id="2d7c6-132">Учетная запись находится в состоянии обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="2d7c6-133">Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2d7c6-133">badRequest</span></span>|<span data-ttu-id="2d7c6-134">7 </span><span class="sxs-lookup"><span data-stu-id="2d7c6-134">7</span></span>|<span data-ttu-id="2d7c6-135">Клиент отправил запрос, который не распознаются или не поддерживается службой.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="2d7c6-136">Феатуренотсуппортед</span><span class="sxs-lookup"><span data-stu-id="2d7c6-136">featureNotSupported</span></span>|<span data-ttu-id="2d7c6-137">8 </span><span class="sxs-lookup"><span data-stu-id="2d7c6-137">8</span></span>|<span data-ttu-id="2d7c6-138">Функции, используемые этой регистрацией, не поддерживаются для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="2d7c6-139">Енроллментрестриктионсенфорцед</span><span class="sxs-lookup"><span data-stu-id="2d7c6-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="2d7c6-140">9 </span><span class="sxs-lookup"><span data-stu-id="2d7c6-140">9</span></span>|<span data-ttu-id="2d7c6-141">Ограничения на регистрацию, настроенные администратором, заблокировали эту регистрацию.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="2d7c6-142">Клиентдисконнектед</span><span class="sxs-lookup"><span data-stu-id="2d7c6-142">clientDisconnected</span></span>|<span data-ttu-id="2d7c6-143">10 </span><span class="sxs-lookup"><span data-stu-id="2d7c6-143">10</span></span>|<span data-ttu-id="2d7c6-144">Превышено время ожидания клиента, или Регистрация прервана ендусер.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="2d7c6-145">Усерабандонмент</span><span class="sxs-lookup"><span data-stu-id="2d7c6-145">userAbandonment</span></span>|<span data-ttu-id="2d7c6-146">-11:00</span><span class="sxs-lookup"><span data-stu-id="2d7c6-146">11</span></span>|<span data-ttu-id="2d7c6-147">Регистрация отменена ендусер.</span><span class="sxs-lookup"><span data-stu-id="2d7c6-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="2d7c6-148">(Ендусер запустил входящую миграцию, но не смог выполнить ее своевременно)</span><span class="sxs-lookup"><span data-stu-id="2d7c6-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

