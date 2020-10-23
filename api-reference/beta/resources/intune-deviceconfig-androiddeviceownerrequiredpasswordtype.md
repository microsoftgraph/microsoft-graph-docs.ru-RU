---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09714a743c441058f0a87ff9d26b864a28022b96
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707838"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="1a536-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1a536-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="1a536-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a536-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a536-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a536-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a536-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a536-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a536-107">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="1a536-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="1a536-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1a536-108">Members</span></span>
|<span data-ttu-id="1a536-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1a536-109">Member</span></span>|<span data-ttu-id="1a536-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1a536-110">Value</span></span>|<span data-ttu-id="1a536-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a536-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a536-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="1a536-112">deviceDefault</span></span>|<span data-ttu-id="1a536-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1a536-113">0</span></span>|<span data-ttu-id="1a536-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="1a536-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="1a536-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="1a536-115">required</span></span>|<span data-ttu-id="1a536-116">1,1</span><span class="sxs-lookup"><span data-stu-id="1a536-116">1</span></span>|<span data-ttu-id="1a536-117">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="1a536-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="1a536-118">числовых</span><span class="sxs-lookup"><span data-stu-id="1a536-118">numeric</span></span>|<span data-ttu-id="1a536-119">2</span><span class="sxs-lookup"><span data-stu-id="1a536-119">2</span></span>|<span data-ttu-id="1a536-120">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="1a536-120">At least numeric.</span></span>|
|<span data-ttu-id="1a536-121">нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="1a536-121">numericComplex</span></span>|<span data-ttu-id="1a536-122">4</span><span class="sxs-lookup"><span data-stu-id="1a536-122">3</span></span>|<span data-ttu-id="1a536-123">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="1a536-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="1a536-124">буквы</span><span class="sxs-lookup"><span data-stu-id="1a536-124">alphabetic</span></span>|<span data-ttu-id="1a536-125">4 </span><span class="sxs-lookup"><span data-stu-id="1a536-125">4</span></span>|<span data-ttu-id="1a536-126">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="1a536-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="1a536-127">цифрового</span><span class="sxs-lookup"><span data-stu-id="1a536-127">alphanumeric</span></span>|<span data-ttu-id="1a536-128">5 </span><span class="sxs-lookup"><span data-stu-id="1a536-128">5</span></span>|<span data-ttu-id="1a536-129">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="1a536-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="1a536-130">алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="1a536-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="1a536-131">6 </span><span class="sxs-lookup"><span data-stu-id="1a536-131">6</span></span>|<span data-ttu-id="1a536-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="1a536-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="1a536-133">ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="1a536-133">lowSecurityBiometric</span></span>|<span data-ttu-id="1a536-134">7 </span><span class="sxs-lookup"><span data-stu-id="1a536-134">7</span></span>|<span data-ttu-id="1a536-135">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="1a536-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="1a536-136">кустомпассворд</span><span class="sxs-lookup"><span data-stu-id="1a536-136">customPassword</span></span>|<span data-ttu-id="1a536-137">8 </span><span class="sxs-lookup"><span data-stu-id="1a536-137">8</span></span>|<span data-ttu-id="1a536-138">Настраиваемый пароль, заданный администратором.</span><span class="sxs-lookup"><span data-stu-id="1a536-138">Custom password set by the admin.</span></span>|





