---
title: тип enum androidWorkProfileRequiredPasswordType
description: Рабочий профиль Android требуется тип пароля.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 741a86f1ce4654fe6d5495521f055490d4c068bc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755947"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="195e8-103">тип enum androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="195e8-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="195e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="195e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="195e8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="195e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="195e8-106">Рабочий профиль Android требуется тип пароля.</span><span class="sxs-lookup"><span data-stu-id="195e8-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="195e8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="195e8-107">Members</span></span>
|<span data-ttu-id="195e8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="195e8-108">Member</span></span>|<span data-ttu-id="195e8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="195e8-109">Value</span></span>|<span data-ttu-id="195e8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="195e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="195e8-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="195e8-111">deviceDefault</span></span>|<span data-ttu-id="195e8-112">0</span><span class="sxs-lookup"><span data-stu-id="195e8-112">0</span></span>|<span data-ttu-id="195e8-113">Значение устройства по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="195e8-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="195e8-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="195e8-114">lowSecurityBiometric</span></span>|<span data-ttu-id="195e8-115">1</span><span class="sxs-lookup"><span data-stu-id="195e8-115">1</span></span>|<span data-ttu-id="195e8-116">Требуется пароль с низкой безопасностью на основе биометрии.</span><span class="sxs-lookup"><span data-stu-id="195e8-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="195e8-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="195e8-117">required</span></span>|<span data-ttu-id="195e8-118">2</span><span class="sxs-lookup"><span data-stu-id="195e8-118">2</span></span>|<span data-ttu-id="195e8-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="195e8-119">Required.</span></span>|
|<span data-ttu-id="195e8-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="195e8-120">atLeastNumeric</span></span>|<span data-ttu-id="195e8-121">3</span><span class="sxs-lookup"><span data-stu-id="195e8-121">3</span></span>|<span data-ttu-id="195e8-122">Требуется по крайней мере числовая пароль.</span><span class="sxs-lookup"><span data-stu-id="195e8-122">At least numeric password required.</span></span>|
|<span data-ttu-id="195e8-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="195e8-123">numericComplex</span></span>|<span data-ttu-id="195e8-124">4 </span><span class="sxs-lookup"><span data-stu-id="195e8-124">4</span></span>|<span data-ttu-id="195e8-125">Требуется числовый сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="195e8-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="195e8-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="195e8-126">atLeastAlphabetic</span></span>|<span data-ttu-id="195e8-127">5 </span><span class="sxs-lookup"><span data-stu-id="195e8-127">5</span></span>|<span data-ttu-id="195e8-128">Требуется по крайней мере алфавитный пароль.</span><span class="sxs-lookup"><span data-stu-id="195e8-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="195e8-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="195e8-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="195e8-130">6 </span><span class="sxs-lookup"><span data-stu-id="195e8-130">6</span></span>|<span data-ttu-id="195e8-131">Требуется, по крайней мере, альфа-числовая пароль.</span><span class="sxs-lookup"><span data-stu-id="195e8-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="195e8-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="195e8-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="195e8-133">7 </span><span class="sxs-lookup"><span data-stu-id="195e8-133">7</span></span>|<span data-ttu-id="195e8-134">По крайней мере, альфа-число с паролем символов.</span><span class="sxs-lookup"><span data-stu-id="195e8-134">At least alphanumeric with symbols password required.</span></span>|




