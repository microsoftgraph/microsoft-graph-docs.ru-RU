---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6f37ddeb108db777b23f55abd67963688b9a3d3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402806"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="57a2b-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="57a2b-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="57a2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57a2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57a2b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57a2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57a2b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57a2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57a2b-107">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="57a2b-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="57a2b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="57a2b-108">Members</span></span>
|<span data-ttu-id="57a2b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="57a2b-109">Member</span></span>|<span data-ttu-id="57a2b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="57a2b-110">Value</span></span>|<span data-ttu-id="57a2b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="57a2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57a2b-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="57a2b-112">deviceDefault</span></span>|<span data-ttu-id="57a2b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="57a2b-113">0</span></span>|<span data-ttu-id="57a2b-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="57a2b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="57a2b-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="57a2b-115">required</span></span>|<span data-ttu-id="57a2b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="57a2b-116">1</span></span>|<span data-ttu-id="57a2b-117">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="57a2b-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="57a2b-118">числовых</span><span class="sxs-lookup"><span data-stu-id="57a2b-118">numeric</span></span>|<span data-ttu-id="57a2b-119">2</span><span class="sxs-lookup"><span data-stu-id="57a2b-119">2</span></span>|<span data-ttu-id="57a2b-120">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="57a2b-120">At least numeric.</span></span>|
|<span data-ttu-id="57a2b-121">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="57a2b-121">numericComplex</span></span>|<span data-ttu-id="57a2b-122">4</span><span class="sxs-lookup"><span data-stu-id="57a2b-122">3</span></span>|<span data-ttu-id="57a2b-123">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="57a2b-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="57a2b-124">буквы</span><span class="sxs-lookup"><span data-stu-id="57a2b-124">alphabetic</span></span>|<span data-ttu-id="57a2b-125">4 </span><span class="sxs-lookup"><span data-stu-id="57a2b-125">4</span></span>|<span data-ttu-id="57a2b-126">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="57a2b-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="57a2b-127">цифрового</span><span class="sxs-lookup"><span data-stu-id="57a2b-127">alphanumeric</span></span>|<span data-ttu-id="57a2b-128">5 </span><span class="sxs-lookup"><span data-stu-id="57a2b-128">5</span></span>|<span data-ttu-id="57a2b-129">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="57a2b-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="57a2b-130">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="57a2b-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="57a2b-131">6 </span><span class="sxs-lookup"><span data-stu-id="57a2b-131">6</span></span>|<span data-ttu-id="57a2b-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="57a2b-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="57a2b-133">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="57a2b-133">lowSecurityBiometric</span></span>|<span data-ttu-id="57a2b-134">7 </span><span class="sxs-lookup"><span data-stu-id="57a2b-134">7</span></span>|<span data-ttu-id="57a2b-135">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="57a2b-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="57a2b-136">кустомпассворд</span><span class="sxs-lookup"><span data-stu-id="57a2b-136">customPassword</span></span>|<span data-ttu-id="57a2b-137">8 </span><span class="sxs-lookup"><span data-stu-id="57a2b-137">8</span></span>|<span data-ttu-id="57a2b-138">Настраиваемый пароль, заданный администратором.</span><span class="sxs-lookup"><span data-stu-id="57a2b-138">Custom password set by the admin.</span></span>|



