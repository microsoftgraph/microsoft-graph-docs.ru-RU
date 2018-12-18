---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
author: tfitzmac
ms.openlocfilehash: 64b5dfcd5b919a428ef6823856dbf67102a316c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331663"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="915fa-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="915fa-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="915fa-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="915fa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="915fa-105">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="915fa-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="915fa-106">Members</span></span>
|<span data-ttu-id="915fa-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="915fa-107">Member</span></span>|<span data-ttu-id="915fa-108">Значение</span><span class="sxs-lookup"><span data-stu-id="915fa-108">Value</span></span>|<span data-ttu-id="915fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="915fa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="915fa-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="915fa-110">deviceDefault</span></span>|<span data-ttu-id="915fa-111">0</span><span class="sxs-lookup"><span data-stu-id="915fa-111">0</span></span>|<span data-ttu-id="915fa-112">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="915fa-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="915fa-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="915fa-113">lowSecurityBiometric</span></span>|<span data-ttu-id="915fa-114">1</span><span class="sxs-lookup"><span data-stu-id="915fa-114">1</span></span>|<span data-ttu-id="915fa-115">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="915fa-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="915fa-116">required</span></span>|<span data-ttu-id="915fa-117">2</span><span class="sxs-lookup"><span data-stu-id="915fa-117">2</span></span>|<span data-ttu-id="915fa-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="915fa-118">Required.</span></span>|
|<span data-ttu-id="915fa-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="915fa-119">atLeastNumeric</span></span>|<span data-ttu-id="915fa-120">3</span><span class="sxs-lookup"><span data-stu-id="915fa-120">3</span></span>|<span data-ttu-id="915fa-121">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-121">At least numeric password required.</span></span>|
|<span data-ttu-id="915fa-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="915fa-122">numericComplex</span></span>|<span data-ttu-id="915fa-123">4</span><span class="sxs-lookup"><span data-stu-id="915fa-123">4</span></span>|<span data-ttu-id="915fa-124">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="915fa-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="915fa-125">atLeastAlphabetic</span></span>|<span data-ttu-id="915fa-126">5</span><span class="sxs-lookup"><span data-stu-id="915fa-126">5</span></span>|<span data-ttu-id="915fa-127">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="915fa-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="915fa-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="915fa-129">6</span><span class="sxs-lookup"><span data-stu-id="915fa-129">6</span></span>|<span data-ttu-id="915fa-130">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="915fa-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="915fa-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="915fa-132">7</span><span class="sxs-lookup"><span data-stu-id="915fa-132">7</span></span>|<span data-ttu-id="915fa-133">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="915fa-133">At least alphanumeric with symbols password required.</span></span>|



