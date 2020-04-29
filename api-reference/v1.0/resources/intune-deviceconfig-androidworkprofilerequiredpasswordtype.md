---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e84439dbd7125d02a5413b46bca1e4e79e13089c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449248"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="9167d-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="9167d-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="9167d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9167d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9167d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9167d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9167d-106">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="9167d-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9167d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9167d-107">Members</span></span>
|<span data-ttu-id="9167d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9167d-108">Member</span></span>|<span data-ttu-id="9167d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9167d-109">Value</span></span>|<span data-ttu-id="9167d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9167d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9167d-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="9167d-111">deviceDefault</span></span>|<span data-ttu-id="9167d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9167d-112">0</span></span>|<span data-ttu-id="9167d-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="9167d-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="9167d-114">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="9167d-114">lowSecurityBiometric</span></span>|<span data-ttu-id="9167d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9167d-115">1</span></span>|<span data-ttu-id="9167d-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="9167d-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9167d-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9167d-117">required</span></span>|<span data-ttu-id="9167d-118">2</span><span class="sxs-lookup"><span data-stu-id="9167d-118">2</span></span>|<span data-ttu-id="9167d-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9167d-119">Required.</span></span>|
|<span data-ttu-id="9167d-120">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="9167d-120">atLeastNumeric</span></span>|<span data-ttu-id="9167d-121">4</span><span class="sxs-lookup"><span data-stu-id="9167d-121">3</span></span>|<span data-ttu-id="9167d-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="9167d-122">At least numeric password required.</span></span>|
|<span data-ttu-id="9167d-123">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="9167d-123">numericComplex</span></span>|<span data-ttu-id="9167d-124">4 </span><span class="sxs-lookup"><span data-stu-id="9167d-124">4</span></span>|<span data-ttu-id="9167d-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="9167d-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="9167d-126">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="9167d-126">atLeastAlphabetic</span></span>|<span data-ttu-id="9167d-127">5 </span><span class="sxs-lookup"><span data-stu-id="9167d-127">5</span></span>|<span data-ttu-id="9167d-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="9167d-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9167d-129">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="9167d-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="9167d-130">6 </span><span class="sxs-lookup"><span data-stu-id="9167d-130">6</span></span>|<span data-ttu-id="9167d-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="9167d-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9167d-132">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="9167d-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="9167d-133">7 </span><span class="sxs-lookup"><span data-stu-id="9167d-133">7</span></span>|<span data-ttu-id="9167d-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="9167d-134">At least alphanumeric with symbols password required.</span></span>|







