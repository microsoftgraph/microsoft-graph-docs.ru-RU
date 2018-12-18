---
title: Тип перечисления androidDeviceOwnerRequiredPasswordType
description: Android политики устройства владельцем требуется тип пароль.
author: tfitzmac
ms.openlocfilehash: e0903bbf5720350b35bf7e5fe5c9a5f9584810c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330228"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="c033c-103">Тип перечисления androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c033c-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c033c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c033c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c033c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c033c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c033c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c033c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c033c-107">Android политики устройства владельцем требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="c033c-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="c033c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c033c-108">Members</span></span>
|<span data-ttu-id="c033c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c033c-109">Member</span></span>|<span data-ttu-id="c033c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c033c-110">Value</span></span>|<span data-ttu-id="c033c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c033c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c033c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c033c-112">deviceDefault</span></span>|<span data-ttu-id="c033c-113">0</span><span class="sxs-lookup"><span data-stu-id="c033c-113">0</span></span>|<span data-ttu-id="c033c-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="c033c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c033c-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c033c-115">required</span></span>|<span data-ttu-id="c033c-116">1</span><span class="sxs-lookup"><span data-stu-id="c033c-116">1</span></span>|<span data-ttu-id="c033c-117">Необходимо задать пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="c033c-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="c033c-118">числовое</span><span class="sxs-lookup"><span data-stu-id="c033c-118">numeric</span></span>|<span data-ttu-id="c033c-119">2</span><span class="sxs-lookup"><span data-stu-id="c033c-119">2</span></span>|<span data-ttu-id="c033c-120">AT бы числовое.</span><span class="sxs-lookup"><span data-stu-id="c033c-120">At least numeric.</span></span>|
|<span data-ttu-id="c033c-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c033c-121">numericComplex</span></span>|<span data-ttu-id="c033c-122">3</span><span class="sxs-lookup"><span data-stu-id="c033c-122">3</span></span>|<span data-ttu-id="c033c-123">AT бы числовое с последовательности не повторяющиеся или упорядоченном.</span><span class="sxs-lookup"><span data-stu-id="c033c-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="c033c-124">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="c033c-124">alphabetic</span></span>|<span data-ttu-id="c033c-125">4</span><span class="sxs-lookup"><span data-stu-id="c033c-125">4</span></span>|<span data-ttu-id="c033c-126">По крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="c033c-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="c033c-127">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="c033c-127">alphanumeric</span></span>|<span data-ttu-id="c033c-128">5</span><span class="sxs-lookup"><span data-stu-id="c033c-128">5</span></span>|<span data-ttu-id="c033c-129">По крайней мере буквенно-цифровой пароль</span><span class="sxs-lookup"><span data-stu-id="c033c-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="c033c-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c033c-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="c033c-131">6</span><span class="sxs-lookup"><span data-stu-id="c033c-131">6</span></span>|<span data-ttu-id="c033c-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="c033c-132">At least alphanumeric with symbols.</span></span>|





