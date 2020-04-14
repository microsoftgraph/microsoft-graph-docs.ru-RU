---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b3c2b0945d91bead7f28ec49e53c68f89fbb19d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470224"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="9754b-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="9754b-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="9754b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9754b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9754b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9754b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9754b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9754b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9754b-107">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="9754b-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9754b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9754b-108">Members</span></span>
|<span data-ttu-id="9754b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9754b-109">Member</span></span>|<span data-ttu-id="9754b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9754b-110">Value</span></span>|<span data-ttu-id="9754b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9754b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9754b-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="9754b-112">deviceDefault</span></span>|<span data-ttu-id="9754b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9754b-113">0</span></span>|<span data-ttu-id="9754b-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="9754b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9754b-115">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="9754b-115">lowSecurityBiometric</span></span>|<span data-ttu-id="9754b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="9754b-116">1</span></span>|<span data-ttu-id="9754b-117">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="9754b-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9754b-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9754b-118">required</span></span>|<span data-ttu-id="9754b-119">2</span><span class="sxs-lookup"><span data-stu-id="9754b-119">2</span></span>|<span data-ttu-id="9754b-120">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9754b-120">Required.</span></span>|
|<span data-ttu-id="9754b-121">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="9754b-121">atLeastNumeric</span></span>|<span data-ttu-id="9754b-122">4</span><span class="sxs-lookup"><span data-stu-id="9754b-122">3</span></span>|<span data-ttu-id="9754b-123">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="9754b-123">At least numeric password required.</span></span>|
|<span data-ttu-id="9754b-124">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="9754b-124">numericComplex</span></span>|<span data-ttu-id="9754b-125">4 </span><span class="sxs-lookup"><span data-stu-id="9754b-125">4</span></span>|<span data-ttu-id="9754b-126">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="9754b-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="9754b-127">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="9754b-127">atLeastAlphabetic</span></span>|<span data-ttu-id="9754b-128">5 </span><span class="sxs-lookup"><span data-stu-id="9754b-128">5</span></span>|<span data-ttu-id="9754b-129">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="9754b-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9754b-130">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="9754b-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="9754b-131">6 </span><span class="sxs-lookup"><span data-stu-id="9754b-131">6</span></span>|<span data-ttu-id="9754b-132">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="9754b-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9754b-133">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="9754b-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="9754b-134">7 </span><span class="sxs-lookup"><span data-stu-id="9754b-134">7</span></span>|<span data-ttu-id="9754b-135">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="9754b-135">At least alphanumeric with symbols password required.</span></span>|



