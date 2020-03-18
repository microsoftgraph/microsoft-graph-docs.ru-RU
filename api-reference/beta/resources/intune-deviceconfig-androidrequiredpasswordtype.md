---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ceac6e3953615524fb78b14c380218bf5c43f19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796736"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="e5105-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="e5105-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="e5105-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5105-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5105-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5105-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5105-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="e5105-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e5105-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e5105-107">Members</span></span>
|<span data-ttu-id="e5105-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e5105-108">Member</span></span>|<span data-ttu-id="e5105-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e5105-109">Value</span></span>|<span data-ttu-id="e5105-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5105-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5105-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="e5105-111">deviceDefault</span></span>|<span data-ttu-id="e5105-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e5105-112">0</span></span>|<span data-ttu-id="e5105-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="e5105-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="e5105-114">буквы</span><span class="sxs-lookup"><span data-stu-id="e5105-114">alphabetic</span></span>|<span data-ttu-id="e5105-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e5105-115">1</span></span>|<span data-ttu-id="e5105-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="e5105-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="e5105-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="e5105-117">alphanumeric</span></span>|<span data-ttu-id="e5105-118">2</span><span class="sxs-lookup"><span data-stu-id="e5105-118">2</span></span>|<span data-ttu-id="e5105-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="e5105-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="e5105-120">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="e5105-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="e5105-121">4</span><span class="sxs-lookup"><span data-stu-id="e5105-121">3</span></span>|<span data-ttu-id="e5105-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="e5105-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="e5105-123">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="e5105-123">lowSecurityBiometric</span></span>|<span data-ttu-id="e5105-124">4 </span><span class="sxs-lookup"><span data-stu-id="e5105-124">4</span></span>|<span data-ttu-id="e5105-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="e5105-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e5105-126">числовых</span><span class="sxs-lookup"><span data-stu-id="e5105-126">numeric</span></span>|<span data-ttu-id="e5105-127">5 </span><span class="sxs-lookup"><span data-stu-id="e5105-127">5</span></span>|<span data-ttu-id="e5105-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="e5105-128">Numeric password required.</span></span>|
|<span data-ttu-id="e5105-129">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="e5105-129">numericComplex</span></span>|<span data-ttu-id="e5105-130">6 </span><span class="sxs-lookup"><span data-stu-id="e5105-130">6</span></span>|<span data-ttu-id="e5105-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="e5105-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="e5105-132">любой</span><span class="sxs-lookup"><span data-stu-id="e5105-132">any</span></span>|<span data-ttu-id="e5105-133">7 </span><span class="sxs-lookup"><span data-stu-id="e5105-133">7</span></span>|<span data-ttu-id="e5105-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="e5105-134">A password or pattern is required, and any is acceptable.</span></span>|



