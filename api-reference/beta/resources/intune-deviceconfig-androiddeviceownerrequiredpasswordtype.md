---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6d783f8bdf5faeed2d3e10a9286a897c8d85783
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796988"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="cd4ac-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="cd4ac-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="cd4ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd4ac-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd4ac-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="cd4ac-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cd4ac-107">Members</span></span>
|<span data-ttu-id="cd4ac-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cd4ac-108">Member</span></span>|<span data-ttu-id="cd4ac-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cd4ac-109">Value</span></span>|<span data-ttu-id="cd4ac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd4ac-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="cd4ac-111">deviceDefault</span></span>|<span data-ttu-id="cd4ac-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cd4ac-112">0</span></span>|<span data-ttu-id="cd4ac-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="cd4ac-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="cd4ac-114">required</span></span>|<span data-ttu-id="cd4ac-115">1,1</span><span class="sxs-lookup"><span data-stu-id="cd4ac-115">1</span></span>|<span data-ttu-id="cd4ac-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="cd4ac-117">числовых</span><span class="sxs-lookup"><span data-stu-id="cd4ac-117">numeric</span></span>|<span data-ttu-id="cd4ac-118">2</span><span class="sxs-lookup"><span data-stu-id="cd4ac-118">2</span></span>|<span data-ttu-id="cd4ac-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-119">At least numeric.</span></span>|
|<span data-ttu-id="cd4ac-120">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="cd4ac-120">numericComplex</span></span>|<span data-ttu-id="cd4ac-121">4</span><span class="sxs-lookup"><span data-stu-id="cd4ac-121">3</span></span>|<span data-ttu-id="cd4ac-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="cd4ac-123">буквы</span><span class="sxs-lookup"><span data-stu-id="cd4ac-123">alphabetic</span></span>|<span data-ttu-id="cd4ac-124">4 </span><span class="sxs-lookup"><span data-stu-id="cd4ac-124">4</span></span>|<span data-ttu-id="cd4ac-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="cd4ac-126">цифрового</span><span class="sxs-lookup"><span data-stu-id="cd4ac-126">alphanumeric</span></span>|<span data-ttu-id="cd4ac-127">5 </span><span class="sxs-lookup"><span data-stu-id="cd4ac-127">5</span></span>|<span data-ttu-id="cd4ac-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="cd4ac-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="cd4ac-129">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="cd4ac-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="cd4ac-130">6 </span><span class="sxs-lookup"><span data-stu-id="cd4ac-130">6</span></span>|<span data-ttu-id="cd4ac-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="cd4ac-132">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="cd4ac-132">lowSecurityBiometric</span></span>|<span data-ttu-id="cd4ac-133">7 </span><span class="sxs-lookup"><span data-stu-id="cd4ac-133">7</span></span>|<span data-ttu-id="cd4ac-134">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-134">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="cd4ac-135">кустомпассворд</span><span class="sxs-lookup"><span data-stu-id="cd4ac-135">customPassword</span></span>|<span data-ttu-id="cd4ac-136">8 </span><span class="sxs-lookup"><span data-stu-id="cd4ac-136">8</span></span>|<span data-ttu-id="cd4ac-137">Настраиваемый пароль, заданный администратором.</span><span class="sxs-lookup"><span data-stu-id="cd4ac-137">Custom password set by the admin.</span></span>|



