---
title: Тип перечисления androidRequiredPasswordType
description: Тип Android пароль.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c85466cf722848efa684fc7b5643293d49de2459
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964090"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="a13af-103">Тип перечисления androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a13af-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a13af-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a13af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a13af-105">Тип Android пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="a13af-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a13af-106">Members</span></span>
|<span data-ttu-id="a13af-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a13af-107">Member</span></span>|<span data-ttu-id="a13af-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a13af-108">Value</span></span>|<span data-ttu-id="a13af-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a13af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a13af-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a13af-110">deviceDefault</span></span>|<span data-ttu-id="a13af-111">0</span><span class="sxs-lookup"><span data-stu-id="a13af-111">0</span></span>|<span data-ttu-id="a13af-112">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="a13af-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="a13af-113">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="a13af-113">alphabetic</span></span>|<span data-ttu-id="a13af-114">1</span><span class="sxs-lookup"><span data-stu-id="a13af-114">1</span></span>|<span data-ttu-id="a13af-115">К буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="a13af-116">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="a13af-116">alphanumeric</span></span>|<span data-ttu-id="a13af-117">2</span><span class="sxs-lookup"><span data-stu-id="a13af-117">2</span></span>|<span data-ttu-id="a13af-118">Буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="a13af-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a13af-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="a13af-120">3</span><span class="sxs-lookup"><span data-stu-id="a13af-120">3</span></span>|<span data-ttu-id="a13af-121">Буквы или цифры с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="a13af-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a13af-122">lowSecurityBiometric</span></span>|<span data-ttu-id="a13af-123">4</span><span class="sxs-lookup"><span data-stu-id="a13af-123">4</span></span>|<span data-ttu-id="a13af-124">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a13af-125">числовое</span><span class="sxs-lookup"><span data-stu-id="a13af-125">numeric</span></span>|<span data-ttu-id="a13af-126">5</span><span class="sxs-lookup"><span data-stu-id="a13af-126">5</span></span>|<span data-ttu-id="a13af-127">Числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-127">Numeric password required.</span></span>|
|<span data-ttu-id="a13af-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a13af-128">numericComplex</span></span>|<span data-ttu-id="a13af-129">6</span><span class="sxs-lookup"><span data-stu-id="a13af-129">6</span></span>|<span data-ttu-id="a13af-130">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="a13af-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="a13af-131">любой</span><span class="sxs-lookup"><span data-stu-id="a13af-131">any</span></span>|<span data-ttu-id="a13af-132">7</span><span class="sxs-lookup"><span data-stu-id="a13af-132">7</span></span>|<span data-ttu-id="a13af-133">Пароль или шаблон является обязательным, а какие-либо допустима.</span><span class="sxs-lookup"><span data-stu-id="a13af-133">A password or pattern is required, and any is acceptable.</span></span>|



