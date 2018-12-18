---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
author: tfitzmac
ms.openlocfilehash: 8d41b4c516ee4aa393ea3a26034e5f575b58fa02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330235"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="29e4f-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="29e4f-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="29e4f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29e4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29e4f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29e4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29e4f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29e4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29e4f-107">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-107">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="29e4f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="29e4f-108">Members</span></span>
|<span data-ttu-id="29e4f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="29e4f-109">Member</span></span>|<span data-ttu-id="29e4f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="29e4f-110">Value</span></span>|<span data-ttu-id="29e4f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="29e4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e4f-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="29e4f-112">deviceDefault</span></span>|<span data-ttu-id="29e4f-113">0</span><span class="sxs-lookup"><span data-stu-id="29e4f-113">0</span></span>|<span data-ttu-id="29e4f-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="29e4f-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="29e4f-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="29e4f-115">lowSecurityBiometric</span></span>|<span data-ttu-id="29e4f-116">1</span><span class="sxs-lookup"><span data-stu-id="29e4f-116">1</span></span>|<span data-ttu-id="29e4f-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="29e4f-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="29e4f-118">required</span></span>|<span data-ttu-id="29e4f-119">2</span><span class="sxs-lookup"><span data-stu-id="29e4f-119">2</span></span>|<span data-ttu-id="29e4f-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29e4f-120">Required.</span></span>|
|<span data-ttu-id="29e4f-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="29e4f-121">atLeastNumeric</span></span>|<span data-ttu-id="29e4f-122">3</span><span class="sxs-lookup"><span data-stu-id="29e4f-122">3</span></span>|<span data-ttu-id="29e4f-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-123">At least numeric password required.</span></span>|
|<span data-ttu-id="29e4f-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="29e4f-124">numericComplex</span></span>|<span data-ttu-id="29e4f-125">4</span><span class="sxs-lookup"><span data-stu-id="29e4f-125">4</span></span>|<span data-ttu-id="29e4f-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="29e4f-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="29e4f-127">atLeastAlphabetic</span></span>|<span data-ttu-id="29e4f-128">5</span><span class="sxs-lookup"><span data-stu-id="29e4f-128">5</span></span>|<span data-ttu-id="29e4f-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="29e4f-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="29e4f-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="29e4f-131">6</span><span class="sxs-lookup"><span data-stu-id="29e4f-131">6</span></span>|<span data-ttu-id="29e4f-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="29e4f-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="29e4f-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="29e4f-134">7</span><span class="sxs-lookup"><span data-stu-id="29e4f-134">7</span></span>|<span data-ttu-id="29e4f-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="29e4f-135">At least alphanumeric with symbols password required.</span></span>|





