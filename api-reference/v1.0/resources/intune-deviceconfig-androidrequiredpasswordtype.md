---
title: Тип перечисления androidRequiredPasswordType
description: Тип Android пароль.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 06a89256920f143af923e6a3949e61843fa7aa00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814422"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="19edb-103">Тип перечисления androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="19edb-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="19edb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19edb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19edb-105">Тип Android пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="19edb-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="19edb-106">Members</span></span>
|<span data-ttu-id="19edb-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="19edb-107">Member</span></span>|<span data-ttu-id="19edb-108">Значение</span><span class="sxs-lookup"><span data-stu-id="19edb-108">Value</span></span>|<span data-ttu-id="19edb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="19edb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19edb-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="19edb-110">deviceDefault</span></span>|<span data-ttu-id="19edb-111">0</span><span class="sxs-lookup"><span data-stu-id="19edb-111">0</span></span>|<span data-ttu-id="19edb-112">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="19edb-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="19edb-113">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="19edb-113">alphabetic</span></span>|<span data-ttu-id="19edb-114">1</span><span class="sxs-lookup"><span data-stu-id="19edb-114">1</span></span>|<span data-ttu-id="19edb-115">К буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="19edb-116">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="19edb-116">alphanumeric</span></span>|<span data-ttu-id="19edb-117">2</span><span class="sxs-lookup"><span data-stu-id="19edb-117">2</span></span>|<span data-ttu-id="19edb-118">Буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="19edb-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="19edb-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="19edb-120">3</span><span class="sxs-lookup"><span data-stu-id="19edb-120">3</span></span>|<span data-ttu-id="19edb-121">Буквы или цифры с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="19edb-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="19edb-122">lowSecurityBiometric</span></span>|<span data-ttu-id="19edb-123">4</span><span class="sxs-lookup"><span data-stu-id="19edb-123">4</span></span>|<span data-ttu-id="19edb-124">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="19edb-125">числовое</span><span class="sxs-lookup"><span data-stu-id="19edb-125">numeric</span></span>|<span data-ttu-id="19edb-126">5</span><span class="sxs-lookup"><span data-stu-id="19edb-126">5</span></span>|<span data-ttu-id="19edb-127">Числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-127">Numeric password required.</span></span>|
|<span data-ttu-id="19edb-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="19edb-128">numericComplex</span></span>|<span data-ttu-id="19edb-129">6</span><span class="sxs-lookup"><span data-stu-id="19edb-129">6</span></span>|<span data-ttu-id="19edb-130">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="19edb-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="19edb-131">любой</span><span class="sxs-lookup"><span data-stu-id="19edb-131">any</span></span>|<span data-ttu-id="19edb-132">7</span><span class="sxs-lookup"><span data-stu-id="19edb-132">7</span></span>|<span data-ttu-id="19edb-133">Пароль или шаблон является обязательным, а какие-либо допустима.</span><span class="sxs-lookup"><span data-stu-id="19edb-133">A password or pattern is required, and any is acceptable.</span></span>|



