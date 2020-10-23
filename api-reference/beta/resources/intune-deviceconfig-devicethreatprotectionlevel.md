---
title: тип перечисления Девицесреатпротектионлевел
description: Уровни защиты от угроз для устройства API защиты от угроз.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 799448f79975cfa2a4879528770f85c3e862c365
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707803"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="dcbe6-103">тип перечисления Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="dcbe6-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="dcbe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcbe6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcbe6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcbe6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcbe6-107">Уровни защиты от угроз для устройства API защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="dcbe6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dcbe6-108">Members</span></span>
|<span data-ttu-id="dcbe6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dcbe6-109">Member</span></span>|<span data-ttu-id="dcbe6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dcbe6-110">Value</span></span>|<span data-ttu-id="dcbe6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dcbe6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcbe6-112">выходе</span><span class="sxs-lookup"><span data-stu-id="dcbe6-112">unavailable</span></span>|<span data-ttu-id="dcbe6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="dcbe6-113">0</span></span>|<span data-ttu-id="dcbe6-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-114">Default Value.</span></span> <span data-ttu-id="dcbe6-115">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-115">Do not use.</span></span>|
|<span data-ttu-id="dcbe6-116">входящего</span><span class="sxs-lookup"><span data-stu-id="dcbe6-116">secured</span></span>|<span data-ttu-id="dcbe6-117">1,1</span><span class="sxs-lookup"><span data-stu-id="dcbe6-117">1</span></span>|<span data-ttu-id="dcbe6-118">Требование к уровню угроз для устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="dcbe6-119">Этот уровень является наиболее безопасным и указывает на то, что на устройстве не обнаружены угрозы.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="dcbe6-120">потребление</span><span class="sxs-lookup"><span data-stu-id="dcbe6-120">low</span></span>|<span data-ttu-id="dcbe6-121">2</span><span class="sxs-lookup"><span data-stu-id="dcbe6-121">2</span></span>|<span data-ttu-id="dcbe6-122">Требование к уровню защиты от угроз для устройства: не хватает.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="dcbe6-123">Низкие — это серьезность угрозы, которая представляет собой минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="dcbe6-124">medium</span><span class="sxs-lookup"><span data-stu-id="dcbe6-124">medium</span></span>|<span data-ttu-id="dcbe6-125">4</span><span class="sxs-lookup"><span data-stu-id="dcbe6-125">3</span></span>|<span data-ttu-id="dcbe6-126">Требования к уровню защиты от угроз устройств: Medium.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="dcbe6-127">Medium — это серьезность угрозы, которая создает умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="dcbe6-128">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="dcbe6-128">high</span></span>|<span data-ttu-id="dcbe6-129">4 </span><span class="sxs-lookup"><span data-stu-id="dcbe6-129">4</span></span>|<span data-ttu-id="dcbe6-130">Требование к уровню защиты от угроз для устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="dcbe6-131">High — это серьезность угрозы, которая создает серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="dcbe6-132">Принимать</span><span class="sxs-lookup"><span data-stu-id="dcbe6-132">notSet</span></span>|<span data-ttu-id="dcbe6-133">10 </span><span class="sxs-lookup"><span data-stu-id="dcbe6-133">10</span></span>|<span data-ttu-id="dcbe6-134">Требование к уровню защиты от угроз для устройства: не задано.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="dcbe6-135">Не задано указывает на то, что устройство не должно соответствовать уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="dcbe6-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





