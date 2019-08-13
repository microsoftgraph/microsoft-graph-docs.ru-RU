---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9112074842e3dc661786acfa6c6c223aa5fe225b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334376"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="36660-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="36660-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="36660-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36660-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36660-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36660-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36660-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="36660-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="36660-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="36660-107">Members</span></span>
|<span data-ttu-id="36660-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="36660-108">Member</span></span>|<span data-ttu-id="36660-109">Значение</span><span class="sxs-lookup"><span data-stu-id="36660-109">Value</span></span>|<span data-ttu-id="36660-110">Описание</span><span class="sxs-lookup"><span data-stu-id="36660-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36660-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="36660-111">deviceDefault</span></span>|<span data-ttu-id="36660-112">нуль</span><span class="sxs-lookup"><span data-stu-id="36660-112">0</span></span>|<span data-ttu-id="36660-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="36660-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="36660-114">буквы</span><span class="sxs-lookup"><span data-stu-id="36660-114">alphabetic</span></span>|<span data-ttu-id="36660-115">1,1</span><span class="sxs-lookup"><span data-stu-id="36660-115">1</span></span>|<span data-ttu-id="36660-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="36660-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="36660-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="36660-117">alphanumeric</span></span>|<span data-ttu-id="36660-118">2</span><span class="sxs-lookup"><span data-stu-id="36660-118">2</span></span>|<span data-ttu-id="36660-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="36660-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="36660-120">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="36660-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="36660-121">4</span><span class="sxs-lookup"><span data-stu-id="36660-121">3</span></span>|<span data-ttu-id="36660-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="36660-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="36660-123">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="36660-123">lowSecurityBiometric</span></span>|<span data-ttu-id="36660-124">SP4</span><span class="sxs-lookup"><span data-stu-id="36660-124">4</span></span>|<span data-ttu-id="36660-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="36660-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="36660-126">числовых</span><span class="sxs-lookup"><span data-stu-id="36660-126">numeric</span></span>|<span data-ttu-id="36660-127">17:00</span><span class="sxs-lookup"><span data-stu-id="36660-127">5</span></span>|<span data-ttu-id="36660-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="36660-128">Numeric password required.</span></span>|
|<span data-ttu-id="36660-129">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="36660-129">numericComplex</span></span>|<span data-ttu-id="36660-130">6 </span><span class="sxs-lookup"><span data-stu-id="36660-130">6</span></span>|<span data-ttu-id="36660-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="36660-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="36660-132">любой</span><span class="sxs-lookup"><span data-stu-id="36660-132">any</span></span>|<span data-ttu-id="36660-133">7 </span><span class="sxs-lookup"><span data-stu-id="36660-133">7</span></span>|<span data-ttu-id="36660-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="36660-134">A password or pattern is required, and any is acceptable.</span></span>|



