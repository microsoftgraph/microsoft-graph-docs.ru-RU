---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 376e33edac921f6771d76a45622a58bca3076c5c
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572336"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="15fac-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="15fac-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="15fac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15fac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15fac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15fac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15fac-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="15fac-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="15fac-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="15fac-107">Members</span></span>
|<span data-ttu-id="15fac-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="15fac-108">Member</span></span>|<span data-ttu-id="15fac-109">Значение</span><span class="sxs-lookup"><span data-stu-id="15fac-109">Value</span></span>|<span data-ttu-id="15fac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15fac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15fac-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="15fac-111">deviceDefault</span></span>|<span data-ttu-id="15fac-112">нуль</span><span class="sxs-lookup"><span data-stu-id="15fac-112">0</span></span>|<span data-ttu-id="15fac-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="15fac-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="15fac-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="15fac-114">required</span></span>|<span data-ttu-id="15fac-115">1,1</span><span class="sxs-lookup"><span data-stu-id="15fac-115">1</span></span>|<span data-ttu-id="15fac-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="15fac-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="15fac-117">числовых</span><span class="sxs-lookup"><span data-stu-id="15fac-117">numeric</span></span>|<span data-ttu-id="15fac-118">2</span><span class="sxs-lookup"><span data-stu-id="15fac-118">2</span></span>|<span data-ttu-id="15fac-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="15fac-119">At least numeric.</span></span>|
|<span data-ttu-id="15fac-120">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="15fac-120">numericComplex</span></span>|<span data-ttu-id="15fac-121">4</span><span class="sxs-lookup"><span data-stu-id="15fac-121">3</span></span>|<span data-ttu-id="15fac-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="15fac-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="15fac-123">буквы</span><span class="sxs-lookup"><span data-stu-id="15fac-123">alphabetic</span></span>|<span data-ttu-id="15fac-124">SP4</span><span class="sxs-lookup"><span data-stu-id="15fac-124">4</span></span>|<span data-ttu-id="15fac-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="15fac-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="15fac-126">цифрового</span><span class="sxs-lookup"><span data-stu-id="15fac-126">alphanumeric</span></span>|<span data-ttu-id="15fac-127">17:00</span><span class="sxs-lookup"><span data-stu-id="15fac-127">5</span></span>|<span data-ttu-id="15fac-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="15fac-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="15fac-129">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="15fac-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="15fac-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="15fac-130">6</span></span>|<span data-ttu-id="15fac-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="15fac-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="15fac-132">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="15fac-132">lowSecurityBiometric</span></span>|<span data-ttu-id="15fac-133">см</span><span class="sxs-lookup"><span data-stu-id="15fac-133">7</span></span>|<span data-ttu-id="15fac-134">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="15fac-134">Low security biometrics based password required.</span></span>|




