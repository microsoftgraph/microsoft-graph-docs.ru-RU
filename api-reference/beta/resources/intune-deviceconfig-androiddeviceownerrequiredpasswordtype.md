---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c575b1b39592eb8191e358563abb6d6bd834e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556381"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="37f2e-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="37f2e-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="37f2e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37f2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37f2e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37f2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37f2e-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="37f2e-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="37f2e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="37f2e-107">Members</span></span>
|<span data-ttu-id="37f2e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="37f2e-108">Member</span></span>|<span data-ttu-id="37f2e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="37f2e-109">Value</span></span>|<span data-ttu-id="37f2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="37f2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f2e-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="37f2e-111">deviceDefault</span></span>|<span data-ttu-id="37f2e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="37f2e-112">0</span></span>|<span data-ttu-id="37f2e-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="37f2e-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="37f2e-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="37f2e-114">required</span></span>|<span data-ttu-id="37f2e-115">1 </span><span class="sxs-lookup"><span data-stu-id="37f2e-115">1</span></span>|<span data-ttu-id="37f2e-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="37f2e-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="37f2e-117">числовых</span><span class="sxs-lookup"><span data-stu-id="37f2e-117">numeric</span></span>|<span data-ttu-id="37f2e-118">2 </span><span class="sxs-lookup"><span data-stu-id="37f2e-118">2</span></span>|<span data-ttu-id="37f2e-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="37f2e-119">At least numeric.</span></span>|
|<span data-ttu-id="37f2e-120">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="37f2e-120">numericComplex</span></span>|<span data-ttu-id="37f2e-121">3 </span><span class="sxs-lookup"><span data-stu-id="37f2e-121">3</span></span>|<span data-ttu-id="37f2e-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="37f2e-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="37f2e-123">буквы</span><span class="sxs-lookup"><span data-stu-id="37f2e-123">alphabetic</span></span>|<span data-ttu-id="37f2e-124">4 </span><span class="sxs-lookup"><span data-stu-id="37f2e-124">4</span></span>|<span data-ttu-id="37f2e-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="37f2e-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="37f2e-126">цифрового</span><span class="sxs-lookup"><span data-stu-id="37f2e-126">alphanumeric</span></span>|<span data-ttu-id="37f2e-127">5 </span><span class="sxs-lookup"><span data-stu-id="37f2e-127">5</span></span>|<span data-ttu-id="37f2e-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="37f2e-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="37f2e-129">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="37f2e-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="37f2e-130">6 </span><span class="sxs-lookup"><span data-stu-id="37f2e-130">6</span></span>|<span data-ttu-id="37f2e-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="37f2e-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="37f2e-132">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="37f2e-132">lowSecurityBiometric</span></span>|<span data-ttu-id="37f2e-133">7 </span><span class="sxs-lookup"><span data-stu-id="37f2e-133">7</span></span>|<span data-ttu-id="37f2e-134">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="37f2e-134">Low security biometrics based password required.</span></span>|





