---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e20e93543ca681ebd9d900aeaac43731a3d4fa2d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444388"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="b5f06-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b5f06-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="b5f06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5f06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5f06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5f06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5f06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5f06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5f06-107">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="b5f06-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="b5f06-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b5f06-108">Members</span></span>
|<span data-ttu-id="b5f06-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b5f06-109">Member</span></span>|<span data-ttu-id="b5f06-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b5f06-110">Value</span></span>|<span data-ttu-id="b5f06-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5f06-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="b5f06-112">deviceDefault</span></span>|<span data-ttu-id="b5f06-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b5f06-113">0</span></span>|<span data-ttu-id="b5f06-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="b5f06-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="b5f06-115">буквы</span><span class="sxs-lookup"><span data-stu-id="b5f06-115">alphabetic</span></span>|<span data-ttu-id="b5f06-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b5f06-116">1</span></span>|<span data-ttu-id="b5f06-117">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="b5f06-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="b5f06-118">цифрового</span><span class="sxs-lookup"><span data-stu-id="b5f06-118">alphanumeric</span></span>|<span data-ttu-id="b5f06-119">2</span><span class="sxs-lookup"><span data-stu-id="b5f06-119">2</span></span>|<span data-ttu-id="b5f06-120">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="b5f06-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="b5f06-121">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="b5f06-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="b5f06-122">4</span><span class="sxs-lookup"><span data-stu-id="b5f06-122">3</span></span>|<span data-ttu-id="b5f06-123">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="b5f06-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="b5f06-124">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="b5f06-124">lowSecurityBiometric</span></span>|<span data-ttu-id="b5f06-125">4 </span><span class="sxs-lookup"><span data-stu-id="b5f06-125">4</span></span>|<span data-ttu-id="b5f06-126">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="b5f06-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="b5f06-127">числовых</span><span class="sxs-lookup"><span data-stu-id="b5f06-127">numeric</span></span>|<span data-ttu-id="b5f06-128">5 </span><span class="sxs-lookup"><span data-stu-id="b5f06-128">5</span></span>|<span data-ttu-id="b5f06-129">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="b5f06-129">Numeric password required.</span></span>|
|<span data-ttu-id="b5f06-130">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="b5f06-130">numericComplex</span></span>|<span data-ttu-id="b5f06-131">6 </span><span class="sxs-lookup"><span data-stu-id="b5f06-131">6</span></span>|<span data-ttu-id="b5f06-132">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="b5f06-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="b5f06-133">любой</span><span class="sxs-lookup"><span data-stu-id="b5f06-133">any</span></span>|<span data-ttu-id="b5f06-134">7 </span><span class="sxs-lookup"><span data-stu-id="b5f06-134">7</span></span>|<span data-ttu-id="b5f06-135">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="b5f06-135">A password or pattern is required, and any is acceptable.</span></span>|



