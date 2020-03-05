---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7d20aee3893d9d74e01fad6858c59d2c524059d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527302"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f9ecc-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f9ecc-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="f9ecc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f9ecc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9ecc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ecc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ecc-107">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f9ecc-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f9ecc-108">Members</span></span>
|<span data-ttu-id="f9ecc-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f9ecc-109">Member</span></span>|<span data-ttu-id="f9ecc-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f9ecc-110">Value</span></span>|<span data-ttu-id="f9ecc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9ecc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ecc-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="f9ecc-112">deviceDefault</span></span>|<span data-ttu-id="f9ecc-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f9ecc-113">0</span></span>|<span data-ttu-id="f9ecc-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f9ecc-115">буквы</span><span class="sxs-lookup"><span data-stu-id="f9ecc-115">alphabetic</span></span>|<span data-ttu-id="f9ecc-116">1 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-116">1</span></span>|<span data-ttu-id="f9ecc-117">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="f9ecc-118">цифрового</span><span class="sxs-lookup"><span data-stu-id="f9ecc-118">alphanumeric</span></span>|<span data-ttu-id="f9ecc-119">2 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-119">2</span></span>|<span data-ttu-id="f9ecc-120">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f9ecc-121">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="f9ecc-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="f9ecc-122">3 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-122">3</span></span>|<span data-ttu-id="f9ecc-123">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f9ecc-124">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="f9ecc-124">lowSecurityBiometric</span></span>|<span data-ttu-id="f9ecc-125">4 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-125">4</span></span>|<span data-ttu-id="f9ecc-126">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f9ecc-127">числовых</span><span class="sxs-lookup"><span data-stu-id="f9ecc-127">numeric</span></span>|<span data-ttu-id="f9ecc-128">5 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-128">5</span></span>|<span data-ttu-id="f9ecc-129">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-129">Numeric password required.</span></span>|
|<span data-ttu-id="f9ecc-130">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="f9ecc-130">numericComplex</span></span>|<span data-ttu-id="f9ecc-131">6 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-131">6</span></span>|<span data-ttu-id="f9ecc-132">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="f9ecc-133">любой</span><span class="sxs-lookup"><span data-stu-id="f9ecc-133">any</span></span>|<span data-ttu-id="f9ecc-134">7 </span><span class="sxs-lookup"><span data-stu-id="f9ecc-134">7</span></span>|<span data-ttu-id="f9ecc-135">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="f9ecc-135">A password or pattern is required, and any is acceptable.</span></span>|



