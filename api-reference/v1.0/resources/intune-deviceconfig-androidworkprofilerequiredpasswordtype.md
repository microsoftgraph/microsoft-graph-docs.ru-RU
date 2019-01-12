---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbe1eb1482e979d236c1f8bf92f687077fb189f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986280"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="c14a8-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c14a8-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c14a8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c14a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c14a8-105">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-105">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="c14a8-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c14a8-106">Members</span></span>
|<span data-ttu-id="c14a8-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c14a8-107">Member</span></span>|<span data-ttu-id="c14a8-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c14a8-108">Value</span></span>|<span data-ttu-id="c14a8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c14a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c14a8-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c14a8-110">deviceDefault</span></span>|<span data-ttu-id="c14a8-111">0</span><span class="sxs-lookup"><span data-stu-id="c14a8-111">0</span></span>|<span data-ttu-id="c14a8-112">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="c14a8-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="c14a8-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c14a8-113">lowSecurityBiometric</span></span>|<span data-ttu-id="c14a8-114">1</span><span class="sxs-lookup"><span data-stu-id="c14a8-114">1</span></span>|<span data-ttu-id="c14a8-115">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c14a8-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c14a8-116">required</span></span>|<span data-ttu-id="c14a8-117">2</span><span class="sxs-lookup"><span data-stu-id="c14a8-117">2</span></span>|<span data-ttu-id="c14a8-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c14a8-118">Required.</span></span>|
|<span data-ttu-id="c14a8-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="c14a8-119">atLeastNumeric</span></span>|<span data-ttu-id="c14a8-120">3</span><span class="sxs-lookup"><span data-stu-id="c14a8-120">3</span></span>|<span data-ttu-id="c14a8-121">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-121">At least numeric password required.</span></span>|
|<span data-ttu-id="c14a8-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c14a8-122">numericComplex</span></span>|<span data-ttu-id="c14a8-123">4</span><span class="sxs-lookup"><span data-stu-id="c14a8-123">4</span></span>|<span data-ttu-id="c14a8-124">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="c14a8-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="c14a8-125">atLeastAlphabetic</span></span>|<span data-ttu-id="c14a8-126">5</span><span class="sxs-lookup"><span data-stu-id="c14a8-126">5</span></span>|<span data-ttu-id="c14a8-127">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="c14a8-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="c14a8-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="c14a8-129">6</span><span class="sxs-lookup"><span data-stu-id="c14a8-129">6</span></span>|<span data-ttu-id="c14a8-130">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="c14a8-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c14a8-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="c14a8-132">7</span><span class="sxs-lookup"><span data-stu-id="c14a8-132">7</span></span>|<span data-ttu-id="c14a8-133">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="c14a8-133">At least alphanumeric with symbols password required.</span></span>|



