---
title: Тип перечисления androidForWorkRequiredPasswordType
description: Android для работы требуется тип пароль.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cc944cf87e9a8daa5c50f31fbb095f09dbee1a65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933584"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="f756c-103">Тип перечисления androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f756c-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f756c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f756c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f756c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f756c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f756c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f756c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f756c-107">Android для работы требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-107">Android For Work required password type.</span></span>
## <a name="members"></a><span data-ttu-id="f756c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f756c-108">Members</span></span>
|<span data-ttu-id="f756c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f756c-109">Member</span></span>|<span data-ttu-id="f756c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f756c-110">Value</span></span>|<span data-ttu-id="f756c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f756c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f756c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f756c-112">deviceDefault</span></span>|<span data-ttu-id="f756c-113">0</span><span class="sxs-lookup"><span data-stu-id="f756c-113">0</span></span>|<span data-ttu-id="f756c-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="f756c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f756c-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="f756c-115">lowSecurityBiometric</span></span>|<span data-ttu-id="f756c-116">1</span><span class="sxs-lookup"><span data-stu-id="f756c-116">1</span></span>|<span data-ttu-id="f756c-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f756c-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f756c-118">required</span></span>|<span data-ttu-id="f756c-119">2</span><span class="sxs-lookup"><span data-stu-id="f756c-119">2</span></span>|<span data-ttu-id="f756c-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f756c-120">Required.</span></span>|
|<span data-ttu-id="f756c-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="f756c-121">atLeastNumeric</span></span>|<span data-ttu-id="f756c-122">3</span><span class="sxs-lookup"><span data-stu-id="f756c-122">3</span></span>|<span data-ttu-id="f756c-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-123">At least numeric password required.</span></span>|
|<span data-ttu-id="f756c-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f756c-124">numericComplex</span></span>|<span data-ttu-id="f756c-125">4</span><span class="sxs-lookup"><span data-stu-id="f756c-125">4</span></span>|<span data-ttu-id="f756c-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="f756c-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="f756c-127">atLeastAlphabetic</span></span>|<span data-ttu-id="f756c-128">5</span><span class="sxs-lookup"><span data-stu-id="f756c-128">5</span></span>|<span data-ttu-id="f756c-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="f756c-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="f756c-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="f756c-131">6</span><span class="sxs-lookup"><span data-stu-id="f756c-131">6</span></span>|<span data-ttu-id="f756c-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="f756c-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f756c-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="f756c-134">7</span><span class="sxs-lookup"><span data-stu-id="f756c-134">7</span></span>|<span data-ttu-id="f756c-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="f756c-135">At least alphanumeric with symbols password required.</span></span>|





