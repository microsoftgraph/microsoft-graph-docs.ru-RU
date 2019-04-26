---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af0231e15cfa815d3fd2e154adf180f3e0c0c43
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566817"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="28f81-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="28f81-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="28f81-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28f81-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28f81-105">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="28f81-105">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="28f81-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="28f81-106">Members</span></span>
|<span data-ttu-id="28f81-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="28f81-107">Member</span></span>|<span data-ttu-id="28f81-108">Значение</span><span class="sxs-lookup"><span data-stu-id="28f81-108">Value</span></span>|<span data-ttu-id="28f81-109">Описание</span><span class="sxs-lookup"><span data-stu-id="28f81-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28f81-110">выходе</span><span class="sxs-lookup"><span data-stu-id="28f81-110">unavailable</span></span>|<span data-ttu-id="28f81-111">нуль</span><span class="sxs-lookup"><span data-stu-id="28f81-111">0</span></span>|<span data-ttu-id="28f81-112">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="28f81-112">Default Value.</span></span> <span data-ttu-id="28f81-113">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="28f81-113">Do not use.</span></span>|
|<span data-ttu-id="28f81-114">входящего</span><span class="sxs-lookup"><span data-stu-id="28f81-114">secured</span></span>|<span data-ttu-id="28f81-115">1 </span><span class="sxs-lookup"><span data-stu-id="28f81-115">1</span></span>|<span data-ttu-id="28f81-116">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="28f81-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="28f81-117">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="28f81-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="28f81-118">потребление</span><span class="sxs-lookup"><span data-stu-id="28f81-118">low</span></span>|<span data-ttu-id="28f81-119">2 </span><span class="sxs-lookup"><span data-stu-id="28f81-119">2</span></span>|<span data-ttu-id="28f81-120">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="28f81-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="28f81-121">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="28f81-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="28f81-122">medium</span><span class="sxs-lookup"><span data-stu-id="28f81-122">medium</span></span>|<span data-ttu-id="28f81-123">3 </span><span class="sxs-lookup"><span data-stu-id="28f81-123">3</span></span>|<span data-ttu-id="28f81-124">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="28f81-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="28f81-125">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="28f81-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="28f81-126">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="28f81-126">high</span></span>|<span data-ttu-id="28f81-127">4 </span><span class="sxs-lookup"><span data-stu-id="28f81-127">4</span></span>|<span data-ttu-id="28f81-128">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="28f81-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="28f81-129">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="28f81-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="28f81-130">Принимать</span><span class="sxs-lookup"><span data-stu-id="28f81-130">notSet</span></span>|<span data-ttu-id="28f81-131">10 </span><span class="sxs-lookup"><span data-stu-id="28f81-131">10</span></span>|<span data-ttu-id="28f81-132">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="28f81-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="28f81-133">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="28f81-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



