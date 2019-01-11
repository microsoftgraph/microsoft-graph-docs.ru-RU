---
title: Тип перечисления androidRequiredPasswordType
description: Тип Android пароль.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aea7ca2448e62bc9d43da5f75b2d4605cda0f520
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855337"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="39322-103">Тип перечисления androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="39322-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="39322-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39322-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39322-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39322-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39322-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39322-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39322-107">Тип Android пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-107">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="39322-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="39322-108">Members</span></span>
|<span data-ttu-id="39322-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="39322-109">Member</span></span>|<span data-ttu-id="39322-110">Значение</span><span class="sxs-lookup"><span data-stu-id="39322-110">Value</span></span>|<span data-ttu-id="39322-111">Описание</span><span class="sxs-lookup"><span data-stu-id="39322-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39322-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="39322-112">deviceDefault</span></span>|<span data-ttu-id="39322-113">0</span><span class="sxs-lookup"><span data-stu-id="39322-113">0</span></span>|<span data-ttu-id="39322-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="39322-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="39322-115">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="39322-115">alphabetic</span></span>|<span data-ttu-id="39322-116">1</span><span class="sxs-lookup"><span data-stu-id="39322-116">1</span></span>|<span data-ttu-id="39322-117">К буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="39322-118">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="39322-118">alphanumeric</span></span>|<span data-ttu-id="39322-119">2</span><span class="sxs-lookup"><span data-stu-id="39322-119">2</span></span>|<span data-ttu-id="39322-120">Буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="39322-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="39322-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="39322-122">3</span><span class="sxs-lookup"><span data-stu-id="39322-122">3</span></span>|<span data-ttu-id="39322-123">Буквы или цифры с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="39322-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="39322-124">lowSecurityBiometric</span></span>|<span data-ttu-id="39322-125">4</span><span class="sxs-lookup"><span data-stu-id="39322-125">4</span></span>|<span data-ttu-id="39322-126">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="39322-127">числовое</span><span class="sxs-lookup"><span data-stu-id="39322-127">numeric</span></span>|<span data-ttu-id="39322-128">5</span><span class="sxs-lookup"><span data-stu-id="39322-128">5</span></span>|<span data-ttu-id="39322-129">Числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-129">Numeric password required.</span></span>|
|<span data-ttu-id="39322-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="39322-130">numericComplex</span></span>|<span data-ttu-id="39322-131">6</span><span class="sxs-lookup"><span data-stu-id="39322-131">6</span></span>|<span data-ttu-id="39322-132">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="39322-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="39322-133">любой</span><span class="sxs-lookup"><span data-stu-id="39322-133">any</span></span>|<span data-ttu-id="39322-134">7</span><span class="sxs-lookup"><span data-stu-id="39322-134">7</span></span>|<span data-ttu-id="39322-135">Пароль или шаблон является обязательным, а какие-либо допустима.</span><span class="sxs-lookup"><span data-stu-id="39322-135">A password or pattern is required, and any is acceptable.</span></span>|





