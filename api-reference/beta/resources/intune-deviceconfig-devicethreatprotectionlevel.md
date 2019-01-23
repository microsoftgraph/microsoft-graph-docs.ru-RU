---
title: Тип перечисления deviceThreatProtectionLevel
description: Уровни защиты threat устройства для API защиты от угроз устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411234"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="c6feb-103">Тип перечисления deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c6feb-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="c6feb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6feb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c6feb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6feb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6feb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6feb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6feb-107">Уровни защиты threat устройства для API защиты от угроз устройства.</span><span class="sxs-lookup"><span data-stu-id="c6feb-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="c6feb-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c6feb-108">Members</span></span>
|<span data-ttu-id="c6feb-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c6feb-109">Member</span></span>|<span data-ttu-id="c6feb-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c6feb-110">Value</span></span>|<span data-ttu-id="c6feb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c6feb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6feb-112">недоступен</span><span class="sxs-lookup"><span data-stu-id="c6feb-112">unavailable</span></span>|<span data-ttu-id="c6feb-113">0</span><span class="sxs-lookup"><span data-stu-id="c6feb-113">0</span></span>|<span data-ttu-id="c6feb-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c6feb-114">Default Value.</span></span> <span data-ttu-id="c6feb-115">Не используйте.</span><span class="sxs-lookup"><span data-stu-id="c6feb-115">Do not use.</span></span>|
|<span data-ttu-id="c6feb-116">защищенная</span><span class="sxs-lookup"><span data-stu-id="c6feb-116">secured</span></span>|<span data-ttu-id="c6feb-117">1</span><span class="sxs-lookup"><span data-stu-id="c6feb-117">1</span></span>|<span data-ttu-id="c6feb-118">Требование уровень угрозы устройств: защищены.</span><span class="sxs-lookup"><span data-stu-id="c6feb-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="c6feb-119">Это самый безопасный уровень и представляет на устройстве не найдены угроз.</span><span class="sxs-lookup"><span data-stu-id="c6feb-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="c6feb-120">Низкая</span><span class="sxs-lookup"><span data-stu-id="c6feb-120">low</span></span>|<span data-ttu-id="c6feb-121">2</span><span class="sxs-lookup"><span data-stu-id="c6feb-121">2</span></span>|<span data-ttu-id="c6feb-122">Требования к уровню защиту от угроз устройств: низкий.</span><span class="sxs-lookup"><span data-stu-id="c6feb-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="c6feb-123">Low представляет уровень серьезности угрозы, который создает минимальным риском на устройстве или устройство данных.</span><span class="sxs-lookup"><span data-stu-id="c6feb-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="c6feb-124">medium</span><span class="sxs-lookup"><span data-stu-id="c6feb-124">medium</span></span>|<span data-ttu-id="c6feb-125">3</span><span class="sxs-lookup"><span data-stu-id="c6feb-125">3</span></span>|<span data-ttu-id="c6feb-126">Требования к уровню защиту от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="c6feb-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="c6feb-127">Средний представляет уровень серьезности угрозы, что позами умеренный риск для устройства или устройства данных.</span><span class="sxs-lookup"><span data-stu-id="c6feb-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="c6feb-128">Высокая</span><span class="sxs-lookup"><span data-stu-id="c6feb-128">high</span></span>|<span data-ttu-id="c6feb-129">4</span><span class="sxs-lookup"><span data-stu-id="c6feb-129">4</span></span>|<span data-ttu-id="c6feb-130">Требования к уровню защиту от угроз устройств: высокая.</span><span class="sxs-lookup"><span data-stu-id="c6feb-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="c6feb-131">High представляет уровень серьезности угрозы, серьезные угрозы для устройства или устройства данных.</span><span class="sxs-lookup"><span data-stu-id="c6feb-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="c6feb-132">notSet</span><span class="sxs-lookup"><span data-stu-id="c6feb-132">notSet</span></span>|<span data-ttu-id="c6feb-133">10</span><span class="sxs-lookup"><span data-stu-id="c6feb-133">10</span></span>|<span data-ttu-id="c6feb-134">Требования к уровню защиту от угроз устройств: не задан.</span><span class="sxs-lookup"><span data-stu-id="c6feb-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="c6feb-135">Не набор показывает, что не является обязательным для устройства в соответствии с уровнем защиту от угроз.</span><span class="sxs-lookup"><span data-stu-id="c6feb-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




