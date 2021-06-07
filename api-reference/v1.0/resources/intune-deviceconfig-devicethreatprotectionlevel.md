---
title: тип enum deviceThreatProtectionLevel
description: Уровни защиты от угроз устройств для API защиты от угроз устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 21147e2be838bef34bc61eb401f57e1c650028d5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755093"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="6fd32-103">тип enum deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6fd32-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="6fd32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fd32-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fd32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fd32-106">Уровни защиты от угроз устройств для API защиты от угроз устройств.</span><span class="sxs-lookup"><span data-stu-id="6fd32-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="6fd32-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6fd32-107">Members</span></span>
|<span data-ttu-id="6fd32-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6fd32-108">Member</span></span>|<span data-ttu-id="6fd32-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6fd32-109">Value</span></span>|<span data-ttu-id="6fd32-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6fd32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fd32-111">недоступно</span><span class="sxs-lookup"><span data-stu-id="6fd32-111">unavailable</span></span>|<span data-ttu-id="6fd32-112">0</span><span class="sxs-lookup"><span data-stu-id="6fd32-112">0</span></span>|<span data-ttu-id="6fd32-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6fd32-113">Default Value.</span></span> <span data-ttu-id="6fd32-114">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="6fd32-114">Do not use.</span></span>|
|<span data-ttu-id="6fd32-115">обеспечено</span><span class="sxs-lookup"><span data-stu-id="6fd32-115">secured</span></span>|<span data-ttu-id="6fd32-116">1</span><span class="sxs-lookup"><span data-stu-id="6fd32-116">1</span></span>|<span data-ttu-id="6fd32-117">Требование уровня угрозы устройства: защищено.</span><span class="sxs-lookup"><span data-stu-id="6fd32-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="6fd32-118">Это самый безопасный уровень, который представляет отсутствие угроз на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6fd32-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="6fd32-119">низкий</span><span class="sxs-lookup"><span data-stu-id="6fd32-119">low</span></span>|<span data-ttu-id="6fd32-120">2</span><span class="sxs-lookup"><span data-stu-id="6fd32-120">2</span></span>|<span data-ttu-id="6fd32-121">Требование уровня защиты от угрозы устройства: низкий.</span><span class="sxs-lookup"><span data-stu-id="6fd32-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="6fd32-122">Низкий уровень представляет серьезность угрозы, которая представляет минимальный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="6fd32-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="6fd32-123">medium</span><span class="sxs-lookup"><span data-stu-id="6fd32-123">medium</span></span>|<span data-ttu-id="6fd32-124">3</span><span class="sxs-lookup"><span data-stu-id="6fd32-124">3</span></span>|<span data-ttu-id="6fd32-125">Требование уровня защиты от угроз устройства: Medium.</span><span class="sxs-lookup"><span data-stu-id="6fd32-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="6fd32-126">Средство представляет собой степень серьезности угрозы, которая представляет умеренный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="6fd32-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="6fd32-127">высокая</span><span class="sxs-lookup"><span data-stu-id="6fd32-127">high</span></span>|<span data-ttu-id="6fd32-128">4 </span><span class="sxs-lookup"><span data-stu-id="6fd32-128">4</span></span>|<span data-ttu-id="6fd32-129">Требование уровня защиты от угрозы устройства: высокое.</span><span class="sxs-lookup"><span data-stu-id="6fd32-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="6fd32-130">Высокая представляет серьезность угрозы, которая представляет серьезный риск для данных устройства или устройства.</span><span class="sxs-lookup"><span data-stu-id="6fd32-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="6fd32-131">notSet</span><span class="sxs-lookup"><span data-stu-id="6fd32-131">notSet</span></span>|<span data-ttu-id="6fd32-132">10 </span><span class="sxs-lookup"><span data-stu-id="6fd32-132">10</span></span>|<span data-ttu-id="6fd32-133">Требование уровня защиты от угрозы устройства: Не установлено.</span><span class="sxs-lookup"><span data-stu-id="6fd32-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="6fd32-134">Не установлено, что для устройства не существует требования к уровню защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="6fd32-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




