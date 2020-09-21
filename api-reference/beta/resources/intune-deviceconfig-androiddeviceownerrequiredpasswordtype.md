---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d3df49d6ed508a8d9860c0bb37a234c9fd6e5c2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968698"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="9a899-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="9a899-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="9a899-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a899-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a899-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a899-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a899-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a899-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a899-107">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="9a899-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9a899-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9a899-108">Members</span></span>
|<span data-ttu-id="9a899-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9a899-109">Member</span></span>|<span data-ttu-id="9a899-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9a899-110">Value</span></span>|<span data-ttu-id="9a899-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9a899-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a899-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="9a899-112">deviceDefault</span></span>|<span data-ttu-id="9a899-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9a899-113">0</span></span>|<span data-ttu-id="9a899-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="9a899-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9a899-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9a899-115">required</span></span>|<span data-ttu-id="9a899-116">1 </span><span class="sxs-lookup"><span data-stu-id="9a899-116">1</span></span>|<span data-ttu-id="9a899-117">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="9a899-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="9a899-118">числовых</span><span class="sxs-lookup"><span data-stu-id="9a899-118">numeric</span></span>|<span data-ttu-id="9a899-119">2 </span><span class="sxs-lookup"><span data-stu-id="9a899-119">2</span></span>|<span data-ttu-id="9a899-120">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="9a899-120">At least numeric.</span></span>|
|<span data-ttu-id="9a899-121">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="9a899-121">numericComplex</span></span>|<span data-ttu-id="9a899-122">4</span><span class="sxs-lookup"><span data-stu-id="9a899-122">3</span></span>|<span data-ttu-id="9a899-123">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="9a899-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="9a899-124">буквы</span><span class="sxs-lookup"><span data-stu-id="9a899-124">alphabetic</span></span>|<span data-ttu-id="9a899-125">4 </span><span class="sxs-lookup"><span data-stu-id="9a899-125">4</span></span>|<span data-ttu-id="9a899-126">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="9a899-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="9a899-127">цифрового</span><span class="sxs-lookup"><span data-stu-id="9a899-127">alphanumeric</span></span>|<span data-ttu-id="9a899-128">5 </span><span class="sxs-lookup"><span data-stu-id="9a899-128">5</span></span>|<span data-ttu-id="9a899-129">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="9a899-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="9a899-130">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="9a899-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="9a899-131">6 </span><span class="sxs-lookup"><span data-stu-id="9a899-131">6</span></span>|<span data-ttu-id="9a899-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="9a899-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="9a899-133">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="9a899-133">lowSecurityBiometric</span></span>|<span data-ttu-id="9a899-134">7 </span><span class="sxs-lookup"><span data-stu-id="9a899-134">7</span></span>|<span data-ttu-id="9a899-135">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="9a899-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9a899-136">кустомпассворд</span><span class="sxs-lookup"><span data-stu-id="9a899-136">customPassword</span></span>|<span data-ttu-id="9a899-137">8 </span><span class="sxs-lookup"><span data-stu-id="9a899-137">8</span></span>|<span data-ttu-id="9a899-138">Настраиваемый пароль, заданный администратором.</span><span class="sxs-lookup"><span data-stu-id="9a899-138">Custom password set by the admin.</span></span>|






