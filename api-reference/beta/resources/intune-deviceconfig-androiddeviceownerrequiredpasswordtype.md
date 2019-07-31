---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 043b2122a346a8540dfd99e4900fc0e59dd22041
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971494"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="d8a05-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="d8a05-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d8a05-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8a05-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8a05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8a05-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="d8a05-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d8a05-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8a05-107">Members</span></span>
|<span data-ttu-id="d8a05-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8a05-108">Member</span></span>|<span data-ttu-id="d8a05-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d8a05-109">Value</span></span>|<span data-ttu-id="d8a05-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a05-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8a05-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="d8a05-111">deviceDefault</span></span>|<span data-ttu-id="d8a05-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d8a05-112">0</span></span>|<span data-ttu-id="d8a05-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="d8a05-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d8a05-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d8a05-114">required</span></span>|<span data-ttu-id="d8a05-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d8a05-115">1</span></span>|<span data-ttu-id="d8a05-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="d8a05-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="d8a05-117">числовых</span><span class="sxs-lookup"><span data-stu-id="d8a05-117">numeric</span></span>|<span data-ttu-id="d8a05-118">2</span><span class="sxs-lookup"><span data-stu-id="d8a05-118">2</span></span>|<span data-ttu-id="d8a05-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="d8a05-119">At least numeric.</span></span>|
|<span data-ttu-id="d8a05-120">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="d8a05-120">numericComplex</span></span>|<span data-ttu-id="d8a05-121">4</span><span class="sxs-lookup"><span data-stu-id="d8a05-121">3</span></span>|<span data-ttu-id="d8a05-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="d8a05-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="d8a05-123">буквы</span><span class="sxs-lookup"><span data-stu-id="d8a05-123">alphabetic</span></span>|<span data-ttu-id="d8a05-124">SP4</span><span class="sxs-lookup"><span data-stu-id="d8a05-124">4</span></span>|<span data-ttu-id="d8a05-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="d8a05-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="d8a05-126">цифрового</span><span class="sxs-lookup"><span data-stu-id="d8a05-126">alphanumeric</span></span>|<span data-ttu-id="d8a05-127">17:00</span><span class="sxs-lookup"><span data-stu-id="d8a05-127">5</span></span>|<span data-ttu-id="d8a05-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="d8a05-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="d8a05-129">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="d8a05-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="d8a05-130">6 </span><span class="sxs-lookup"><span data-stu-id="d8a05-130">6</span></span>|<span data-ttu-id="d8a05-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="d8a05-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="d8a05-132">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="d8a05-132">lowSecurityBiometric</span></span>|<span data-ttu-id="d8a05-133">7 </span><span class="sxs-lookup"><span data-stu-id="d8a05-133">7</span></span>|<span data-ttu-id="d8a05-134">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="d8a05-134">Low security biometrics based password required.</span></span>|





