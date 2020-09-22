---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3aaf2ad668e87f7f3fee1a8f168845203704a5a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021553"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="7319a-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="7319a-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="7319a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7319a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7319a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7319a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7319a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7319a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7319a-107">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="7319a-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="7319a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7319a-108">Members</span></span>
|<span data-ttu-id="7319a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7319a-109">Member</span></span>|<span data-ttu-id="7319a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7319a-110">Value</span></span>|<span data-ttu-id="7319a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7319a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7319a-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="7319a-112">deviceDefault</span></span>|<span data-ttu-id="7319a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7319a-113">0</span></span>|<span data-ttu-id="7319a-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="7319a-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="7319a-115">буквы</span><span class="sxs-lookup"><span data-stu-id="7319a-115">alphabetic</span></span>|<span data-ttu-id="7319a-116">1 </span><span class="sxs-lookup"><span data-stu-id="7319a-116">1</span></span>|<span data-ttu-id="7319a-117">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="7319a-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="7319a-118">цифрового</span><span class="sxs-lookup"><span data-stu-id="7319a-118">alphanumeric</span></span>|<span data-ttu-id="7319a-119">2 </span><span class="sxs-lookup"><span data-stu-id="7319a-119">2</span></span>|<span data-ttu-id="7319a-120">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="7319a-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="7319a-121">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="7319a-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="7319a-122">4</span><span class="sxs-lookup"><span data-stu-id="7319a-122">3</span></span>|<span data-ttu-id="7319a-123">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="7319a-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="7319a-124">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="7319a-124">lowSecurityBiometric</span></span>|<span data-ttu-id="7319a-125">4 </span><span class="sxs-lookup"><span data-stu-id="7319a-125">4</span></span>|<span data-ttu-id="7319a-126">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="7319a-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="7319a-127">числовых</span><span class="sxs-lookup"><span data-stu-id="7319a-127">numeric</span></span>|<span data-ttu-id="7319a-128">5 </span><span class="sxs-lookup"><span data-stu-id="7319a-128">5</span></span>|<span data-ttu-id="7319a-129">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="7319a-129">Numeric password required.</span></span>|
|<span data-ttu-id="7319a-130">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="7319a-130">numericComplex</span></span>|<span data-ttu-id="7319a-131">6 </span><span class="sxs-lookup"><span data-stu-id="7319a-131">6</span></span>|<span data-ttu-id="7319a-132">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="7319a-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="7319a-133">любой</span><span class="sxs-lookup"><span data-stu-id="7319a-133">any</span></span>|<span data-ttu-id="7319a-134">7 </span><span class="sxs-lookup"><span data-stu-id="7319a-134">7</span></span>|<span data-ttu-id="7319a-135">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="7319a-135">A password or pattern is required, and any is acceptable.</span></span>|






