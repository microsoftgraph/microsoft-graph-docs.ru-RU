---
title: Тип перечисления androidForWorkRequiredPasswordType
description: Android для работы требуется тип пароль.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3da48449de63fa134c68e3f27fd415c286666e4e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419606"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="5153b-103">Тип перечисления androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5153b-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="5153b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5153b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5153b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5153b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5153b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5153b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5153b-107">Android для работы требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="5153b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5153b-108">Members</span></span>
|<span data-ttu-id="5153b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5153b-109">Member</span></span>|<span data-ttu-id="5153b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5153b-110">Value</span></span>|<span data-ttu-id="5153b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5153b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5153b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5153b-112">deviceDefault</span></span>|<span data-ttu-id="5153b-113">0</span><span class="sxs-lookup"><span data-stu-id="5153b-113">0</span></span>|<span data-ttu-id="5153b-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="5153b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="5153b-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="5153b-115">lowSecurityBiometric</span></span>|<span data-ttu-id="5153b-116">1</span><span class="sxs-lookup"><span data-stu-id="5153b-116">1</span></span>|<span data-ttu-id="5153b-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="5153b-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="5153b-118">required</span></span>|<span data-ttu-id="5153b-119">2</span><span class="sxs-lookup"><span data-stu-id="5153b-119">2</span></span>|<span data-ttu-id="5153b-120">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="5153b-120">Required.</span></span>|
|<span data-ttu-id="5153b-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="5153b-121">atLeastNumeric</span></span>|<span data-ttu-id="5153b-122">3</span><span class="sxs-lookup"><span data-stu-id="5153b-122">3</span></span>|<span data-ttu-id="5153b-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-123">At least numeric password required.</span></span>|
|<span data-ttu-id="5153b-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="5153b-124">numericComplex</span></span>|<span data-ttu-id="5153b-125">4</span><span class="sxs-lookup"><span data-stu-id="5153b-125">4</span></span>|<span data-ttu-id="5153b-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="5153b-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="5153b-127">atLeastAlphabetic</span></span>|<span data-ttu-id="5153b-128">5</span><span class="sxs-lookup"><span data-stu-id="5153b-128">5</span></span>|<span data-ttu-id="5153b-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="5153b-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="5153b-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="5153b-131">6</span><span class="sxs-lookup"><span data-stu-id="5153b-131">6</span></span>|<span data-ttu-id="5153b-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="5153b-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="5153b-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="5153b-134">7</span><span class="sxs-lookup"><span data-stu-id="5153b-134">7</span></span>|<span data-ttu-id="5153b-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="5153b-135">At least alphanumeric with symbols password required.</span></span>|




