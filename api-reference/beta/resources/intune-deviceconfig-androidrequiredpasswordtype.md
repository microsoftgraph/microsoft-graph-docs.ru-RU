---
title: Тип перечисления androidRequiredPasswordType
description: Тип Android пароль.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eebc6b0ad6eed346927fd48a2dc1f82b5e529b28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392915"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="0392e-103">Тип перечисления androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0392e-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="0392e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0392e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0392e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0392e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0392e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0392e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0392e-107">Тип Android пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="0392e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0392e-108">Members</span></span>
|<span data-ttu-id="0392e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0392e-109">Member</span></span>|<span data-ttu-id="0392e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0392e-110">Value</span></span>|<span data-ttu-id="0392e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0392e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0392e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0392e-112">deviceDefault</span></span>|<span data-ttu-id="0392e-113">0</span><span class="sxs-lookup"><span data-stu-id="0392e-113">0</span></span>|<span data-ttu-id="0392e-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="0392e-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="0392e-115">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="0392e-115">alphabetic</span></span>|<span data-ttu-id="0392e-116">1</span><span class="sxs-lookup"><span data-stu-id="0392e-116">1</span></span>|<span data-ttu-id="0392e-117">К буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="0392e-118">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="0392e-118">alphanumeric</span></span>|<span data-ttu-id="0392e-119">2</span><span class="sxs-lookup"><span data-stu-id="0392e-119">2</span></span>|<span data-ttu-id="0392e-120">Буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="0392e-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="0392e-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="0392e-122">3</span><span class="sxs-lookup"><span data-stu-id="0392e-122">3</span></span>|<span data-ttu-id="0392e-123">Буквы или цифры с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="0392e-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="0392e-124">lowSecurityBiometric</span></span>|<span data-ttu-id="0392e-125">4</span><span class="sxs-lookup"><span data-stu-id="0392e-125">4</span></span>|<span data-ttu-id="0392e-126">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0392e-127">числовое</span><span class="sxs-lookup"><span data-stu-id="0392e-127">numeric</span></span>|<span data-ttu-id="0392e-128">5</span><span class="sxs-lookup"><span data-stu-id="0392e-128">5</span></span>|<span data-ttu-id="0392e-129">Числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-129">Numeric password required.</span></span>|
|<span data-ttu-id="0392e-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="0392e-130">numericComplex</span></span>|<span data-ttu-id="0392e-131">6</span><span class="sxs-lookup"><span data-stu-id="0392e-131">6</span></span>|<span data-ttu-id="0392e-132">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="0392e-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="0392e-133">любой</span><span class="sxs-lookup"><span data-stu-id="0392e-133">any</span></span>|<span data-ttu-id="0392e-134">7</span><span class="sxs-lookup"><span data-stu-id="0392e-134">7</span></span>|<span data-ttu-id="0392e-135">Пароль или шаблон является обязательным, а какие-либо допустима.</span><span class="sxs-lookup"><span data-stu-id="0392e-135">A password or pattern is required, and any is acceptable.</span></span>|




