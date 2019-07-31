---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5553329c8519aa40eb4f1ee3ee3cb48f66c06995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011640"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="a0a48-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="a0a48-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a0a48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0a48-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0a48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a48-106">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="a0a48-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a0a48-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a0a48-107">Members</span></span>
|<span data-ttu-id="a0a48-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a0a48-108">Member</span></span>|<span data-ttu-id="a0a48-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a0a48-109">Value</span></span>|<span data-ttu-id="a0a48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a48-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="a0a48-111">deviceDefault</span></span>|<span data-ttu-id="a0a48-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a0a48-112">0</span></span>|<span data-ttu-id="a0a48-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="a0a48-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a0a48-114">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="a0a48-114">lowSecurityBiometric</span></span>|<span data-ttu-id="a0a48-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a0a48-115">1</span></span>|<span data-ttu-id="a0a48-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="a0a48-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a0a48-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a0a48-117">required</span></span>|<span data-ttu-id="a0a48-118">2</span><span class="sxs-lookup"><span data-stu-id="a0a48-118">2</span></span>|<span data-ttu-id="a0a48-119">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a0a48-119">Required.</span></span>|
|<span data-ttu-id="a0a48-120">Атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="a0a48-120">atLeastNumeric</span></span>|<span data-ttu-id="a0a48-121">4</span><span class="sxs-lookup"><span data-stu-id="a0a48-121">3</span></span>|<span data-ttu-id="a0a48-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="a0a48-122">At least numeric password required.</span></span>|
|<span data-ttu-id="a0a48-123">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="a0a48-123">numericComplex</span></span>|<span data-ttu-id="a0a48-124">SP4</span><span class="sxs-lookup"><span data-stu-id="a0a48-124">4</span></span>|<span data-ttu-id="a0a48-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="a0a48-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="a0a48-126">Атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="a0a48-126">atLeastAlphabetic</span></span>|<span data-ttu-id="a0a48-127">17:00</span><span class="sxs-lookup"><span data-stu-id="a0a48-127">5</span></span>|<span data-ttu-id="a0a48-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="a0a48-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="a0a48-129">Атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="a0a48-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="a0a48-130">6 </span><span class="sxs-lookup"><span data-stu-id="a0a48-130">6</span></span>|<span data-ttu-id="a0a48-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="a0a48-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="a0a48-132">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="a0a48-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="a0a48-133">7 </span><span class="sxs-lookup"><span data-stu-id="a0a48-133">7</span></span>|<span data-ttu-id="a0a48-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="a0a48-134">At least alphanumeric with symbols password required.</span></span>|





