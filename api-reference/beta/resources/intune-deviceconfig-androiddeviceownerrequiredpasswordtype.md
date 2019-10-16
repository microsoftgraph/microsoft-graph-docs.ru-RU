---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a94dabb436ec11dd340c15afcbd7ed2f04ddbca
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538639"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="0598b-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="0598b-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="0598b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0598b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0598b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0598b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0598b-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="0598b-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="0598b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0598b-107">Members</span></span>
|<span data-ttu-id="0598b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0598b-108">Member</span></span>|<span data-ttu-id="0598b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0598b-109">Value</span></span>|<span data-ttu-id="0598b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0598b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0598b-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="0598b-111">deviceDefault</span></span>|<span data-ttu-id="0598b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0598b-112">0</span></span>|<span data-ttu-id="0598b-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="0598b-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="0598b-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0598b-114">required</span></span>|<span data-ttu-id="0598b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0598b-115">1</span></span>|<span data-ttu-id="0598b-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="0598b-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="0598b-117">числовых</span><span class="sxs-lookup"><span data-stu-id="0598b-117">numeric</span></span>|<span data-ttu-id="0598b-118">2</span><span class="sxs-lookup"><span data-stu-id="0598b-118">2</span></span>|<span data-ttu-id="0598b-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="0598b-119">At least numeric.</span></span>|
|<span data-ttu-id="0598b-120">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="0598b-120">numericComplex</span></span>|<span data-ttu-id="0598b-121">4</span><span class="sxs-lookup"><span data-stu-id="0598b-121">3</span></span>|<span data-ttu-id="0598b-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="0598b-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="0598b-123">буквы</span><span class="sxs-lookup"><span data-stu-id="0598b-123">alphabetic</span></span>|<span data-ttu-id="0598b-124">4 </span><span class="sxs-lookup"><span data-stu-id="0598b-124">4</span></span>|<span data-ttu-id="0598b-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="0598b-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="0598b-126">цифрового</span><span class="sxs-lookup"><span data-stu-id="0598b-126">alphanumeric</span></span>|<span data-ttu-id="0598b-127">5 </span><span class="sxs-lookup"><span data-stu-id="0598b-127">5</span></span>|<span data-ttu-id="0598b-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="0598b-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="0598b-129">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="0598b-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="0598b-130">6 </span><span class="sxs-lookup"><span data-stu-id="0598b-130">6</span></span>|<span data-ttu-id="0598b-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="0598b-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="0598b-132">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="0598b-132">lowSecurityBiometric</span></span>|<span data-ttu-id="0598b-133">7 </span><span class="sxs-lookup"><span data-stu-id="0598b-133">7</span></span>|<span data-ttu-id="0598b-134">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="0598b-134">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0598b-135">кустомпассворд</span><span class="sxs-lookup"><span data-stu-id="0598b-135">customPassword</span></span>|<span data-ttu-id="0598b-136">8 </span><span class="sxs-lookup"><span data-stu-id="0598b-136">8</span></span>|<span data-ttu-id="0598b-137">Настраиваемый пароль, заданный администратором.</span><span class="sxs-lookup"><span data-stu-id="0598b-137">Custom password set by the admin.</span></span>|



