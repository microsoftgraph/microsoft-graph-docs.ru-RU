---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69398df9bd84b9a0cd965fc26aaddee57cde174b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43465705"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="77e80-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="77e80-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="77e80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77e80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77e80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77e80-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="77e80-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="77e80-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="77e80-107">Members</span></span>
|<span data-ttu-id="77e80-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="77e80-108">Member</span></span>|<span data-ttu-id="77e80-109">Значение</span><span class="sxs-lookup"><span data-stu-id="77e80-109">Value</span></span>|<span data-ttu-id="77e80-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77e80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77e80-111">выходе</span><span class="sxs-lookup"><span data-stu-id="77e80-111">unavailable</span></span>|<span data-ttu-id="77e80-112">нуль</span><span class="sxs-lookup"><span data-stu-id="77e80-112">0</span></span>|<span data-ttu-id="77e80-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="77e80-113">Default Value.</span></span> <span data-ttu-id="77e80-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="77e80-114">Do not use.</span></span>|
|<span data-ttu-id="77e80-115">входящего</span><span class="sxs-lookup"><span data-stu-id="77e80-115">secured</span></span>|<span data-ttu-id="77e80-116">1 </span><span class="sxs-lookup"><span data-stu-id="77e80-116">1</span></span>|<span data-ttu-id="77e80-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="77e80-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="77e80-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="77e80-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="77e80-119">потребление</span><span class="sxs-lookup"><span data-stu-id="77e80-119">low</span></span>|<span data-ttu-id="77e80-120">2 </span><span class="sxs-lookup"><span data-stu-id="77e80-120">2</span></span>|<span data-ttu-id="77e80-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="77e80-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="77e80-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="77e80-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="77e80-123">medium</span><span class="sxs-lookup"><span data-stu-id="77e80-123">medium</span></span>|<span data-ttu-id="77e80-124">4</span><span class="sxs-lookup"><span data-stu-id="77e80-124">3</span></span>|<span data-ttu-id="77e80-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="77e80-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="77e80-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="77e80-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="77e80-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="77e80-127">high</span></span>|<span data-ttu-id="77e80-128">4 </span><span class="sxs-lookup"><span data-stu-id="77e80-128">4</span></span>|<span data-ttu-id="77e80-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="77e80-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="77e80-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="77e80-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="77e80-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="77e80-131">notSet</span></span>|<span data-ttu-id="77e80-132">10 </span><span class="sxs-lookup"><span data-stu-id="77e80-132">10</span></span>|<span data-ttu-id="77e80-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="77e80-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="77e80-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="77e80-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|







