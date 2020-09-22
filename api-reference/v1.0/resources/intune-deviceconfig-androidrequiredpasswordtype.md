---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4921263e1960617b8d9e013ce12a799e11d61516
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041563"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="84957-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="84957-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="84957-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84957-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84957-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84957-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84957-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="84957-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="84957-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="84957-107">Members</span></span>
|<span data-ttu-id="84957-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="84957-108">Member</span></span>|<span data-ttu-id="84957-109">Значение</span><span class="sxs-lookup"><span data-stu-id="84957-109">Value</span></span>|<span data-ttu-id="84957-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84957-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84957-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="84957-111">deviceDefault</span></span>|<span data-ttu-id="84957-112">нуль</span><span class="sxs-lookup"><span data-stu-id="84957-112">0</span></span>|<span data-ttu-id="84957-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="84957-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="84957-114">буквы</span><span class="sxs-lookup"><span data-stu-id="84957-114">alphabetic</span></span>|<span data-ttu-id="84957-115">1 </span><span class="sxs-lookup"><span data-stu-id="84957-115">1</span></span>|<span data-ttu-id="84957-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="84957-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="84957-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="84957-117">alphanumeric</span></span>|<span data-ttu-id="84957-118">2 </span><span class="sxs-lookup"><span data-stu-id="84957-118">2</span></span>|<span data-ttu-id="84957-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="84957-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="84957-120">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="84957-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="84957-121">4</span><span class="sxs-lookup"><span data-stu-id="84957-121">3</span></span>|<span data-ttu-id="84957-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="84957-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="84957-123">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="84957-123">lowSecurityBiometric</span></span>|<span data-ttu-id="84957-124">4 </span><span class="sxs-lookup"><span data-stu-id="84957-124">4</span></span>|<span data-ttu-id="84957-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="84957-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="84957-126">числовых</span><span class="sxs-lookup"><span data-stu-id="84957-126">numeric</span></span>|<span data-ttu-id="84957-127">5 </span><span class="sxs-lookup"><span data-stu-id="84957-127">5</span></span>|<span data-ttu-id="84957-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="84957-128">Numeric password required.</span></span>|
|<span data-ttu-id="84957-129">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="84957-129">numericComplex</span></span>|<span data-ttu-id="84957-130">6 </span><span class="sxs-lookup"><span data-stu-id="84957-130">6</span></span>|<span data-ttu-id="84957-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="84957-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="84957-132">любой</span><span class="sxs-lookup"><span data-stu-id="84957-132">any</span></span>|<span data-ttu-id="84957-133">7 </span><span class="sxs-lookup"><span data-stu-id="84957-133">7</span></span>|<span data-ttu-id="84957-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="84957-134">A password or pattern is required, and any is acceptable.</span></span>|









