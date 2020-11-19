---
title: тип перечисления Андроидфорворкрекуиредпассвордтипе
description: Для работы Android необходим тип пароля.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 381febc21db2951393b42689acecf4b729eb0b0f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216537"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="11348-103">тип перечисления Андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="11348-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="11348-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11348-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11348-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11348-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11348-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11348-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11348-107">Для работы Android необходим тип пароля.</span><span class="sxs-lookup"><span data-stu-id="11348-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="11348-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="11348-108">Members</span></span>
|<span data-ttu-id="11348-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="11348-109">Member</span></span>|<span data-ttu-id="11348-110">Значение</span><span class="sxs-lookup"><span data-stu-id="11348-110">Value</span></span>|<span data-ttu-id="11348-111">Описание</span><span class="sxs-lookup"><span data-stu-id="11348-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11348-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="11348-112">deviceDefault</span></span>|<span data-ttu-id="11348-113">нуль</span><span class="sxs-lookup"><span data-stu-id="11348-113">0</span></span>|<span data-ttu-id="11348-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="11348-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="11348-115">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="11348-115">lowSecurityBiometric</span></span>|<span data-ttu-id="11348-116">1,1</span><span class="sxs-lookup"><span data-stu-id="11348-116">1</span></span>|<span data-ttu-id="11348-117">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="11348-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="11348-118">Обязательный</span><span class="sxs-lookup"><span data-stu-id="11348-118">required</span></span>|<span data-ttu-id="11348-119">2</span><span class="sxs-lookup"><span data-stu-id="11348-119">2</span></span>|<span data-ttu-id="11348-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11348-120">Required.</span></span>|
|<span data-ttu-id="11348-121">атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="11348-121">atLeastNumeric</span></span>|<span data-ttu-id="11348-122">4</span><span class="sxs-lookup"><span data-stu-id="11348-122">3</span></span>|<span data-ttu-id="11348-123">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="11348-123">At least numeric password required.</span></span>|
|<span data-ttu-id="11348-124">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="11348-124">numericComplex</span></span>|<span data-ttu-id="11348-125">4 </span><span class="sxs-lookup"><span data-stu-id="11348-125">4</span></span>|<span data-ttu-id="11348-126">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="11348-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="11348-127">атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="11348-127">atLeastAlphabetic</span></span>|<span data-ttu-id="11348-128">5 </span><span class="sxs-lookup"><span data-stu-id="11348-128">5</span></span>|<span data-ttu-id="11348-129">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="11348-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="11348-130">атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="11348-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="11348-131">6 </span><span class="sxs-lookup"><span data-stu-id="11348-131">6</span></span>|<span data-ttu-id="11348-132">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="11348-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="11348-133">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="11348-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="11348-134">7 </span><span class="sxs-lookup"><span data-stu-id="11348-134">7</span></span>|<span data-ttu-id="11348-135">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="11348-135">At least alphanumeric with symbols password required.</span></span>|




