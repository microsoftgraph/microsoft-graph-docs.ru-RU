---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bcdf143e880940bd407d3c1d550b51ee491346c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948501"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="68cd6-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="68cd6-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="68cd6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68cd6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68cd6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68cd6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68cd6-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="68cd6-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="68cd6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="68cd6-107">Members</span></span>
|<span data-ttu-id="68cd6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="68cd6-108">Member</span></span>|<span data-ttu-id="68cd6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="68cd6-109">Value</span></span>|<span data-ttu-id="68cd6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="68cd6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68cd6-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="68cd6-111">deviceDefault</span></span>|<span data-ttu-id="68cd6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="68cd6-112">0</span></span>|<span data-ttu-id="68cd6-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="68cd6-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="68cd6-114">буквы</span><span class="sxs-lookup"><span data-stu-id="68cd6-114">alphabetic</span></span>|<span data-ttu-id="68cd6-115">1,1</span><span class="sxs-lookup"><span data-stu-id="68cd6-115">1</span></span>|<span data-ttu-id="68cd6-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="68cd6-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="68cd6-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="68cd6-117">alphanumeric</span></span>|<span data-ttu-id="68cd6-118">2</span><span class="sxs-lookup"><span data-stu-id="68cd6-118">2</span></span>|<span data-ttu-id="68cd6-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="68cd6-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="68cd6-120">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="68cd6-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="68cd6-121">4</span><span class="sxs-lookup"><span data-stu-id="68cd6-121">3</span></span>|<span data-ttu-id="68cd6-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="68cd6-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="68cd6-123">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="68cd6-123">lowSecurityBiometric</span></span>|<span data-ttu-id="68cd6-124">SP4</span><span class="sxs-lookup"><span data-stu-id="68cd6-124">4</span></span>|<span data-ttu-id="68cd6-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="68cd6-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="68cd6-126">числовых</span><span class="sxs-lookup"><span data-stu-id="68cd6-126">numeric</span></span>|<span data-ttu-id="68cd6-127">17:00</span><span class="sxs-lookup"><span data-stu-id="68cd6-127">5</span></span>|<span data-ttu-id="68cd6-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="68cd6-128">Numeric password required.</span></span>|
|<span data-ttu-id="68cd6-129">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="68cd6-129">numericComplex</span></span>|<span data-ttu-id="68cd6-130">6 </span><span class="sxs-lookup"><span data-stu-id="68cd6-130">6</span></span>|<span data-ttu-id="68cd6-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="68cd6-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="68cd6-132">любой</span><span class="sxs-lookup"><span data-stu-id="68cd6-132">any</span></span>|<span data-ttu-id="68cd6-133">7 </span><span class="sxs-lookup"><span data-stu-id="68cd6-133">7</span></span>|<span data-ttu-id="68cd6-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="68cd6-134">A password or pattern is required, and any is acceptable.</span></span>|




