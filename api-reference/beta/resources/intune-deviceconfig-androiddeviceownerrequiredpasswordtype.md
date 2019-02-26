---
title: тип перечисления Андроиддевицеовнеррекуиредпассвордтипе
description: Обязательный тип пароля для политики владельца устройств Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79d71fbabc4597c87c9cee782904334e2f12d7e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172592"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="e6ff4-103">тип перечисления Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="e6ff4-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="e6ff4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6ff4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6ff4-106">Обязательный тип пароля для политики владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e6ff4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e6ff4-107">Members</span></span>
|<span data-ttu-id="e6ff4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e6ff4-108">Member</span></span>|<span data-ttu-id="e6ff4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ff4-109">Value</span></span>|<span data-ttu-id="e6ff4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ff4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ff4-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="e6ff4-111">deviceDefault</span></span>|<span data-ttu-id="e6ff4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e6ff4-112">0</span></span>|<span data-ttu-id="e6ff4-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="e6ff4-114">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e6ff4-114">required</span></span>|<span data-ttu-id="e6ff4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e6ff4-115">1</span></span>|<span data-ttu-id="e6ff4-116">Должен быть задан пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="e6ff4-117">числовых</span><span class="sxs-lookup"><span data-stu-id="e6ff4-117">numeric</span></span>|<span data-ttu-id="e6ff4-118">2</span><span class="sxs-lookup"><span data-stu-id="e6ff4-118">2</span></span>|<span data-ttu-id="e6ff4-119">По крайней мере число цифр.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-119">At least numeric.</span></span>|
|<span data-ttu-id="e6ff4-120">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="e6ff4-120">numericComplex</span></span>|<span data-ttu-id="e6ff4-121">4</span><span class="sxs-lookup"><span data-stu-id="e6ff4-121">3</span></span>|<span data-ttu-id="e6ff4-122">По крайней мере цифры без повторяющихся или упорядоченных последовательностей.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="e6ff4-123">буквы</span><span class="sxs-lookup"><span data-stu-id="e6ff4-123">alphabetic</span></span>|<span data-ttu-id="e6ff4-124">4</span><span class="sxs-lookup"><span data-stu-id="e6ff4-124">4</span></span>|<span data-ttu-id="e6ff4-125">По крайней мере буквенно — пароль.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="e6ff4-126">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="e6ff4-126">alphanumeric</span></span>|<span data-ttu-id="e6ff4-127">17:00</span><span class="sxs-lookup"><span data-stu-id="e6ff4-127">5</span></span>|<span data-ttu-id="e6ff4-128">По крайней мере буквенно-цифровые пароли</span><span class="sxs-lookup"><span data-stu-id="e6ff4-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="e6ff4-129">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="e6ff4-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="e6ff4-130">6</span><span class="sxs-lookup"><span data-stu-id="e6ff4-130">6</span></span>|<span data-ttu-id="e6ff4-131">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="e6ff4-131">At least alphanumeric with symbols.</span></span>|




