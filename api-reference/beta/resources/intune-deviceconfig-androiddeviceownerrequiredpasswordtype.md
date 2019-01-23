---
title: Тип перечисления androidDeviceOwnerRequiredPasswordType
description: Android политики устройства владельцем требуется тип пароль.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403541"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="a97f5-103">Тип перечисления androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a97f5-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a97f5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a97f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a97f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a97f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a97f5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a97f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a97f5-107">Android политики устройства владельцем требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="a97f5-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a97f5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a97f5-108">Members</span></span>
|<span data-ttu-id="a97f5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a97f5-109">Member</span></span>|<span data-ttu-id="a97f5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a97f5-110">Value</span></span>|<span data-ttu-id="a97f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a97f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a97f5-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a97f5-112">deviceDefault</span></span>|<span data-ttu-id="a97f5-113">0</span><span class="sxs-lookup"><span data-stu-id="a97f5-113">0</span></span>|<span data-ttu-id="a97f5-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="a97f5-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="a97f5-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a97f5-115">required</span></span>|<span data-ttu-id="a97f5-116">1</span><span class="sxs-lookup"><span data-stu-id="a97f5-116">1</span></span>|<span data-ttu-id="a97f5-117">Необходимо задать пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="a97f5-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="a97f5-118">числовое</span><span class="sxs-lookup"><span data-stu-id="a97f5-118">numeric</span></span>|<span data-ttu-id="a97f5-119">2</span><span class="sxs-lookup"><span data-stu-id="a97f5-119">2</span></span>|<span data-ttu-id="a97f5-120">AT бы числовое.</span><span class="sxs-lookup"><span data-stu-id="a97f5-120">At least numeric.</span></span>|
|<span data-ttu-id="a97f5-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a97f5-121">numericComplex</span></span>|<span data-ttu-id="a97f5-122">3</span><span class="sxs-lookup"><span data-stu-id="a97f5-122">3</span></span>|<span data-ttu-id="a97f5-123">AT бы числовое с последовательности не повторяющиеся или упорядоченном.</span><span class="sxs-lookup"><span data-stu-id="a97f5-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="a97f5-124">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="a97f5-124">alphabetic</span></span>|<span data-ttu-id="a97f5-125">4</span><span class="sxs-lookup"><span data-stu-id="a97f5-125">4</span></span>|<span data-ttu-id="a97f5-126">По крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="a97f5-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="a97f5-127">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="a97f5-127">alphanumeric</span></span>|<span data-ttu-id="a97f5-128">5</span><span class="sxs-lookup"><span data-stu-id="a97f5-128">5</span></span>|<span data-ttu-id="a97f5-129">По крайней мере буквенно-цифровой пароль</span><span class="sxs-lookup"><span data-stu-id="a97f5-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="a97f5-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a97f5-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="a97f5-131">6</span><span class="sxs-lookup"><span data-stu-id="a97f5-131">6</span></span>|<span data-ttu-id="a97f5-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="a97f5-132">At least alphanumeric with symbols.</span></span>|




