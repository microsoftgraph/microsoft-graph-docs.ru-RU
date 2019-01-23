---
title: Тип перечисления androidWorkProfileRequiredPasswordType
description: Android профиля рабочего требуется тип пароль.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cdf8c03dab6642cf6859ca822001a71b041c0e54
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399901"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="ab329-103">Тип перечисления androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ab329-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="ab329-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab329-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab329-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab329-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab329-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab329-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab329-107">Android профиля рабочего требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="ab329-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ab329-108">Members</span></span>
|<span data-ttu-id="ab329-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ab329-109">Member</span></span>|<span data-ttu-id="ab329-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ab329-110">Value</span></span>|<span data-ttu-id="ab329-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab329-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab329-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ab329-112">deviceDefault</span></span>|<span data-ttu-id="ab329-113">0</span><span class="sxs-lookup"><span data-stu-id="ab329-113">0</span></span>|<span data-ttu-id="ab329-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="ab329-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="ab329-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="ab329-115">lowSecurityBiometric</span></span>|<span data-ttu-id="ab329-116">1</span><span class="sxs-lookup"><span data-stu-id="ab329-116">1</span></span>|<span data-ttu-id="ab329-117">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="ab329-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="ab329-118">required</span></span>|<span data-ttu-id="ab329-119">2</span><span class="sxs-lookup"><span data-stu-id="ab329-119">2</span></span>|<span data-ttu-id="ab329-120">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="ab329-120">Required.</span></span>|
|<span data-ttu-id="ab329-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="ab329-121">atLeastNumeric</span></span>|<span data-ttu-id="ab329-122">3</span><span class="sxs-lookup"><span data-stu-id="ab329-122">3</span></span>|<span data-ttu-id="ab329-123">Требуется по крайней мере цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-123">At least numeric password required.</span></span>|
|<span data-ttu-id="ab329-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="ab329-124">numericComplex</span></span>|<span data-ttu-id="ab329-125">4</span><span class="sxs-lookup"><span data-stu-id="ab329-125">4</span></span>|<span data-ttu-id="ab329-126">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="ab329-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="ab329-127">atLeastAlphabetic</span></span>|<span data-ttu-id="ab329-128">5</span><span class="sxs-lookup"><span data-stu-id="ab329-128">5</span></span>|<span data-ttu-id="ab329-129">Требуется по крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="ab329-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="ab329-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="ab329-131">6</span><span class="sxs-lookup"><span data-stu-id="ab329-131">6</span></span>|<span data-ttu-id="ab329-132">Требуется по крайней мере буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="ab329-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="ab329-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="ab329-134">7</span><span class="sxs-lookup"><span data-stu-id="ab329-134">7</span></span>|<span data-ttu-id="ab329-135">По крайней мере буквенно-цифровых с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="ab329-135">At least alphanumeric with symbols password required.</span></span>|




