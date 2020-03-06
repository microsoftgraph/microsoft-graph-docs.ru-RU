---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24065e97b08b408193f4a3108db5e51fa6f1d28a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530945"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="462c1-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="462c1-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="462c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="462c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="462c1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="462c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="462c1-106">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="462c1-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="462c1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="462c1-107">Members</span></span>
|<span data-ttu-id="462c1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="462c1-108">Member</span></span>|<span data-ttu-id="462c1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="462c1-109">Value</span></span>|<span data-ttu-id="462c1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="462c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="462c1-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="462c1-111">deviceDefault</span></span>|<span data-ttu-id="462c1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="462c1-112">0</span></span>|<span data-ttu-id="462c1-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="462c1-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="462c1-114">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="462c1-114">lowSecurityBiometric</span></span>|<span data-ttu-id="462c1-115">1 </span><span class="sxs-lookup"><span data-stu-id="462c1-115">1</span></span>|<span data-ttu-id="462c1-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="462c1-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="462c1-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="462c1-117">required</span></span>|<span data-ttu-id="462c1-118">2 </span><span class="sxs-lookup"><span data-stu-id="462c1-118">2</span></span>|<span data-ttu-id="462c1-119">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="462c1-119">Required.</span></span>|
|<span data-ttu-id="462c1-120">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="462c1-120">atLeastNumeric</span></span>|<span data-ttu-id="462c1-121">3 </span><span class="sxs-lookup"><span data-stu-id="462c1-121">3</span></span>|<span data-ttu-id="462c1-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="462c1-122">At least numeric password required.</span></span>|
|<span data-ttu-id="462c1-123">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="462c1-123">numericComplex</span></span>|<span data-ttu-id="462c1-124">4 </span><span class="sxs-lookup"><span data-stu-id="462c1-124">4</span></span>|<span data-ttu-id="462c1-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="462c1-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="462c1-126">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="462c1-126">atLeastAlphabetic</span></span>|<span data-ttu-id="462c1-127">5 </span><span class="sxs-lookup"><span data-stu-id="462c1-127">5</span></span>|<span data-ttu-id="462c1-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="462c1-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="462c1-129">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="462c1-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="462c1-130">6 </span><span class="sxs-lookup"><span data-stu-id="462c1-130">6</span></span>|<span data-ttu-id="462c1-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="462c1-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="462c1-132">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="462c1-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="462c1-133">7 </span><span class="sxs-lookup"><span data-stu-id="462c1-133">7</span></span>|<span data-ttu-id="462c1-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="462c1-134">At least alphanumeric with symbols password required.</span></span>|




