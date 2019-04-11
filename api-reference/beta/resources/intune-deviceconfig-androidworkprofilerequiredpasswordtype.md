---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bbe0e64fdbbca78766bf7471d29d6cdf17b0714
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802725"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="23a87-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="23a87-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="23a87-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23a87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23a87-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23a87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23a87-106">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="23a87-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="23a87-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="23a87-107">Members</span></span>
|<span data-ttu-id="23a87-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="23a87-108">Member</span></span>|<span data-ttu-id="23a87-109">Значение</span><span class="sxs-lookup"><span data-stu-id="23a87-109">Value</span></span>|<span data-ttu-id="23a87-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23a87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a87-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="23a87-111">deviceDefault</span></span>|<span data-ttu-id="23a87-112">нуль</span><span class="sxs-lookup"><span data-stu-id="23a87-112">0</span></span>|<span data-ttu-id="23a87-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="23a87-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="23a87-114">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="23a87-114">lowSecurityBiometric</span></span>|<span data-ttu-id="23a87-115">1,1</span><span class="sxs-lookup"><span data-stu-id="23a87-115">1</span></span>|<span data-ttu-id="23a87-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="23a87-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="23a87-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="23a87-117">required</span></span>|<span data-ttu-id="23a87-118">2</span><span class="sxs-lookup"><span data-stu-id="23a87-118">2</span></span>|<span data-ttu-id="23a87-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23a87-119">Required.</span></span>|
|<span data-ttu-id="23a87-120">Атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="23a87-120">atLeastNumeric</span></span>|<span data-ttu-id="23a87-121">4</span><span class="sxs-lookup"><span data-stu-id="23a87-121">3</span></span>|<span data-ttu-id="23a87-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="23a87-122">At least numeric password required.</span></span>|
|<span data-ttu-id="23a87-123">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="23a87-123">numericComplex</span></span>|<span data-ttu-id="23a87-124">SP4</span><span class="sxs-lookup"><span data-stu-id="23a87-124">4</span></span>|<span data-ttu-id="23a87-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="23a87-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="23a87-126">Атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="23a87-126">atLeastAlphabetic</span></span>|<span data-ttu-id="23a87-127">17:00</span><span class="sxs-lookup"><span data-stu-id="23a87-127">5</span></span>|<span data-ttu-id="23a87-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="23a87-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="23a87-129">Атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="23a87-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="23a87-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="23a87-130">6</span></span>|<span data-ttu-id="23a87-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="23a87-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="23a87-132">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="23a87-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="23a87-133">см</span><span class="sxs-lookup"><span data-stu-id="23a87-133">7</span></span>|<span data-ttu-id="23a87-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="23a87-134">At least alphanumeric with symbols password required.</span></span>|





