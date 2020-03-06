---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e1ac4e27243adc47b087aa6453ff316d9b2e2fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530964"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="8ab1a-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="8ab1a-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="8ab1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ab1a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab1a-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="8ab1a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8ab1a-107">Members</span></span>
|<span data-ttu-id="8ab1a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8ab1a-108">Member</span></span>|<span data-ttu-id="8ab1a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8ab1a-109">Value</span></span>|<span data-ttu-id="8ab1a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab1a-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="8ab1a-111">deviceDefault</span></span>|<span data-ttu-id="8ab1a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8ab1a-112">0</span></span>|<span data-ttu-id="8ab1a-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="8ab1a-114">буквы</span><span class="sxs-lookup"><span data-stu-id="8ab1a-114">alphabetic</span></span>|<span data-ttu-id="8ab1a-115">1 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-115">1</span></span>|<span data-ttu-id="8ab1a-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="8ab1a-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="8ab1a-117">alphanumeric</span></span>|<span data-ttu-id="8ab1a-118">2 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-118">2</span></span>|<span data-ttu-id="8ab1a-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="8ab1a-120">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="8ab1a-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="8ab1a-121">3 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-121">3</span></span>|<span data-ttu-id="8ab1a-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="8ab1a-123">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="8ab1a-123">lowSecurityBiometric</span></span>|<span data-ttu-id="8ab1a-124">4 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-124">4</span></span>|<span data-ttu-id="8ab1a-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="8ab1a-126">числовых</span><span class="sxs-lookup"><span data-stu-id="8ab1a-126">numeric</span></span>|<span data-ttu-id="8ab1a-127">5 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-127">5</span></span>|<span data-ttu-id="8ab1a-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-128">Numeric password required.</span></span>|
|<span data-ttu-id="8ab1a-129">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="8ab1a-129">numericComplex</span></span>|<span data-ttu-id="8ab1a-130">6 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-130">6</span></span>|<span data-ttu-id="8ab1a-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="8ab1a-132">любой</span><span class="sxs-lookup"><span data-stu-id="8ab1a-132">any</span></span>|<span data-ttu-id="8ab1a-133">7 </span><span class="sxs-lookup"><span data-stu-id="8ab1a-133">7</span></span>|<span data-ttu-id="8ab1a-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="8ab1a-134">A password or pattern is required, and any is acceptable.</span></span>|




