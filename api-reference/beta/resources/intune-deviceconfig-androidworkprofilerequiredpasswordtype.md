---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 97820113cda826a97d5bac5854577d4b4434eb57
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912234"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="80eb9-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80eb9-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="80eb9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="80eb9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80eb9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80eb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80eb9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="80eb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80eb9-107">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="80eb9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="80eb9-108">Members</span></span>
|<span data-ttu-id="80eb9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="80eb9-109">Member</span></span>|<span data-ttu-id="80eb9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="80eb9-110">Value</span></span>|<span data-ttu-id="80eb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="80eb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80eb9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="80eb9-112">deviceDefault</span></span>|<span data-ttu-id="80eb9-113">0</span><span class="sxs-lookup"><span data-stu-id="80eb9-113">0</span></span>|<span data-ttu-id="80eb9-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="80eb9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="80eb9-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="80eb9-115">lowSecurityBiometric</span></span>|<span data-ttu-id="80eb9-116">1</span><span class="sxs-lookup"><span data-stu-id="80eb9-116">1</span></span>|<span data-ttu-id="80eb9-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="80eb9-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="80eb9-118">required</span></span>|<span data-ttu-id="80eb9-119">2</span><span class="sxs-lookup"><span data-stu-id="80eb9-119">2</span></span>|<span data-ttu-id="80eb9-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80eb9-120">Required.</span></span>|
|<span data-ttu-id="80eb9-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="80eb9-121">atLeastNumeric</span></span>|<span data-ttu-id="80eb9-122">3</span><span class="sxs-lookup"><span data-stu-id="80eb9-122">3</span></span>|<span data-ttu-id="80eb9-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-123">At least numeric password required.</span></span>|
|<span data-ttu-id="80eb9-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="80eb9-124">numericComplex</span></span>|<span data-ttu-id="80eb9-125">4</span><span class="sxs-lookup"><span data-stu-id="80eb9-125">4</span></span>|<span data-ttu-id="80eb9-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="80eb9-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="80eb9-127">atLeastAlphabetic</span></span>|<span data-ttu-id="80eb9-128">5</span><span class="sxs-lookup"><span data-stu-id="80eb9-128">5</span></span>|<span data-ttu-id="80eb9-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="80eb9-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="80eb9-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="80eb9-131">6</span><span class="sxs-lookup"><span data-stu-id="80eb9-131">6</span></span>|<span data-ttu-id="80eb9-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="80eb9-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="80eb9-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="80eb9-134">7</span><span class="sxs-lookup"><span data-stu-id="80eb9-134">7</span></span>|<span data-ttu-id="80eb9-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="80eb9-135">At least alphanumeric with symbols password required.</span></span>|





