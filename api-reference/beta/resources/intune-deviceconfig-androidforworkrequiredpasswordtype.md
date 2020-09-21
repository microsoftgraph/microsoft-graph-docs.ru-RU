---
title: тип перечисления Андроидфорворкрекуиредпассвордтипе
description: Для работы Android необходим тип пароля.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20c7e330d060346557717e9eea0924b275c60d04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968495"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="3fd5c-103">тип перечисления Андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="3fd5c-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="3fd5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fd5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fd5c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fd5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd5c-107">Для работы Android необходим тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="3fd5c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3fd5c-108">Members</span></span>
|<span data-ttu-id="3fd5c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3fd5c-109">Member</span></span>|<span data-ttu-id="3fd5c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3fd5c-110">Value</span></span>|<span data-ttu-id="3fd5c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3fd5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd5c-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="3fd5c-112">deviceDefault</span></span>|<span data-ttu-id="3fd5c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3fd5c-113">0</span></span>|<span data-ttu-id="3fd5c-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="3fd5c-115">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="3fd5c-115">lowSecurityBiometric</span></span>|<span data-ttu-id="3fd5c-116">1 </span><span class="sxs-lookup"><span data-stu-id="3fd5c-116">1</span></span>|<span data-ttu-id="3fd5c-117">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="3fd5c-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="3fd5c-118">required</span></span>|<span data-ttu-id="3fd5c-119">2 </span><span class="sxs-lookup"><span data-stu-id="3fd5c-119">2</span></span>|<span data-ttu-id="3fd5c-120">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-120">Required.</span></span>|
|<span data-ttu-id="3fd5c-121">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="3fd5c-121">atLeastNumeric</span></span>|<span data-ttu-id="3fd5c-122">4</span><span class="sxs-lookup"><span data-stu-id="3fd5c-122">3</span></span>|<span data-ttu-id="3fd5c-123">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-123">At least numeric password required.</span></span>|
|<span data-ttu-id="3fd5c-124">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="3fd5c-124">numericComplex</span></span>|<span data-ttu-id="3fd5c-125">4 </span><span class="sxs-lookup"><span data-stu-id="3fd5c-125">4</span></span>|<span data-ttu-id="3fd5c-126">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="3fd5c-127">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="3fd5c-127">atLeastAlphabetic</span></span>|<span data-ttu-id="3fd5c-128">5 </span><span class="sxs-lookup"><span data-stu-id="3fd5c-128">5</span></span>|<span data-ttu-id="3fd5c-129">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="3fd5c-130">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="3fd5c-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="3fd5c-131">6 </span><span class="sxs-lookup"><span data-stu-id="3fd5c-131">6</span></span>|<span data-ttu-id="3fd5c-132">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="3fd5c-133">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="3fd5c-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="3fd5c-134">7 </span><span class="sxs-lookup"><span data-stu-id="3fd5c-134">7</span></span>|<span data-ttu-id="3fd5c-135">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="3fd5c-135">At least alphanumeric with symbols password required.</span></span>|






