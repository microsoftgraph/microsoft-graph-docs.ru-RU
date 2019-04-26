---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575172"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="12a79-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="12a79-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="12a79-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12a79-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a79-105">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="12a79-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="12a79-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="12a79-106">Members</span></span>
|<span data-ttu-id="12a79-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="12a79-107">Member</span></span>|<span data-ttu-id="12a79-108">Значение</span><span class="sxs-lookup"><span data-stu-id="12a79-108">Value</span></span>|<span data-ttu-id="12a79-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12a79-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a79-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="12a79-110">deviceDefault</span></span>|<span data-ttu-id="12a79-111">нуль</span><span class="sxs-lookup"><span data-stu-id="12a79-111">0</span></span>|<span data-ttu-id="12a79-112">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="12a79-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="12a79-113">буквы</span><span class="sxs-lookup"><span data-stu-id="12a79-113">alphabetic</span></span>|<span data-ttu-id="12a79-114">1 </span><span class="sxs-lookup"><span data-stu-id="12a79-114">1</span></span>|<span data-ttu-id="12a79-115">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="12a79-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="12a79-116">цифрового</span><span class="sxs-lookup"><span data-stu-id="12a79-116">alphanumeric</span></span>|<span data-ttu-id="12a79-117">2 </span><span class="sxs-lookup"><span data-stu-id="12a79-117">2</span></span>|<span data-ttu-id="12a79-118">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="12a79-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="12a79-119">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="12a79-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="12a79-120">3 </span><span class="sxs-lookup"><span data-stu-id="12a79-120">3</span></span>|<span data-ttu-id="12a79-121">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="12a79-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="12a79-122">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="12a79-122">lowSecurityBiometric</span></span>|<span data-ttu-id="12a79-123">4 </span><span class="sxs-lookup"><span data-stu-id="12a79-123">4</span></span>|<span data-ttu-id="12a79-124">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="12a79-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="12a79-125">числовых</span><span class="sxs-lookup"><span data-stu-id="12a79-125">numeric</span></span>|<span data-ttu-id="12a79-126">5 </span><span class="sxs-lookup"><span data-stu-id="12a79-126">5</span></span>|<span data-ttu-id="12a79-127">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="12a79-127">Numeric password required.</span></span>|
|<span data-ttu-id="12a79-128">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="12a79-128">numericComplex</span></span>|<span data-ttu-id="12a79-129">6 </span><span class="sxs-lookup"><span data-stu-id="12a79-129">6</span></span>|<span data-ttu-id="12a79-130">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="12a79-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="12a79-131">любой</span><span class="sxs-lookup"><span data-stu-id="12a79-131">any</span></span>|<span data-ttu-id="12a79-132">7 </span><span class="sxs-lookup"><span data-stu-id="12a79-132">7</span></span>|<span data-ttu-id="12a79-133">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="12a79-133">A password or pattern is required, and any is acceptable.</span></span>|



