---
title: Тип перечисления androidRequiredPasswordType
description: Тип Android пароль.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc82ccd0519196495839f533dc09264525ac7fec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957552"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="cc090-103">Тип перечисления androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cc090-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="cc090-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc090-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc090-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc090-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc090-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cc090-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc090-107">Тип Android пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-107">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="cc090-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cc090-108">Members</span></span>
|<span data-ttu-id="cc090-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cc090-109">Member</span></span>|<span data-ttu-id="cc090-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cc090-110">Value</span></span>|<span data-ttu-id="cc090-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc090-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc090-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="cc090-112">deviceDefault</span></span>|<span data-ttu-id="cc090-113">0</span><span class="sxs-lookup"><span data-stu-id="cc090-113">0</span></span>|<span data-ttu-id="cc090-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="cc090-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="cc090-115">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="cc090-115">alphabetic</span></span>|<span data-ttu-id="cc090-116">1</span><span class="sxs-lookup"><span data-stu-id="cc090-116">1</span></span>|<span data-ttu-id="cc090-117">К буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="cc090-118">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="cc090-118">alphanumeric</span></span>|<span data-ttu-id="cc090-119">2</span><span class="sxs-lookup"><span data-stu-id="cc090-119">2</span></span>|<span data-ttu-id="cc090-120">Буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="cc090-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="cc090-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="cc090-122">3</span><span class="sxs-lookup"><span data-stu-id="cc090-122">3</span></span>|<span data-ttu-id="cc090-123">Буквы или цифры с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="cc090-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="cc090-124">lowSecurityBiometric</span></span>|<span data-ttu-id="cc090-125">4</span><span class="sxs-lookup"><span data-stu-id="cc090-125">4</span></span>|<span data-ttu-id="cc090-126">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="cc090-127">числовое</span><span class="sxs-lookup"><span data-stu-id="cc090-127">numeric</span></span>|<span data-ttu-id="cc090-128">5</span><span class="sxs-lookup"><span data-stu-id="cc090-128">5</span></span>|<span data-ttu-id="cc090-129">Числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-129">Numeric password required.</span></span>|
|<span data-ttu-id="cc090-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="cc090-130">numericComplex</span></span>|<span data-ttu-id="cc090-131">6</span><span class="sxs-lookup"><span data-stu-id="cc090-131">6</span></span>|<span data-ttu-id="cc090-132">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="cc090-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="cc090-133">любой</span><span class="sxs-lookup"><span data-stu-id="cc090-133">any</span></span>|<span data-ttu-id="cc090-134">7</span><span class="sxs-lookup"><span data-stu-id="cc090-134">7</span></span>|<span data-ttu-id="cc090-135">Пароль или шаблон является обязательным, а какие-либо допустима.</span><span class="sxs-lookup"><span data-stu-id="cc090-135">A password or pattern is required, and any is acceptable.</span></span>|





