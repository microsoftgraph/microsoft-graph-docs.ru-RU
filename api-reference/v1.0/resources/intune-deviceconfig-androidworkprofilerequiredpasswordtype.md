---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2e9c65138a6dee7082b85261fd62c0fe9a9fd5e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028681"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="ccade-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="ccade-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="ccade-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccade-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccade-105">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="ccade-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="ccade-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ccade-106">Members</span></span>
|<span data-ttu-id="ccade-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ccade-107">Member</span></span>|<span data-ttu-id="ccade-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ccade-108">Value</span></span>|<span data-ttu-id="ccade-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ccade-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccade-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="ccade-110">deviceDefault</span></span>|<span data-ttu-id="ccade-111">нуль</span><span class="sxs-lookup"><span data-stu-id="ccade-111">0</span></span>|<span data-ttu-id="ccade-112">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="ccade-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="ccade-113">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="ccade-113">lowSecurityBiometric</span></span>|<span data-ttu-id="ccade-114">1,1</span><span class="sxs-lookup"><span data-stu-id="ccade-114">1</span></span>|<span data-ttu-id="ccade-115">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="ccade-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="ccade-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="ccade-116">required</span></span>|<span data-ttu-id="ccade-117">2</span><span class="sxs-lookup"><span data-stu-id="ccade-117">2</span></span>|<span data-ttu-id="ccade-118">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ccade-118">Required.</span></span>|
|<span data-ttu-id="ccade-119">Атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="ccade-119">atLeastNumeric</span></span>|<span data-ttu-id="ccade-120">4</span><span class="sxs-lookup"><span data-stu-id="ccade-120">3</span></span>|<span data-ttu-id="ccade-121">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="ccade-121">At least numeric password required.</span></span>|
|<span data-ttu-id="ccade-122">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="ccade-122">numericComplex</span></span>|<span data-ttu-id="ccade-123">SP4</span><span class="sxs-lookup"><span data-stu-id="ccade-123">4</span></span>|<span data-ttu-id="ccade-124">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="ccade-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="ccade-125">Атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="ccade-125">atLeastAlphabetic</span></span>|<span data-ttu-id="ccade-126">17:00</span><span class="sxs-lookup"><span data-stu-id="ccade-126">5</span></span>|<span data-ttu-id="ccade-127">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="ccade-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="ccade-128">Атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="ccade-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="ccade-129">6 </span><span class="sxs-lookup"><span data-stu-id="ccade-129">6</span></span>|<span data-ttu-id="ccade-130">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="ccade-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="ccade-131">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="ccade-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="ccade-132">7 </span><span class="sxs-lookup"><span data-stu-id="ccade-132">7</span></span>|<span data-ttu-id="ccade-133">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="ccade-133">At least alphanumeric with symbols password required.</span></span>|



