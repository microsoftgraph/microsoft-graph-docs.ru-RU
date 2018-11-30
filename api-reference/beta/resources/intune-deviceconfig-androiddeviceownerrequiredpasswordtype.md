---
title: Тип перечисления androidDeviceOwnerRequiredPasswordType
description: Android политики устройства владельцем требуется тип пароль.
ms.openlocfilehash: 16f4bc59f2b4fa9f37989d1bc1978cdfacb2892c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079221"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="3d27b-103">Тип перечисления androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3d27b-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="3d27b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d27b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d27b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d27b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d27b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3d27b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d27b-107">Android политики устройства владельцем требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="3d27b-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="3d27b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3d27b-108">Members</span></span>
|<span data-ttu-id="3d27b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3d27b-109">Member</span></span>|<span data-ttu-id="3d27b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3d27b-110">Value</span></span>|<span data-ttu-id="3d27b-111">Description</span><span class="sxs-lookup"><span data-stu-id="3d27b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d27b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3d27b-112">deviceDefault</span></span>|<span data-ttu-id="3d27b-113">0</span><span class="sxs-lookup"><span data-stu-id="3d27b-113">0</span></span>|<span data-ttu-id="3d27b-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="3d27b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="3d27b-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="3d27b-115">required</span></span>|<span data-ttu-id="3d27b-116">1</span><span class="sxs-lookup"><span data-stu-id="3d27b-116">1</span></span>|<span data-ttu-id="3d27b-117">Необходимо задать пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="3d27b-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="3d27b-118">числовое</span><span class="sxs-lookup"><span data-stu-id="3d27b-118">numeric</span></span>|<span data-ttu-id="3d27b-119">2</span><span class="sxs-lookup"><span data-stu-id="3d27b-119">2</span></span>|<span data-ttu-id="3d27b-120">AT бы числовое.</span><span class="sxs-lookup"><span data-stu-id="3d27b-120">At least numeric.</span></span>|
|<span data-ttu-id="3d27b-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="3d27b-121">numericComplex</span></span>|<span data-ttu-id="3d27b-122">3</span><span class="sxs-lookup"><span data-stu-id="3d27b-122">3</span></span>|<span data-ttu-id="3d27b-123">AT бы числовое с последовательности не повторяющиеся или упорядоченном.</span><span class="sxs-lookup"><span data-stu-id="3d27b-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="3d27b-124">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="3d27b-124">alphabetic</span></span>|<span data-ttu-id="3d27b-125">4</span><span class="sxs-lookup"><span data-stu-id="3d27b-125">4</span></span>|<span data-ttu-id="3d27b-126">По крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="3d27b-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="3d27b-127">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="3d27b-127">alphanumeric</span></span>|<span data-ttu-id="3d27b-128">5</span><span class="sxs-lookup"><span data-stu-id="3d27b-128">5</span></span>|<span data-ttu-id="3d27b-129">По крайней мере буквенно-цифровой пароль</span><span class="sxs-lookup"><span data-stu-id="3d27b-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="3d27b-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="3d27b-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="3d27b-131">6</span><span class="sxs-lookup"><span data-stu-id="3d27b-131">6</span></span>|<span data-ttu-id="3d27b-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="3d27b-132">At least alphanumeric with symbols.</span></span>|





