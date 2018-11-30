---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
ms.openlocfilehash: f9cdf225f9fe7dfc42fb728bad615a7abde11bef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024851"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="32868-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="32868-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="32868-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32868-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32868-105">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="32868-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="32868-106">Members</span></span>
|<span data-ttu-id="32868-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="32868-107">Member</span></span>|<span data-ttu-id="32868-108">Значение</span><span class="sxs-lookup"><span data-stu-id="32868-108">Value</span></span>|<span data-ttu-id="32868-109">Description</span><span class="sxs-lookup"><span data-stu-id="32868-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32868-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="32868-110">deviceDefault</span></span>|<span data-ttu-id="32868-111">0</span><span class="sxs-lookup"><span data-stu-id="32868-111">0</span></span>|<span data-ttu-id="32868-112">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="32868-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="32868-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="32868-113">lowSecurityBiometric</span></span>|<span data-ttu-id="32868-114">1</span><span class="sxs-lookup"><span data-stu-id="32868-114">1</span></span>|<span data-ttu-id="32868-115">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="32868-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="32868-116">required</span></span>|<span data-ttu-id="32868-117">2</span><span class="sxs-lookup"><span data-stu-id="32868-117">2</span></span>|<span data-ttu-id="32868-118">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="32868-118">Required.</span></span>|
|<span data-ttu-id="32868-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="32868-119">atLeastNumeric</span></span>|<span data-ttu-id="32868-120">3</span><span class="sxs-lookup"><span data-stu-id="32868-120">3</span></span>|<span data-ttu-id="32868-121">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-121">At least numeric password required.</span></span>|
|<span data-ttu-id="32868-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="32868-122">numericComplex</span></span>|<span data-ttu-id="32868-123">4</span><span class="sxs-lookup"><span data-stu-id="32868-123">4</span></span>|<span data-ttu-id="32868-124">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="32868-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="32868-125">atLeastAlphabetic</span></span>|<span data-ttu-id="32868-126">5</span><span class="sxs-lookup"><span data-stu-id="32868-126">5</span></span>|<span data-ttu-id="32868-127">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="32868-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="32868-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="32868-129">6</span><span class="sxs-lookup"><span data-stu-id="32868-129">6</span></span>|<span data-ttu-id="32868-130">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="32868-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="32868-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="32868-132">7</span><span class="sxs-lookup"><span data-stu-id="32868-132">7</span></span>|<span data-ttu-id="32868-133">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="32868-133">At least alphanumeric with symbols password required.</span></span>|



