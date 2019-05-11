---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c60b9f2775fdad7bc9f1f2fa3ae18992fc2e4757
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946905"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="8b279-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="8b279-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="8b279-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b279-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b279-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b279-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b279-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="8b279-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="8b279-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8b279-107">Members</span></span>
|<span data-ttu-id="8b279-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8b279-108">Member</span></span>|<span data-ttu-id="8b279-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8b279-109">Value</span></span>|<span data-ttu-id="8b279-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b279-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b279-111">выходе</span><span class="sxs-lookup"><span data-stu-id="8b279-111">unavailable</span></span>|<span data-ttu-id="8b279-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8b279-112">0</span></span>|<span data-ttu-id="8b279-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b279-113">Default Value.</span></span> <span data-ttu-id="8b279-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="8b279-114">Do not use.</span></span>|
|<span data-ttu-id="8b279-115">входящего</span><span class="sxs-lookup"><span data-stu-id="8b279-115">secured</span></span>|<span data-ttu-id="8b279-116">1,1</span><span class="sxs-lookup"><span data-stu-id="8b279-116">1</span></span>|<span data-ttu-id="8b279-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="8b279-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="8b279-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="8b279-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="8b279-119">потребление</span><span class="sxs-lookup"><span data-stu-id="8b279-119">low</span></span>|<span data-ttu-id="8b279-120">2</span><span class="sxs-lookup"><span data-stu-id="8b279-120">2</span></span>|<span data-ttu-id="8b279-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="8b279-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="8b279-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="8b279-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="8b279-123">medium</span><span class="sxs-lookup"><span data-stu-id="8b279-123">medium</span></span>|<span data-ttu-id="8b279-124">4</span><span class="sxs-lookup"><span data-stu-id="8b279-124">3</span></span>|<span data-ttu-id="8b279-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="8b279-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="8b279-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="8b279-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="8b279-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="8b279-127">high</span></span>|<span data-ttu-id="8b279-128">SP4</span><span class="sxs-lookup"><span data-stu-id="8b279-128">4</span></span>|<span data-ttu-id="8b279-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="8b279-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="8b279-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="8b279-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="8b279-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="8b279-131">notSet</span></span>|<span data-ttu-id="8b279-132">10 </span><span class="sxs-lookup"><span data-stu-id="8b279-132">10</span></span>|<span data-ttu-id="8b279-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="8b279-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="8b279-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="8b279-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




