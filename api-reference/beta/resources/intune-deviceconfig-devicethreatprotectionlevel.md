---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 895e8bd056c688ed26ba5fe57c688c66ab6ac846
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989961"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="bea41-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="bea41-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="bea41-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bea41-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bea41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea41-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="bea41-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="bea41-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bea41-107">Members</span></span>
|<span data-ttu-id="bea41-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bea41-108">Member</span></span>|<span data-ttu-id="bea41-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bea41-109">Value</span></span>|<span data-ttu-id="bea41-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bea41-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea41-111">выходе</span><span class="sxs-lookup"><span data-stu-id="bea41-111">unavailable</span></span>|<span data-ttu-id="bea41-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bea41-112">0</span></span>|<span data-ttu-id="bea41-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bea41-113">Default Value.</span></span> <span data-ttu-id="bea41-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="bea41-114">Do not use.</span></span>|
|<span data-ttu-id="bea41-115">входящего</span><span class="sxs-lookup"><span data-stu-id="bea41-115">secured</span></span>|<span data-ttu-id="bea41-116">1,1</span><span class="sxs-lookup"><span data-stu-id="bea41-116">1</span></span>|<span data-ttu-id="bea41-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="bea41-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="bea41-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="bea41-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="bea41-119">потребление</span><span class="sxs-lookup"><span data-stu-id="bea41-119">low</span></span>|<span data-ttu-id="bea41-120">2</span><span class="sxs-lookup"><span data-stu-id="bea41-120">2</span></span>|<span data-ttu-id="bea41-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="bea41-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="bea41-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="bea41-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="bea41-123">medium</span><span class="sxs-lookup"><span data-stu-id="bea41-123">medium</span></span>|<span data-ttu-id="bea41-124">4</span><span class="sxs-lookup"><span data-stu-id="bea41-124">3</span></span>|<span data-ttu-id="bea41-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="bea41-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="bea41-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="bea41-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="bea41-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="bea41-127">high</span></span>|<span data-ttu-id="bea41-128">SP4</span><span class="sxs-lookup"><span data-stu-id="bea41-128">4</span></span>|<span data-ttu-id="bea41-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="bea41-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="bea41-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="bea41-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="bea41-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="bea41-131">notSet</span></span>|<span data-ttu-id="bea41-132">10 </span><span class="sxs-lookup"><span data-stu-id="bea41-132">10</span></span>|<span data-ttu-id="bea41-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="bea41-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="bea41-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="bea41-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





