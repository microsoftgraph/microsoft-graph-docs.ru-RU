---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ecdf54051b1545b842cbc3c49359b9a77f12e2e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140245"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="5bf27-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="5bf27-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="5bf27-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bf27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bf27-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bf27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bf27-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="5bf27-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="5bf27-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5bf27-107">Members</span></span>
|<span data-ttu-id="5bf27-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5bf27-108">Member</span></span>|<span data-ttu-id="5bf27-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5bf27-109">Value</span></span>|<span data-ttu-id="5bf27-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bf27-111">выходе</span><span class="sxs-lookup"><span data-stu-id="5bf27-111">unavailable</span></span>|<span data-ttu-id="5bf27-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5bf27-112">0</span></span>|<span data-ttu-id="5bf27-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5bf27-113">Default Value.</span></span> <span data-ttu-id="5bf27-114">Не используйте.</span><span class="sxs-lookup"><span data-stu-id="5bf27-114">Do not use.</span></span>|
|<span data-ttu-id="5bf27-115">входящего</span><span class="sxs-lookup"><span data-stu-id="5bf27-115">secured</span></span>|<span data-ttu-id="5bf27-116">1,1</span><span class="sxs-lookup"><span data-stu-id="5bf27-116">1</span></span>|<span data-ttu-id="5bf27-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="5bf27-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="5bf27-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="5bf27-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="5bf27-119">потребление</span><span class="sxs-lookup"><span data-stu-id="5bf27-119">low</span></span>|<span data-ttu-id="5bf27-120">2</span><span class="sxs-lookup"><span data-stu-id="5bf27-120">2</span></span>|<span data-ttu-id="5bf27-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="5bf27-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="5bf27-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="5bf27-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="5bf27-123">medium</span><span class="sxs-lookup"><span data-stu-id="5bf27-123">medium</span></span>|<span data-ttu-id="5bf27-124">4</span><span class="sxs-lookup"><span data-stu-id="5bf27-124">3</span></span>|<span data-ttu-id="5bf27-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="5bf27-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="5bf27-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="5bf27-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="5bf27-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="5bf27-127">high</span></span>|<span data-ttu-id="5bf27-128">4</span><span class="sxs-lookup"><span data-stu-id="5bf27-128">4</span></span>|<span data-ttu-id="5bf27-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="5bf27-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="5bf27-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="5bf27-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="5bf27-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="5bf27-131">notSet</span></span>|<span data-ttu-id="5bf27-132">десяти</span><span class="sxs-lookup"><span data-stu-id="5bf27-132">10</span></span>|<span data-ttu-id="5bf27-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="5bf27-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="5bf27-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="5bf27-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




