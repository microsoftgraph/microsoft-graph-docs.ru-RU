---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1845656d43ec2a8f567506ed61b5ee3bc6d8a9ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151522"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f2ac0-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f2ac0-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f2ac0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2ac0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2ac0-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f2ac0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f2ac0-107">Members</span></span>
|<span data-ttu-id="f2ac0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f2ac0-108">Member</span></span>|<span data-ttu-id="f2ac0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f2ac0-109">Value</span></span>|<span data-ttu-id="f2ac0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f2ac0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2ac0-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="f2ac0-111">deviceDefault</span></span>|<span data-ttu-id="f2ac0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f2ac0-112">0</span></span>|<span data-ttu-id="f2ac0-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f2ac0-114">буквы</span><span class="sxs-lookup"><span data-stu-id="f2ac0-114">alphabetic</span></span>|<span data-ttu-id="f2ac0-115">1,1</span><span class="sxs-lookup"><span data-stu-id="f2ac0-115">1</span></span>|<span data-ttu-id="f2ac0-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="f2ac0-117">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="f2ac0-117">alphanumeric</span></span>|<span data-ttu-id="f2ac0-118">2</span><span class="sxs-lookup"><span data-stu-id="f2ac0-118">2</span></span>|<span data-ttu-id="f2ac0-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f2ac0-120">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="f2ac0-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="f2ac0-121">4</span><span class="sxs-lookup"><span data-stu-id="f2ac0-121">3</span></span>|<span data-ttu-id="f2ac0-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f2ac0-123">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="f2ac0-123">lowSecurityBiometric</span></span>|<span data-ttu-id="f2ac0-124">4</span><span class="sxs-lookup"><span data-stu-id="f2ac0-124">4</span></span>|<span data-ttu-id="f2ac0-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f2ac0-126">числовых</span><span class="sxs-lookup"><span data-stu-id="f2ac0-126">numeric</span></span>|<span data-ttu-id="f2ac0-127">17:00</span><span class="sxs-lookup"><span data-stu-id="f2ac0-127">5</span></span>|<span data-ttu-id="f2ac0-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-128">Numeric password required.</span></span>|
|<span data-ttu-id="f2ac0-129">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="f2ac0-129">numericComplex</span></span>|<span data-ttu-id="f2ac0-130">6</span><span class="sxs-lookup"><span data-stu-id="f2ac0-130">6</span></span>|<span data-ttu-id="f2ac0-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="f2ac0-132">любой</span><span class="sxs-lookup"><span data-stu-id="f2ac0-132">any</span></span>|<span data-ttu-id="f2ac0-133">7</span><span class="sxs-lookup"><span data-stu-id="f2ac0-133">7</span></span>|<span data-ttu-id="f2ac0-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="f2ac0-134">A password or pattern is required, and any is acceptable.</span></span>|




