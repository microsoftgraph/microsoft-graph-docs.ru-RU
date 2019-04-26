---
title: тип перечисления Андроидворкпрофилерекуиредпассвордтипе
description: Необходимый тип пароля для рабочего профиля Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1dbb0b7e523ea6ca3ac1be3328cf58e30d9a892
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575158"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="afa02-103">тип перечисления Андроидворкпрофилерекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="afa02-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="afa02-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="afa02-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afa02-105">Необходимый тип пароля для рабочего профиля Android.</span><span class="sxs-lookup"><span data-stu-id="afa02-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="afa02-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="afa02-106">Members</span></span>
|<span data-ttu-id="afa02-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="afa02-107">Member</span></span>|<span data-ttu-id="afa02-108">Значение</span><span class="sxs-lookup"><span data-stu-id="afa02-108">Value</span></span>|<span data-ttu-id="afa02-109">Описание</span><span class="sxs-lookup"><span data-stu-id="afa02-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afa02-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="afa02-110">deviceDefault</span></span>|<span data-ttu-id="afa02-111">нуль</span><span class="sxs-lookup"><span data-stu-id="afa02-111">0</span></span>|<span data-ttu-id="afa02-112">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="afa02-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="afa02-113">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="afa02-113">lowSecurityBiometric</span></span>|<span data-ttu-id="afa02-114">1 </span><span class="sxs-lookup"><span data-stu-id="afa02-114">1</span></span>|<span data-ttu-id="afa02-115">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="afa02-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="afa02-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="afa02-116">required</span></span>|<span data-ttu-id="afa02-117">2 </span><span class="sxs-lookup"><span data-stu-id="afa02-117">2</span></span>|<span data-ttu-id="afa02-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afa02-118">Required.</span></span>|
|<span data-ttu-id="afa02-119">Атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="afa02-119">atLeastNumeric</span></span>|<span data-ttu-id="afa02-120">3 </span><span class="sxs-lookup"><span data-stu-id="afa02-120">3</span></span>|<span data-ttu-id="afa02-121">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="afa02-121">At least numeric password required.</span></span>|
|<span data-ttu-id="afa02-122">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="afa02-122">numericComplex</span></span>|<span data-ttu-id="afa02-123">4 </span><span class="sxs-lookup"><span data-stu-id="afa02-123">4</span></span>|<span data-ttu-id="afa02-124">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="afa02-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="afa02-125">Атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="afa02-125">atLeastAlphabetic</span></span>|<span data-ttu-id="afa02-126">5 </span><span class="sxs-lookup"><span data-stu-id="afa02-126">5</span></span>|<span data-ttu-id="afa02-127">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="afa02-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="afa02-128">Атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="afa02-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="afa02-129">6 </span><span class="sxs-lookup"><span data-stu-id="afa02-129">6</span></span>|<span data-ttu-id="afa02-130">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="afa02-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="afa02-131">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="afa02-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="afa02-132">7 </span><span class="sxs-lookup"><span data-stu-id="afa02-132">7</span></span>|<span data-ttu-id="afa02-133">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="afa02-133">At least alphanumeric with symbols password required.</span></span>|



