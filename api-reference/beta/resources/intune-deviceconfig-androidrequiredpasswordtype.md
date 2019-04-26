---
title: тип перечисления Андроидрекуиредпассвордтипе
description: Требуемый тип пароля для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562498"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="af422-103">тип перечисления Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="af422-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="af422-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af422-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af422-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af422-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af422-106">Требуемый тип пароля для Android.</span><span class="sxs-lookup"><span data-stu-id="af422-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="af422-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="af422-107">Members</span></span>
|<span data-ttu-id="af422-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="af422-108">Member</span></span>|<span data-ttu-id="af422-109">Значение</span><span class="sxs-lookup"><span data-stu-id="af422-109">Value</span></span>|<span data-ttu-id="af422-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af422-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af422-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="af422-111">deviceDefault</span></span>|<span data-ttu-id="af422-112">нуль</span><span class="sxs-lookup"><span data-stu-id="af422-112">0</span></span>|<span data-ttu-id="af422-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="af422-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="af422-114">буквы</span><span class="sxs-lookup"><span data-stu-id="af422-114">alphabetic</span></span>|<span data-ttu-id="af422-115">1 </span><span class="sxs-lookup"><span data-stu-id="af422-115">1</span></span>|<span data-ttu-id="af422-116">Необходим алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="af422-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="af422-117">цифрового</span><span class="sxs-lookup"><span data-stu-id="af422-117">alphanumeric</span></span>|<span data-ttu-id="af422-118">2 </span><span class="sxs-lookup"><span data-stu-id="af422-118">2</span></span>|<span data-ttu-id="af422-119">Необходимо указать буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="af422-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="af422-120">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="af422-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="af422-121">3 </span><span class="sxs-lookup"><span data-stu-id="af422-121">3</span></span>|<span data-ttu-id="af422-122">Требуются буквенно-цифровые символы с паролем.</span><span class="sxs-lookup"><span data-stu-id="af422-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="af422-123">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="af422-123">lowSecurityBiometric</span></span>|<span data-ttu-id="af422-124">4 </span><span class="sxs-lookup"><span data-stu-id="af422-124">4</span></span>|<span data-ttu-id="af422-125">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="af422-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="af422-126">числовых</span><span class="sxs-lookup"><span data-stu-id="af422-126">numeric</span></span>|<span data-ttu-id="af422-127">5 </span><span class="sxs-lookup"><span data-stu-id="af422-127">5</span></span>|<span data-ttu-id="af422-128">Необходим числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="af422-128">Numeric password required.</span></span>|
|<span data-ttu-id="af422-129">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="af422-129">numericComplex</span></span>|<span data-ttu-id="af422-130">6 </span><span class="sxs-lookup"><span data-stu-id="af422-130">6</span></span>|<span data-ttu-id="af422-131">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="af422-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="af422-132">любой</span><span class="sxs-lookup"><span data-stu-id="af422-132">any</span></span>|<span data-ttu-id="af422-133">7 </span><span class="sxs-lookup"><span data-stu-id="af422-133">7</span></span>|<span data-ttu-id="af422-134">Необходим пароль или шаблон, а любой из них приемлем.</span><span class="sxs-lookup"><span data-stu-id="af422-134">A password or pattern is required, and any is acceptable.</span></span>|





