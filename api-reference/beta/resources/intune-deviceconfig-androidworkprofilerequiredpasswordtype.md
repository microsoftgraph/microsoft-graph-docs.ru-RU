---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 28b02f37bad557f71901c15d03ba963143cb05f3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796133"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="38727-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="38727-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="38727-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38727-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38727-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38727-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38727-106">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="38727-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="38727-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="38727-107">Members</span></span>
|<span data-ttu-id="38727-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="38727-108">Member</span></span>|<span data-ttu-id="38727-109">Значение</span><span class="sxs-lookup"><span data-stu-id="38727-109">Value</span></span>|<span data-ttu-id="38727-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38727-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38727-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="38727-111">deviceDefault</span></span>|<span data-ttu-id="38727-112">нуль</span><span class="sxs-lookup"><span data-stu-id="38727-112">0</span></span>|<span data-ttu-id="38727-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="38727-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="38727-114">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="38727-114">lowSecurityBiometric</span></span>|<span data-ttu-id="38727-115">1,1</span><span class="sxs-lookup"><span data-stu-id="38727-115">1</span></span>|<span data-ttu-id="38727-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="38727-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="38727-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="38727-117">required</span></span>|<span data-ttu-id="38727-118">2</span><span class="sxs-lookup"><span data-stu-id="38727-118">2</span></span>|<span data-ttu-id="38727-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38727-119">Required.</span></span>|
|<span data-ttu-id="38727-120">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="38727-120">atLeastNumeric</span></span>|<span data-ttu-id="38727-121">4</span><span class="sxs-lookup"><span data-stu-id="38727-121">3</span></span>|<span data-ttu-id="38727-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="38727-122">At least numeric password required.</span></span>|
|<span data-ttu-id="38727-123">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="38727-123">numericComplex</span></span>|<span data-ttu-id="38727-124">4 </span><span class="sxs-lookup"><span data-stu-id="38727-124">4</span></span>|<span data-ttu-id="38727-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="38727-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="38727-126">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="38727-126">atLeastAlphabetic</span></span>|<span data-ttu-id="38727-127">5 </span><span class="sxs-lookup"><span data-stu-id="38727-127">5</span></span>|<span data-ttu-id="38727-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="38727-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="38727-129">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="38727-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="38727-130">6 </span><span class="sxs-lookup"><span data-stu-id="38727-130">6</span></span>|<span data-ttu-id="38727-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="38727-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="38727-132">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="38727-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="38727-133">7 </span><span class="sxs-lookup"><span data-stu-id="38727-133">7</span></span>|<span data-ttu-id="38727-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="38727-134">At least alphanumeric with symbols password required.</span></span>|



