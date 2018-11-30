---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
ms.openlocfilehash: 8dee8332155cd3d0ba94424090df94d07f214d18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080491"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="7bea0-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7bea0-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="7bea0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7bea0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bea0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bea0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bea0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7bea0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bea0-107">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="7bea0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7bea0-108">Members</span></span>
|<span data-ttu-id="7bea0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7bea0-109">Member</span></span>|<span data-ttu-id="7bea0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7bea0-110">Value</span></span>|<span data-ttu-id="7bea0-111">Description</span><span class="sxs-lookup"><span data-stu-id="7bea0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bea0-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7bea0-112">deviceDefault</span></span>|<span data-ttu-id="7bea0-113">0</span><span class="sxs-lookup"><span data-stu-id="7bea0-113">0</span></span>|<span data-ttu-id="7bea0-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="7bea0-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="7bea0-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="7bea0-115">lowSecurityBiometric</span></span>|<span data-ttu-id="7bea0-116">1</span><span class="sxs-lookup"><span data-stu-id="7bea0-116">1</span></span>|<span data-ttu-id="7bea0-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="7bea0-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="7bea0-118">required</span></span>|<span data-ttu-id="7bea0-119">2</span><span class="sxs-lookup"><span data-stu-id="7bea0-119">2</span></span>|<span data-ttu-id="7bea0-120">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="7bea0-120">Required.</span></span>|
|<span data-ttu-id="7bea0-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="7bea0-121">atLeastNumeric</span></span>|<span data-ttu-id="7bea0-122">3</span><span class="sxs-lookup"><span data-stu-id="7bea0-122">3</span></span>|<span data-ttu-id="7bea0-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-123">At least numeric password required.</span></span>|
|<span data-ttu-id="7bea0-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="7bea0-124">numericComplex</span></span>|<span data-ttu-id="7bea0-125">4</span><span class="sxs-lookup"><span data-stu-id="7bea0-125">4</span></span>|<span data-ttu-id="7bea0-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="7bea0-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="7bea0-127">atLeastAlphabetic</span></span>|<span data-ttu-id="7bea0-128">5</span><span class="sxs-lookup"><span data-stu-id="7bea0-128">5</span></span>|<span data-ttu-id="7bea0-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="7bea0-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="7bea0-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="7bea0-131">6</span><span class="sxs-lookup"><span data-stu-id="7bea0-131">6</span></span>|<span data-ttu-id="7bea0-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="7bea0-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="7bea0-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="7bea0-134">7</span><span class="sxs-lookup"><span data-stu-id="7bea0-134">7</span></span>|<span data-ttu-id="7bea0-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="7bea0-135">At least alphanumeric with symbols password required.</span></span>|





