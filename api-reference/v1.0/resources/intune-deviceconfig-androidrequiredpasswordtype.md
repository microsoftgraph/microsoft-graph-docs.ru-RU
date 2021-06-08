---
title: тип enum androidRequiredPasswordType
description: Тип пароля, требуемого для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d179666a4de9256e98c704bccd9e512d4aebd0ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760288"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="2e085-103">тип enum androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2e085-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="2e085-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e085-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e085-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e085-106">Тип пароля, требуемого для Android.</span><span class="sxs-lookup"><span data-stu-id="2e085-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="2e085-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2e085-107">Members</span></span>
|<span data-ttu-id="2e085-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2e085-108">Member</span></span>|<span data-ttu-id="2e085-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2e085-109">Value</span></span>|<span data-ttu-id="2e085-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e085-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e085-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2e085-111">deviceDefault</span></span>|<span data-ttu-id="2e085-112">0</span><span class="sxs-lookup"><span data-stu-id="2e085-112">0</span></span>|<span data-ttu-id="2e085-113">Значение устройства по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="2e085-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="2e085-114">алфавитный</span><span class="sxs-lookup"><span data-stu-id="2e085-114">alphabetic</span></span>|<span data-ttu-id="2e085-115">1</span><span class="sxs-lookup"><span data-stu-id="2e085-115">1</span></span>|<span data-ttu-id="2e085-116">Требуется алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="2e085-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="2e085-117">alphanumeric</span><span class="sxs-lookup"><span data-stu-id="2e085-117">alphanumeric</span></span>|<span data-ttu-id="2e085-118">2</span><span class="sxs-lookup"><span data-stu-id="2e085-118">2</span></span>|<span data-ttu-id="2e085-119">Необходимый альфа-пароль.</span><span class="sxs-lookup"><span data-stu-id="2e085-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="2e085-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="2e085-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="2e085-121">3</span><span class="sxs-lookup"><span data-stu-id="2e085-121">3</span></span>|<span data-ttu-id="2e085-122">Альфа-число с паролем символов.</span><span class="sxs-lookup"><span data-stu-id="2e085-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="2e085-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="2e085-123">lowSecurityBiometric</span></span>|<span data-ttu-id="2e085-124">4 </span><span class="sxs-lookup"><span data-stu-id="2e085-124">4</span></span>|<span data-ttu-id="2e085-125">Требуется пароль с низкой безопасностью на основе биометрии.</span><span class="sxs-lookup"><span data-stu-id="2e085-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="2e085-126">числовая</span><span class="sxs-lookup"><span data-stu-id="2e085-126">numeric</span></span>|<span data-ttu-id="2e085-127">5 </span><span class="sxs-lookup"><span data-stu-id="2e085-127">5</span></span>|<span data-ttu-id="2e085-128">Необходимый числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="2e085-128">Numeric password required.</span></span>|
|<span data-ttu-id="2e085-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="2e085-129">numericComplex</span></span>|<span data-ttu-id="2e085-130">6 </span><span class="sxs-lookup"><span data-stu-id="2e085-130">6</span></span>|<span data-ttu-id="2e085-131">Требуется числовый сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="2e085-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="2e085-132">любой</span><span class="sxs-lookup"><span data-stu-id="2e085-132">any</span></span>|<span data-ttu-id="2e085-133">7 </span><span class="sxs-lookup"><span data-stu-id="2e085-133">7</span></span>|<span data-ttu-id="2e085-134">Требуется пароль или шаблон, и любой из них является приемлемым.</span><span class="sxs-lookup"><span data-stu-id="2e085-134">A password or pattern is required, and any is acceptable.</span></span>|




