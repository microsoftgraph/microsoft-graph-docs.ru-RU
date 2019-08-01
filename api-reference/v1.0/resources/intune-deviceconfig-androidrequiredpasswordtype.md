---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0562d059ca69358190c49fb6b518abccdc98c449
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028709"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="36924-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="36924-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="36924-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36924-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36924-105">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="36924-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="36924-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="36924-106">Members</span></span>
|<span data-ttu-id="36924-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="36924-107">Member</span></span>|<span data-ttu-id="36924-108">Значение</span><span class="sxs-lookup"><span data-stu-id="36924-108">Value</span></span>|<span data-ttu-id="36924-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36924-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36924-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="36924-110">deviceDefault</span></span>|<span data-ttu-id="36924-111">нуль</span><span class="sxs-lookup"><span data-stu-id="36924-111">0</span></span>|<span data-ttu-id="36924-112">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="36924-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="36924-113">буквы</span><span class="sxs-lookup"><span data-stu-id="36924-113">alphabetic</span></span>|<span data-ttu-id="36924-114">1,1</span><span class="sxs-lookup"><span data-stu-id="36924-114">1</span></span>|<span data-ttu-id="36924-115">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="36924-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="36924-116">цифрового</span><span class="sxs-lookup"><span data-stu-id="36924-116">alphanumeric</span></span>|<span data-ttu-id="36924-117">2</span><span class="sxs-lookup"><span data-stu-id="36924-117">2</span></span>|<span data-ttu-id="36924-118">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="36924-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="36924-119">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="36924-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="36924-120">4</span><span class="sxs-lookup"><span data-stu-id="36924-120">3</span></span>|<span data-ttu-id="36924-121">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="36924-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="36924-122">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="36924-122">lowSecurityBiometric</span></span>|<span data-ttu-id="36924-123">SP4</span><span class="sxs-lookup"><span data-stu-id="36924-123">4</span></span>|<span data-ttu-id="36924-124">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="36924-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="36924-125">числовых</span><span class="sxs-lookup"><span data-stu-id="36924-125">numeric</span></span>|<span data-ttu-id="36924-126">17:00</span><span class="sxs-lookup"><span data-stu-id="36924-126">5</span></span>|<span data-ttu-id="36924-127">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="36924-127">Numeric password required.</span></span>|
|<span data-ttu-id="36924-128">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="36924-128">numericComplex</span></span>|<span data-ttu-id="36924-129">6 </span><span class="sxs-lookup"><span data-stu-id="36924-129">6</span></span>|<span data-ttu-id="36924-130">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="36924-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="36924-131">любой</span><span class="sxs-lookup"><span data-stu-id="36924-131">any</span></span>|<span data-ttu-id="36924-132">7 </span><span class="sxs-lookup"><span data-stu-id="36924-132">7</span></span>|<span data-ttu-id="36924-133">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="36924-133">A password or pattern is required, and any is acceptable.</span></span>|



