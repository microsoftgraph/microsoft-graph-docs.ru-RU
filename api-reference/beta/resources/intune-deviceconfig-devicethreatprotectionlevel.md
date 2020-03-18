---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aa69e2e4d2122a8611a0db6a277dbfd5085561ba
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791991"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="e3b45-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="e3b45-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="e3b45-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3b45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3b45-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3b45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3b45-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="e3b45-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="e3b45-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e3b45-107">Members</span></span>
|<span data-ttu-id="e3b45-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e3b45-108">Member</span></span>|<span data-ttu-id="e3b45-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e3b45-109">Value</span></span>|<span data-ttu-id="e3b45-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e3b45-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3b45-111">выходе</span><span class="sxs-lookup"><span data-stu-id="e3b45-111">unavailable</span></span>|<span data-ttu-id="e3b45-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e3b45-112">0</span></span>|<span data-ttu-id="e3b45-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e3b45-113">Default Value.</span></span> <span data-ttu-id="e3b45-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="e3b45-114">Do not use.</span></span>|
|<span data-ttu-id="e3b45-115">входящего</span><span class="sxs-lookup"><span data-stu-id="e3b45-115">secured</span></span>|<span data-ttu-id="e3b45-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e3b45-116">1</span></span>|<span data-ttu-id="e3b45-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="e3b45-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="e3b45-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="e3b45-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="e3b45-119">потребление</span><span class="sxs-lookup"><span data-stu-id="e3b45-119">low</span></span>|<span data-ttu-id="e3b45-120">2</span><span class="sxs-lookup"><span data-stu-id="e3b45-120">2</span></span>|<span data-ttu-id="e3b45-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="e3b45-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="e3b45-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="e3b45-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="e3b45-123">medium</span><span class="sxs-lookup"><span data-stu-id="e3b45-123">medium</span></span>|<span data-ttu-id="e3b45-124">4</span><span class="sxs-lookup"><span data-stu-id="e3b45-124">3</span></span>|<span data-ttu-id="e3b45-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="e3b45-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="e3b45-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="e3b45-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="e3b45-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="e3b45-127">high</span></span>|<span data-ttu-id="e3b45-128">4 </span><span class="sxs-lookup"><span data-stu-id="e3b45-128">4</span></span>|<span data-ttu-id="e3b45-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="e3b45-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="e3b45-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="e3b45-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="e3b45-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="e3b45-131">notSet</span></span>|<span data-ttu-id="e3b45-132">10 </span><span class="sxs-lookup"><span data-stu-id="e3b45-132">10</span></span>|<span data-ttu-id="e3b45-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="e3b45-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="e3b45-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="e3b45-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



