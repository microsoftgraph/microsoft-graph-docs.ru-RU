---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1baa25eeac9745b41a9b2fc356ff98f3991ad8f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449354"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="c5a45-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c5a45-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="c5a45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5a45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5a45-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5a45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a45-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="c5a45-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c5a45-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5a45-107">Members</span></span>
|<span data-ttu-id="c5a45-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5a45-108">Member</span></span>|<span data-ttu-id="c5a45-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c5a45-109">Value</span></span>|<span data-ttu-id="c5a45-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a45-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a45-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="c5a45-111">deviceDefault</span></span>|<span data-ttu-id="c5a45-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c5a45-112">0</span></span>|<span data-ttu-id="c5a45-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="c5a45-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="c5a45-114">буквы</span><span class="sxs-lookup"><span data-stu-id="c5a45-114">alphabetic</span></span>|<span data-ttu-id="c5a45-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c5a45-115">1</span></span>|<span data-ttu-id="c5a45-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="c5a45-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="c5a45-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="c5a45-117">alphanumeric</span></span>|<span data-ttu-id="c5a45-118">2</span><span class="sxs-lookup"><span data-stu-id="c5a45-118">2</span></span>|<span data-ttu-id="c5a45-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="c5a45-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="c5a45-120">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="c5a45-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="c5a45-121">4</span><span class="sxs-lookup"><span data-stu-id="c5a45-121">3</span></span>|<span data-ttu-id="c5a45-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="c5a45-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="c5a45-123">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="c5a45-123">lowSecurityBiometric</span></span>|<span data-ttu-id="c5a45-124">4 </span><span class="sxs-lookup"><span data-stu-id="c5a45-124">4</span></span>|<span data-ttu-id="c5a45-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="c5a45-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c5a45-126">числовых</span><span class="sxs-lookup"><span data-stu-id="c5a45-126">numeric</span></span>|<span data-ttu-id="c5a45-127">5 </span><span class="sxs-lookup"><span data-stu-id="c5a45-127">5</span></span>|<span data-ttu-id="c5a45-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="c5a45-128">Numeric password required.</span></span>|
|<span data-ttu-id="c5a45-129">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="c5a45-129">numericComplex</span></span>|<span data-ttu-id="c5a45-130">6 </span><span class="sxs-lookup"><span data-stu-id="c5a45-130">6</span></span>|<span data-ttu-id="c5a45-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="c5a45-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="c5a45-132">любой</span><span class="sxs-lookup"><span data-stu-id="c5a45-132">any</span></span>|<span data-ttu-id="c5a45-133">7 </span><span class="sxs-lookup"><span data-stu-id="c5a45-133">7</span></span>|<span data-ttu-id="c5a45-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="c5a45-134">A password or pattern is required, and any is acceptable.</span></span>|







