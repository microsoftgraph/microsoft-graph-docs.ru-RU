---
title: тип перечисления Манажеддевицепартнеррепортедхеалсстате
description: Доступные состояния работоспособности для API работоспособности устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b0df2859ccee3d4eff9b98c6effb44a4552d93db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091063"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="dfc21-103">тип перечисления Манажеддевицепартнеррепортедхеалсстате</span><span class="sxs-lookup"><span data-stu-id="dfc21-103">managedDevicePartnerReportedHealthState enum type</span></span>

<span data-ttu-id="dfc21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfc21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfc21-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfc21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfc21-106">Доступные состояния работоспособности для API работоспособности устройств</span><span class="sxs-lookup"><span data-stu-id="dfc21-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="dfc21-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dfc21-107">Members</span></span>
|<span data-ttu-id="dfc21-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dfc21-108">Member</span></span>|<span data-ttu-id="dfc21-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dfc21-109">Value</span></span>|<span data-ttu-id="dfc21-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfc21-111">unknown</span><span class="sxs-lookup"><span data-stu-id="dfc21-111">unknown</span></span>|<span data-ttu-id="dfc21-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dfc21-112">0</span></span>|<span data-ttu-id="dfc21-113">Состояние работоспособности устройства еще не отображается</span><span class="sxs-lookup"><span data-stu-id="dfc21-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="dfc21-114">активной</span><span class="sxs-lookup"><span data-stu-id="dfc21-114">activated</span></span>|<span data-ttu-id="dfc21-115">1 </span><span class="sxs-lookup"><span data-stu-id="dfc21-115">1</span></span>|<span data-ttu-id="dfc21-116">Устройство активировано партнером по защите от угроз для мобильных устройств, но еще не сообщило о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="dfc21-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="dfc21-117">деактивирован</span><span class="sxs-lookup"><span data-stu-id="dfc21-117">deactivated</span></span>|<span data-ttu-id="dfc21-118">2 </span><span class="sxs-lookup"><span data-stu-id="dfc21-118">2</span></span>|<span data-ttu-id="dfc21-119">Устройство отключено партнером по защите от угроз для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfc21-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="dfc21-120">Работоспособность устройства неизвестна.</span><span class="sxs-lookup"><span data-stu-id="dfc21-120">The device health is not known.</span></span>|
|<span data-ttu-id="dfc21-121">входящего</span><span class="sxs-lookup"><span data-stu-id="dfc21-121">secured</span></span>|<span data-ttu-id="dfc21-122">4</span><span class="sxs-lookup"><span data-stu-id="dfc21-122">3</span></span>|<span data-ttu-id="dfc21-123">Устройство считается защищенным партнером по защите от угроз для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfc21-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="dfc21-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="dfc21-124">lowSeverity</span></span>|<span data-ttu-id="dfc21-125">4 </span><span class="sxs-lookup"><span data-stu-id="dfc21-125">4</span></span>|<span data-ttu-id="dfc21-126">Устройство считается нехваткой угроз для партнера по защите от угроз для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfc21-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="dfc21-127">медиумсеверити</span><span class="sxs-lookup"><span data-stu-id="dfc21-127">mediumSeverity</span></span>|<span data-ttu-id="dfc21-128">5 </span><span class="sxs-lookup"><span data-stu-id="dfc21-128">5</span></span>|<span data-ttu-id="dfc21-129">Устройство считается средней угрозой с помощью партнера по защите от угроз для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfc21-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="dfc21-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="dfc21-130">highSeverity</span></span>|<span data-ttu-id="dfc21-131">6 </span><span class="sxs-lookup"><span data-stu-id="dfc21-131">6</span></span>|<span data-ttu-id="dfc21-132">Устройство считается высокой угрозой с помощью партнера по защите от угроз для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfc21-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="dfc21-133">не отвечает</span><span class="sxs-lookup"><span data-stu-id="dfc21-133">unresponsive</span></span>|<span data-ttu-id="dfc21-134">7 </span><span class="sxs-lookup"><span data-stu-id="dfc21-134">7</span></span>|<span data-ttu-id="dfc21-135">Устройство считается неотвечающим для системы защиты от угроз для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfc21-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="dfc21-136">Работоспособность устройства неизвестна.</span><span class="sxs-lookup"><span data-stu-id="dfc21-136">The device health is not known.</span></span>|
|<span data-ttu-id="dfc21-137">раскрыты</span><span class="sxs-lookup"><span data-stu-id="dfc21-137">compromised</span></span>|<span data-ttu-id="dfc21-138">8 </span><span class="sxs-lookup"><span data-stu-id="dfc21-138">8</span></span>|<span data-ttu-id="dfc21-139">Устройство считается скомпрометированным партнером по защите от угроз.</span><span class="sxs-lookup"><span data-stu-id="dfc21-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="dfc21-140">Это означает, что у устройства есть активная угроза или риск, который не может быть легко исправлен конечным пользователем, и пользователь должен связаться с администратором ИТ.</span><span class="sxs-lookup"><span data-stu-id="dfc21-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="dfc21-141">неправильно настроенный</span><span class="sxs-lookup"><span data-stu-id="dfc21-141">misconfigured</span></span>|<span data-ttu-id="dfc21-142">9 </span><span class="sxs-lookup"><span data-stu-id="dfc21-142">9</span></span>|<span data-ttu-id="dfc21-143">Устройство считается неправильно настроенным с помощью партнера по защите от угроз.</span><span class="sxs-lookup"><span data-stu-id="dfc21-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="dfc21-144">Это означает, что на устройстве отсутствует необходимый профиль или конфигурация для правильного функционирования партнера по защите от угроз, поэтому не удается завершить анализ угроз или риска.</span><span class="sxs-lookup"><span data-stu-id="dfc21-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|









