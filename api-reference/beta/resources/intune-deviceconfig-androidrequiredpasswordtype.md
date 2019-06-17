---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2cfbf31bc2c263031e2e850e4caf479abb325ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988953"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="0af1d-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="0af1d-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="0af1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0af1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0af1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0af1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0af1d-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="0af1d-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="0af1d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0af1d-107">Members</span></span>
|<span data-ttu-id="0af1d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0af1d-108">Member</span></span>|<span data-ttu-id="0af1d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0af1d-109">Value</span></span>|<span data-ttu-id="0af1d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0af1d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af1d-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="0af1d-111">deviceDefault</span></span>|<span data-ttu-id="0af1d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0af1d-112">0</span></span>|<span data-ttu-id="0af1d-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="0af1d-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="0af1d-114">буквы</span><span class="sxs-lookup"><span data-stu-id="0af1d-114">alphabetic</span></span>|<span data-ttu-id="0af1d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0af1d-115">1</span></span>|<span data-ttu-id="0af1d-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="0af1d-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="0af1d-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="0af1d-117">alphanumeric</span></span>|<span data-ttu-id="0af1d-118">2</span><span class="sxs-lookup"><span data-stu-id="0af1d-118">2</span></span>|<span data-ttu-id="0af1d-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="0af1d-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="0af1d-120">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="0af1d-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="0af1d-121">4</span><span class="sxs-lookup"><span data-stu-id="0af1d-121">3</span></span>|<span data-ttu-id="0af1d-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="0af1d-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="0af1d-123">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="0af1d-123">lowSecurityBiometric</span></span>|<span data-ttu-id="0af1d-124">SP4</span><span class="sxs-lookup"><span data-stu-id="0af1d-124">4</span></span>|<span data-ttu-id="0af1d-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="0af1d-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0af1d-126">числовых</span><span class="sxs-lookup"><span data-stu-id="0af1d-126">numeric</span></span>|<span data-ttu-id="0af1d-127">17:00</span><span class="sxs-lookup"><span data-stu-id="0af1d-127">5</span></span>|<span data-ttu-id="0af1d-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="0af1d-128">Numeric password required.</span></span>|
|<span data-ttu-id="0af1d-129">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="0af1d-129">numericComplex</span></span>|<span data-ttu-id="0af1d-130">6 </span><span class="sxs-lookup"><span data-stu-id="0af1d-130">6</span></span>|<span data-ttu-id="0af1d-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="0af1d-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="0af1d-132">любой</span><span class="sxs-lookup"><span data-stu-id="0af1d-132">any</span></span>|<span data-ttu-id="0af1d-133">7 </span><span class="sxs-lookup"><span data-stu-id="0af1d-133">7</span></span>|<span data-ttu-id="0af1d-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="0af1d-134">A password or pattern is required, and any is acceptable.</span></span>|





