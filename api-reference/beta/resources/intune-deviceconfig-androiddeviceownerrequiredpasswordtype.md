---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c575b1b39592eb8191e358563abb6d6bd834e7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802354"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="716c4-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="716c4-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="716c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="716c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="716c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="716c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="716c4-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="716c4-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="716c4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="716c4-107">Members</span></span>
|<span data-ttu-id="716c4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="716c4-108">Member</span></span>|<span data-ttu-id="716c4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="716c4-109">Value</span></span>|<span data-ttu-id="716c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="716c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="716c4-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="716c4-111">deviceDefault</span></span>|<span data-ttu-id="716c4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="716c4-112">0</span></span>|<span data-ttu-id="716c4-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="716c4-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="716c4-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="716c4-114">required</span></span>|<span data-ttu-id="716c4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="716c4-115">1</span></span>|<span data-ttu-id="716c4-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="716c4-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="716c4-117">числовых</span><span class="sxs-lookup"><span data-stu-id="716c4-117">numeric</span></span>|<span data-ttu-id="716c4-118">2</span><span class="sxs-lookup"><span data-stu-id="716c4-118">2</span></span>|<span data-ttu-id="716c4-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="716c4-119">At least numeric.</span></span>|
|<span data-ttu-id="716c4-120">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="716c4-120">numericComplex</span></span>|<span data-ttu-id="716c4-121">4</span><span class="sxs-lookup"><span data-stu-id="716c4-121">3</span></span>|<span data-ttu-id="716c4-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="716c4-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="716c4-123">буквы</span><span class="sxs-lookup"><span data-stu-id="716c4-123">alphabetic</span></span>|<span data-ttu-id="716c4-124">SP4</span><span class="sxs-lookup"><span data-stu-id="716c4-124">4</span></span>|<span data-ttu-id="716c4-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="716c4-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="716c4-126">цифрового</span><span class="sxs-lookup"><span data-stu-id="716c4-126">alphanumeric</span></span>|<span data-ttu-id="716c4-127">17:00</span><span class="sxs-lookup"><span data-stu-id="716c4-127">5</span></span>|<span data-ttu-id="716c4-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="716c4-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="716c4-129">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="716c4-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="716c4-130">ICMPv6</span><span class="sxs-lookup"><span data-stu-id="716c4-130">6</span></span>|<span data-ttu-id="716c4-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="716c4-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="716c4-132">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="716c4-132">lowSecurityBiometric</span></span>|<span data-ttu-id="716c4-133">см</span><span class="sxs-lookup"><span data-stu-id="716c4-133">7</span></span>|<span data-ttu-id="716c4-134">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="716c4-134">Low security biometrics based password required.</span></span>|





