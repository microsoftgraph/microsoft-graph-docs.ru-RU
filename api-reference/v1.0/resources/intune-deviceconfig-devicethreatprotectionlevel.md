---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 37de38cd6b6a459546596d68acdadf7a9bc9d489
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056837"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="1b6d1-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="1b6d1-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="1b6d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b6d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b6d1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b6d1-106">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="1b6d1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1b6d1-107">Members</span></span>
|<span data-ttu-id="1b6d1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1b6d1-108">Member</span></span>|<span data-ttu-id="1b6d1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1b6d1-109">Value</span></span>|<span data-ttu-id="1b6d1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b6d1-111">выходе</span><span class="sxs-lookup"><span data-stu-id="1b6d1-111">unavailable</span></span>|<span data-ttu-id="1b6d1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1b6d1-112">0</span></span>|<span data-ttu-id="1b6d1-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-113">Default Value.</span></span> <span data-ttu-id="1b6d1-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-114">Do not use.</span></span>|
|<span data-ttu-id="1b6d1-115">входящего</span><span class="sxs-lookup"><span data-stu-id="1b6d1-115">secured</span></span>|<span data-ttu-id="1b6d1-116">1 </span><span class="sxs-lookup"><span data-stu-id="1b6d1-116">1</span></span>|<span data-ttu-id="1b6d1-117">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="1b6d1-118">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="1b6d1-119">потребление</span><span class="sxs-lookup"><span data-stu-id="1b6d1-119">low</span></span>|<span data-ttu-id="1b6d1-120">2 </span><span class="sxs-lookup"><span data-stu-id="1b6d1-120">2</span></span>|<span data-ttu-id="1b6d1-121">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="1b6d1-122">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="1b6d1-123">medium</span><span class="sxs-lookup"><span data-stu-id="1b6d1-123">medium</span></span>|<span data-ttu-id="1b6d1-124">4</span><span class="sxs-lookup"><span data-stu-id="1b6d1-124">3</span></span>|<span data-ttu-id="1b6d1-125">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="1b6d1-126">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="1b6d1-127">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="1b6d1-127">high</span></span>|<span data-ttu-id="1b6d1-128">4 </span><span class="sxs-lookup"><span data-stu-id="1b6d1-128">4</span></span>|<span data-ttu-id="1b6d1-129">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="1b6d1-130">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="1b6d1-131">Принимать</span><span class="sxs-lookup"><span data-stu-id="1b6d1-131">notSet</span></span>|<span data-ttu-id="1b6d1-132">10 </span><span class="sxs-lookup"><span data-stu-id="1b6d1-132">10</span></span>|<span data-ttu-id="1b6d1-133">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="1b6d1-134">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="1b6d1-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|









