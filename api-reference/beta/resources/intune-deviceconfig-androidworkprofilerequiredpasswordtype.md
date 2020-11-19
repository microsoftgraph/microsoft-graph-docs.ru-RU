---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aa7ab836addd205d0b39c14fa0dcb42dd71bb81a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256962"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="0ccf3-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="0ccf3-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="0ccf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ccf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ccf3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ccf3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ccf3-107">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="0ccf3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0ccf3-108">Members</span></span>
|<span data-ttu-id="0ccf3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0ccf3-109">Member</span></span>|<span data-ttu-id="0ccf3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0ccf3-110">Value</span></span>|<span data-ttu-id="0ccf3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ccf3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ccf3-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="0ccf3-112">deviceDefault</span></span>|<span data-ttu-id="0ccf3-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0ccf3-113">0</span></span>|<span data-ttu-id="0ccf3-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="0ccf3-115">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="0ccf3-115">lowSecurityBiometric</span></span>|<span data-ttu-id="0ccf3-116">1,1</span><span class="sxs-lookup"><span data-stu-id="0ccf3-116">1</span></span>|<span data-ttu-id="0ccf3-117">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0ccf3-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0ccf3-118">required</span></span>|<span data-ttu-id="0ccf3-119">2</span><span class="sxs-lookup"><span data-stu-id="0ccf3-119">2</span></span>|<span data-ttu-id="0ccf3-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-120">Required.</span></span>|
|<span data-ttu-id="0ccf3-121">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="0ccf3-121">atLeastNumeric</span></span>|<span data-ttu-id="0ccf3-122">4</span><span class="sxs-lookup"><span data-stu-id="0ccf3-122">3</span></span>|<span data-ttu-id="0ccf3-123">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-123">At least numeric password required.</span></span>|
|<span data-ttu-id="0ccf3-124">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="0ccf3-124">numericComplex</span></span>|<span data-ttu-id="0ccf3-125">4 </span><span class="sxs-lookup"><span data-stu-id="0ccf3-125">4</span></span>|<span data-ttu-id="0ccf3-126">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="0ccf3-127">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="0ccf3-127">atLeastAlphabetic</span></span>|<span data-ttu-id="0ccf3-128">5 </span><span class="sxs-lookup"><span data-stu-id="0ccf3-128">5</span></span>|<span data-ttu-id="0ccf3-129">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="0ccf3-130">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="0ccf3-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="0ccf3-131">6 </span><span class="sxs-lookup"><span data-stu-id="0ccf3-131">6</span></span>|<span data-ttu-id="0ccf3-132">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="0ccf3-133">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="0ccf3-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="0ccf3-134">7 </span><span class="sxs-lookup"><span data-stu-id="0ccf3-134">7</span></span>|<span data-ttu-id="0ccf3-135">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="0ccf3-135">At least alphanumeric with symbols password required.</span></span>|




