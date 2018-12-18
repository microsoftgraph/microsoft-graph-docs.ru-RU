---
title: Тип перечисления androidRequiredPasswordType
description: Тип Android пароль.
author: tfitzmac
ms.openlocfilehash: e9b757dc86bf71462f7f987cedfcd9e04497880e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349219"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="1c518-103">Тип перечисления androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1c518-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="1c518-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1c518-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c518-105">Тип Android пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-105">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="1c518-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="1c518-106">Members</span></span>
|<span data-ttu-id="1c518-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="1c518-107">Member</span></span>|<span data-ttu-id="1c518-108">Значение</span><span class="sxs-lookup"><span data-stu-id="1c518-108">Value</span></span>|<span data-ttu-id="1c518-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1c518-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c518-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1c518-110">deviceDefault</span></span>|<span data-ttu-id="1c518-111">0</span><span class="sxs-lookup"><span data-stu-id="1c518-111">0</span></span>|<span data-ttu-id="1c518-112">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="1c518-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="1c518-113">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="1c518-113">alphabetic</span></span>|<span data-ttu-id="1c518-114">1</span><span class="sxs-lookup"><span data-stu-id="1c518-114">1</span></span>|<span data-ttu-id="1c518-115">К буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="1c518-116">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="1c518-116">alphanumeric</span></span>|<span data-ttu-id="1c518-117">2</span><span class="sxs-lookup"><span data-stu-id="1c518-117">2</span></span>|<span data-ttu-id="1c518-118">Буквенно-цифровой пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="1c518-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="1c518-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="1c518-120">3</span><span class="sxs-lookup"><span data-stu-id="1c518-120">3</span></span>|<span data-ttu-id="1c518-121">Буквы или цифры с символы пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="1c518-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="1c518-122">lowSecurityBiometric</span></span>|<span data-ttu-id="1c518-123">4</span><span class="sxs-lookup"><span data-stu-id="1c518-123">4</span></span>|<span data-ttu-id="1c518-124">Биометрия низкой безопасности на основе пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="1c518-125">числовое</span><span class="sxs-lookup"><span data-stu-id="1c518-125">numeric</span></span>|<span data-ttu-id="1c518-126">5</span><span class="sxs-lookup"><span data-stu-id="1c518-126">5</span></span>|<span data-ttu-id="1c518-127">Числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-127">Numeric password required.</span></span>|
|<span data-ttu-id="1c518-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="1c518-128">numericComplex</span></span>|<span data-ttu-id="1c518-129">6</span><span class="sxs-lookup"><span data-stu-id="1c518-129">6</span></span>|<span data-ttu-id="1c518-130">Числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="1c518-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="1c518-131">любой</span><span class="sxs-lookup"><span data-stu-id="1c518-131">any</span></span>|<span data-ttu-id="1c518-132">7</span><span class="sxs-lookup"><span data-stu-id="1c518-132">7</span></span>|<span data-ttu-id="1c518-133">Пароль или шаблон является обязательным, а какие-либо допустима.</span><span class="sxs-lookup"><span data-stu-id="1c518-133">A password or pattern is required, and any is acceptable.</span></span>|



