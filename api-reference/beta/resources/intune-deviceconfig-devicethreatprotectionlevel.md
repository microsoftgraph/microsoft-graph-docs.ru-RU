---
title: Тип перечисления deviceThreatProtectionLevel
description: Уровни защиты threat устройства для API защиты от угроз устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d4c17fc9883b23417a4c72ac7cc3c75512865c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948053"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="65f5a-103">Тип перечисления deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="65f5a-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="65f5a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65f5a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65f5a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65f5a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65f5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65f5a-107">Уровни защиты threat устройства для API защиты от угроз устройства.</span><span class="sxs-lookup"><span data-stu-id="65f5a-107">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="65f5a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="65f5a-108">Members</span></span>
|<span data-ttu-id="65f5a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="65f5a-109">Member</span></span>|<span data-ttu-id="65f5a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="65f5a-110">Value</span></span>|<span data-ttu-id="65f5a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65f5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f5a-112">недоступен</span><span class="sxs-lookup"><span data-stu-id="65f5a-112">unavailable</span></span>|<span data-ttu-id="65f5a-113">0</span><span class="sxs-lookup"><span data-stu-id="65f5a-113">0</span></span>|<span data-ttu-id="65f5a-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="65f5a-114">Default Value.</span></span> <span data-ttu-id="65f5a-115">Не используйте.</span><span class="sxs-lookup"><span data-stu-id="65f5a-115">Do not use.</span></span>|
|<span data-ttu-id="65f5a-116">защищенная</span><span class="sxs-lookup"><span data-stu-id="65f5a-116">secured</span></span>|<span data-ttu-id="65f5a-117">1</span><span class="sxs-lookup"><span data-stu-id="65f5a-117">1</span></span>|<span data-ttu-id="65f5a-118">Требование уровень угрозы устройств: защищены.</span><span class="sxs-lookup"><span data-stu-id="65f5a-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="65f5a-119">Это самый безопасный уровень и представляет на устройстве не найдены угроз.</span><span class="sxs-lookup"><span data-stu-id="65f5a-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="65f5a-120">Низкая</span><span class="sxs-lookup"><span data-stu-id="65f5a-120">low</span></span>|<span data-ttu-id="65f5a-121">2</span><span class="sxs-lookup"><span data-stu-id="65f5a-121">2</span></span>|<span data-ttu-id="65f5a-122">Требования к уровню защиту от угроз устройств: низкий.</span><span class="sxs-lookup"><span data-stu-id="65f5a-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="65f5a-123">Low представляет уровень серьезности угрозы, который создает минимальным риском на устройстве или устройство данных.</span><span class="sxs-lookup"><span data-stu-id="65f5a-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="65f5a-124">medium</span><span class="sxs-lookup"><span data-stu-id="65f5a-124">medium</span></span>|<span data-ttu-id="65f5a-125">3</span><span class="sxs-lookup"><span data-stu-id="65f5a-125">3</span></span>|<span data-ttu-id="65f5a-126">Требования к уровню защиту от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="65f5a-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="65f5a-127">Средний представляет уровень серьезности угрозы, что позами умеренный риск для устройства или устройства данных.</span><span class="sxs-lookup"><span data-stu-id="65f5a-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="65f5a-128">Высокая</span><span class="sxs-lookup"><span data-stu-id="65f5a-128">high</span></span>|<span data-ttu-id="65f5a-129">4</span><span class="sxs-lookup"><span data-stu-id="65f5a-129">4</span></span>|<span data-ttu-id="65f5a-130">Требования к уровню защиту от угроз устройств: высокая.</span><span class="sxs-lookup"><span data-stu-id="65f5a-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="65f5a-131">High представляет уровень серьезности угрозы, серьезные угрозы для устройства или устройства данных.</span><span class="sxs-lookup"><span data-stu-id="65f5a-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="65f5a-132">notSet</span><span class="sxs-lookup"><span data-stu-id="65f5a-132">notSet</span></span>|<span data-ttu-id="65f5a-133">10</span><span class="sxs-lookup"><span data-stu-id="65f5a-133">10</span></span>|<span data-ttu-id="65f5a-134">Требования к уровню защиту от угроз устройств: не задан.</span><span class="sxs-lookup"><span data-stu-id="65f5a-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="65f5a-135">Не набор показывает, что не является обязательным для устройства в соответствии с уровнем защиту от угроз.</span><span class="sxs-lookup"><span data-stu-id="65f5a-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





