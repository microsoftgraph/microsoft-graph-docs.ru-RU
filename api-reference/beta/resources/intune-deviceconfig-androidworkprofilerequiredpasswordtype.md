---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e211fd0f793f710c31a303a73662af556c0794a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891527"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="dfc80-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dfc80-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="dfc80-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dfc80-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfc80-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfc80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfc80-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dfc80-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfc80-107">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="dfc80-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dfc80-108">Members</span></span>
|<span data-ttu-id="dfc80-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dfc80-109">Member</span></span>|<span data-ttu-id="dfc80-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dfc80-110">Value</span></span>|<span data-ttu-id="dfc80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfc80-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="dfc80-112">deviceDefault</span></span>|<span data-ttu-id="dfc80-113">0</span><span class="sxs-lookup"><span data-stu-id="dfc80-113">0</span></span>|<span data-ttu-id="dfc80-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="dfc80-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="dfc80-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="dfc80-115">lowSecurityBiometric</span></span>|<span data-ttu-id="dfc80-116">1</span><span class="sxs-lookup"><span data-stu-id="dfc80-116">1</span></span>|<span data-ttu-id="dfc80-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="dfc80-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dfc80-118">required</span></span>|<span data-ttu-id="dfc80-119">2</span><span class="sxs-lookup"><span data-stu-id="dfc80-119">2</span></span>|<span data-ttu-id="dfc80-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfc80-120">Required.</span></span>|
|<span data-ttu-id="dfc80-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="dfc80-121">atLeastNumeric</span></span>|<span data-ttu-id="dfc80-122">3</span><span class="sxs-lookup"><span data-stu-id="dfc80-122">3</span></span>|<span data-ttu-id="dfc80-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-123">At least numeric password required.</span></span>|
|<span data-ttu-id="dfc80-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="dfc80-124">numericComplex</span></span>|<span data-ttu-id="dfc80-125">4</span><span class="sxs-lookup"><span data-stu-id="dfc80-125">4</span></span>|<span data-ttu-id="dfc80-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="dfc80-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="dfc80-127">atLeastAlphabetic</span></span>|<span data-ttu-id="dfc80-128">5</span><span class="sxs-lookup"><span data-stu-id="dfc80-128">5</span></span>|<span data-ttu-id="dfc80-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="dfc80-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="dfc80-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="dfc80-131">6</span><span class="sxs-lookup"><span data-stu-id="dfc80-131">6</span></span>|<span data-ttu-id="dfc80-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="dfc80-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="dfc80-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="dfc80-134">7</span><span class="sxs-lookup"><span data-stu-id="dfc80-134">7</span></span>|<span data-ttu-id="dfc80-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="dfc80-135">At least alphanumeric with symbols password required.</span></span>|





