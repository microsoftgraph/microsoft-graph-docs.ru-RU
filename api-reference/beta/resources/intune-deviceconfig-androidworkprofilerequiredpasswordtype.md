---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 822c2021040b0dc4e6eb827e9fec54a40b5cad64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062087"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="b972e-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b972e-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="b972e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b972e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b972e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b972e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b972e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b972e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b972e-107">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="b972e-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="b972e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b972e-108">Members</span></span>
|<span data-ttu-id="b972e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b972e-109">Member</span></span>|<span data-ttu-id="b972e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b972e-110">Value</span></span>|<span data-ttu-id="b972e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b972e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b972e-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="b972e-112">deviceDefault</span></span>|<span data-ttu-id="b972e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b972e-113">0</span></span>|<span data-ttu-id="b972e-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="b972e-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="b972e-115">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="b972e-115">lowSecurityBiometric</span></span>|<span data-ttu-id="b972e-116">1 </span><span class="sxs-lookup"><span data-stu-id="b972e-116">1</span></span>|<span data-ttu-id="b972e-117">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="b972e-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="b972e-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b972e-118">required</span></span>|<span data-ttu-id="b972e-119">2 </span><span class="sxs-lookup"><span data-stu-id="b972e-119">2</span></span>|<span data-ttu-id="b972e-120">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b972e-120">Required.</span></span>|
|<span data-ttu-id="b972e-121">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="b972e-121">atLeastNumeric</span></span>|<span data-ttu-id="b972e-122">4</span><span class="sxs-lookup"><span data-stu-id="b972e-122">3</span></span>|<span data-ttu-id="b972e-123">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="b972e-123">At least numeric password required.</span></span>|
|<span data-ttu-id="b972e-124">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="b972e-124">numericComplex</span></span>|<span data-ttu-id="b972e-125">4 </span><span class="sxs-lookup"><span data-stu-id="b972e-125">4</span></span>|<span data-ttu-id="b972e-126">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="b972e-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="b972e-127">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="b972e-127">atLeastAlphabetic</span></span>|<span data-ttu-id="b972e-128">5 </span><span class="sxs-lookup"><span data-stu-id="b972e-128">5</span></span>|<span data-ttu-id="b972e-129">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="b972e-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="b972e-130">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="b972e-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="b972e-131">6 </span><span class="sxs-lookup"><span data-stu-id="b972e-131">6</span></span>|<span data-ttu-id="b972e-132">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="b972e-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="b972e-133">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="b972e-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="b972e-134">7 </span><span class="sxs-lookup"><span data-stu-id="b972e-134">7</span></span>|<span data-ttu-id="b972e-135">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="b972e-135">At least alphanumeric with symbols password required.</span></span>|






