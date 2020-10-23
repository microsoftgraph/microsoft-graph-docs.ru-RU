---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f78829f47a8f1d029ed78b2fb0d63192af69a3e6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725605"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f8c8e-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f8c8e-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="f8c8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8c8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8c8e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8c8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8c8e-107">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f8c8e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f8c8e-108">Members</span></span>
|<span data-ttu-id="f8c8e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f8c8e-109">Member</span></span>|<span data-ttu-id="f8c8e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f8c8e-110">Value</span></span>|<span data-ttu-id="f8c8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f8c8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8c8e-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="f8c8e-112">deviceDefault</span></span>|<span data-ttu-id="f8c8e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f8c8e-113">0</span></span>|<span data-ttu-id="f8c8e-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f8c8e-115">буквы</span><span class="sxs-lookup"><span data-stu-id="f8c8e-115">alphabetic</span></span>|<span data-ttu-id="f8c8e-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f8c8e-116">1</span></span>|<span data-ttu-id="f8c8e-117">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="f8c8e-118">цифрового</span><span class="sxs-lookup"><span data-stu-id="f8c8e-118">alphanumeric</span></span>|<span data-ttu-id="f8c8e-119">2</span><span class="sxs-lookup"><span data-stu-id="f8c8e-119">2</span></span>|<span data-ttu-id="f8c8e-120">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f8c8e-121">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="f8c8e-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="f8c8e-122">4</span><span class="sxs-lookup"><span data-stu-id="f8c8e-122">3</span></span>|<span data-ttu-id="f8c8e-123">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f8c8e-124">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="f8c8e-124">lowSecurityBiometric</span></span>|<span data-ttu-id="f8c8e-125">4 </span><span class="sxs-lookup"><span data-stu-id="f8c8e-125">4</span></span>|<span data-ttu-id="f8c8e-126">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f8c8e-127">числовых</span><span class="sxs-lookup"><span data-stu-id="f8c8e-127">numeric</span></span>|<span data-ttu-id="f8c8e-128">5 </span><span class="sxs-lookup"><span data-stu-id="f8c8e-128">5</span></span>|<span data-ttu-id="f8c8e-129">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-129">Numeric password required.</span></span>|
|<span data-ttu-id="f8c8e-130">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="f8c8e-130">numericComplex</span></span>|<span data-ttu-id="f8c8e-131">6 </span><span class="sxs-lookup"><span data-stu-id="f8c8e-131">6</span></span>|<span data-ttu-id="f8c8e-132">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="f8c8e-133">любой</span><span class="sxs-lookup"><span data-stu-id="f8c8e-133">any</span></span>|<span data-ttu-id="f8c8e-134">7 </span><span class="sxs-lookup"><span data-stu-id="f8c8e-134">7</span></span>|<span data-ttu-id="f8c8e-135">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="f8c8e-135">A password or pattern is required, and any is acceptable.</span></span>|





