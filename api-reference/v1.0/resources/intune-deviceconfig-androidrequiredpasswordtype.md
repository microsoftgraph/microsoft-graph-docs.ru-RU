---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255404"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="35160-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="35160-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="35160-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35160-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35160-105">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="35160-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="35160-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="35160-106">Members</span></span>
|<span data-ttu-id="35160-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="35160-107">Member</span></span>|<span data-ttu-id="35160-108">Значение</span><span class="sxs-lookup"><span data-stu-id="35160-108">Value</span></span>|<span data-ttu-id="35160-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35160-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35160-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="35160-110">deviceDefault</span></span>|<span data-ttu-id="35160-111">нуль</span><span class="sxs-lookup"><span data-stu-id="35160-111">0</span></span>|<span data-ttu-id="35160-112">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="35160-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="35160-113">буквы</span><span class="sxs-lookup"><span data-stu-id="35160-113">alphabetic</span></span>|<span data-ttu-id="35160-114">1,1</span><span class="sxs-lookup"><span data-stu-id="35160-114">1</span></span>|<span data-ttu-id="35160-115">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="35160-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="35160-116">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="35160-116">alphanumeric</span></span>|<span data-ttu-id="35160-117">2</span><span class="sxs-lookup"><span data-stu-id="35160-117">2</span></span>|<span data-ttu-id="35160-118">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="35160-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="35160-119">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="35160-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="35160-120">4</span><span class="sxs-lookup"><span data-stu-id="35160-120">3</span></span>|<span data-ttu-id="35160-121">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="35160-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="35160-122">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="35160-122">lowSecurityBiometric</span></span>|<span data-ttu-id="35160-123">4</span><span class="sxs-lookup"><span data-stu-id="35160-123">4</span></span>|<span data-ttu-id="35160-124">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="35160-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="35160-125">числовых</span><span class="sxs-lookup"><span data-stu-id="35160-125">numeric</span></span>|<span data-ttu-id="35160-126">17:00</span><span class="sxs-lookup"><span data-stu-id="35160-126">5</span></span>|<span data-ttu-id="35160-127">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="35160-127">Numeric password required.</span></span>|
|<span data-ttu-id="35160-128">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="35160-128">numericComplex</span></span>|<span data-ttu-id="35160-129">6</span><span class="sxs-lookup"><span data-stu-id="35160-129">6</span></span>|<span data-ttu-id="35160-130">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="35160-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="35160-131">любой</span><span class="sxs-lookup"><span data-stu-id="35160-131">any</span></span>|<span data-ttu-id="35160-132">7</span><span class="sxs-lookup"><span data-stu-id="35160-132">7</span></span>|<span data-ttu-id="35160-133">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="35160-133">A password or pattern is required, and any is acceptable.</span></span>|



