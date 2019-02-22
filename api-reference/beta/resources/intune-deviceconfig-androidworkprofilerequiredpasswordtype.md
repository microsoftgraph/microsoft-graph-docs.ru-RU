---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 742ffaff4c235f9abfeb44d707a3af4429fc86e6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169190"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="cf165-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="cf165-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="cf165-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf165-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf165-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf165-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf165-106">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="cf165-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="cf165-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cf165-107">Members</span></span>
|<span data-ttu-id="cf165-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cf165-108">Member</span></span>|<span data-ttu-id="cf165-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cf165-109">Value</span></span>|<span data-ttu-id="cf165-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cf165-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf165-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="cf165-111">deviceDefault</span></span>|<span data-ttu-id="cf165-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cf165-112">0</span></span>|<span data-ttu-id="cf165-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="cf165-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="cf165-114">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="cf165-114">lowSecurityBiometric</span></span>|<span data-ttu-id="cf165-115">1,1</span><span class="sxs-lookup"><span data-stu-id="cf165-115">1</span></span>|<span data-ttu-id="cf165-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="cf165-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="cf165-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="cf165-117">required</span></span>|<span data-ttu-id="cf165-118">2</span><span class="sxs-lookup"><span data-stu-id="cf165-118">2</span></span>|<span data-ttu-id="cf165-119">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="cf165-119">Required.</span></span>|
|<span data-ttu-id="cf165-120">Атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="cf165-120">atLeastNumeric</span></span>|<span data-ttu-id="cf165-121">4</span><span class="sxs-lookup"><span data-stu-id="cf165-121">3</span></span>|<span data-ttu-id="cf165-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="cf165-122">At least numeric password required.</span></span>|
|<span data-ttu-id="cf165-123">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="cf165-123">numericComplex</span></span>|<span data-ttu-id="cf165-124">4</span><span class="sxs-lookup"><span data-stu-id="cf165-124">4</span></span>|<span data-ttu-id="cf165-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="cf165-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="cf165-126">Атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="cf165-126">atLeastAlphabetic</span></span>|<span data-ttu-id="cf165-127">17:00</span><span class="sxs-lookup"><span data-stu-id="cf165-127">5</span></span>|<span data-ttu-id="cf165-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="cf165-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="cf165-129">Атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="cf165-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="cf165-130">6</span><span class="sxs-lookup"><span data-stu-id="cf165-130">6</span></span>|<span data-ttu-id="cf165-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="cf165-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="cf165-132">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="cf165-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="cf165-133">7</span><span class="sxs-lookup"><span data-stu-id="cf165-133">7</span></span>|<span data-ttu-id="cf165-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="cf165-134">At least alphanumeric with symbols password required.</span></span>|




