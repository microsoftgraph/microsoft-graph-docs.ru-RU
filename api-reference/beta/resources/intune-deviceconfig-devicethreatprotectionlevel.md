---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 311a2e9a8db68d41d3c4a55f9691446b4e96c2d3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796173"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="dff65-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="dff65-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="dff65-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dff65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dff65-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dff65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dff65-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="dff65-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="dff65-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dff65-107">Members</span></span>
|<span data-ttu-id="dff65-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dff65-108">Member</span></span>|<span data-ttu-id="dff65-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dff65-109">Value</span></span>|<span data-ttu-id="dff65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dff65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff65-111">выходе</span><span class="sxs-lookup"><span data-stu-id="dff65-111">unavailable</span></span>|<span data-ttu-id="dff65-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dff65-112">0</span></span>|<span data-ttu-id="dff65-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dff65-113">Default Value.</span></span> <span data-ttu-id="dff65-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="dff65-114">Do not use.</span></span>|
|<span data-ttu-id="dff65-115">входящего</span><span class="sxs-lookup"><span data-stu-id="dff65-115">secured</span></span>|<span data-ttu-id="dff65-116">1,1</span><span class="sxs-lookup"><span data-stu-id="dff65-116">1</span></span>|<span data-ttu-id="dff65-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="dff65-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="dff65-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="dff65-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="dff65-119">потребление</span><span class="sxs-lookup"><span data-stu-id="dff65-119">low</span></span>|<span data-ttu-id="dff65-120">2</span><span class="sxs-lookup"><span data-stu-id="dff65-120">2</span></span>|<span data-ttu-id="dff65-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="dff65-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="dff65-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="dff65-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="dff65-123">medium</span><span class="sxs-lookup"><span data-stu-id="dff65-123">medium</span></span>|<span data-ttu-id="dff65-124">4</span><span class="sxs-lookup"><span data-stu-id="dff65-124">3</span></span>|<span data-ttu-id="dff65-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="dff65-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="dff65-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="dff65-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="dff65-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="dff65-127">high</span></span>|<span data-ttu-id="dff65-128">SP4</span><span class="sxs-lookup"><span data-stu-id="dff65-128">4</span></span>|<span data-ttu-id="dff65-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="dff65-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="dff65-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="dff65-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="dff65-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="dff65-131">notSet</span></span>|<span data-ttu-id="dff65-132">десяти</span><span class="sxs-lookup"><span data-stu-id="dff65-132">10</span></span>|<span data-ttu-id="dff65-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="dff65-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="dff65-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="dff65-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





