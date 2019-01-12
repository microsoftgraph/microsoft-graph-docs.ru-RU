---
title: Тип перечисления androidDeviceOwnerRequiredPasswordType
description: Android политики устройства владельцем требуется тип пароль.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1208de597baff9dd05a48663435a3a928f3dae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938043"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="f33b3-103">Тип перечисления androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f33b3-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f33b3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f33b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f33b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f33b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f33b3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f33b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f33b3-107">Android политики устройства владельцем требуется тип пароль.</span><span class="sxs-lookup"><span data-stu-id="f33b3-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="f33b3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f33b3-108">Members</span></span>
|<span data-ttu-id="f33b3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f33b3-109">Member</span></span>|<span data-ttu-id="f33b3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f33b3-110">Value</span></span>|<span data-ttu-id="f33b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f33b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f33b3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f33b3-112">deviceDefault</span></span>|<span data-ttu-id="f33b3-113">0</span><span class="sxs-lookup"><span data-stu-id="f33b3-113">0</span></span>|<span data-ttu-id="f33b3-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="f33b3-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f33b3-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f33b3-115">required</span></span>|<span data-ttu-id="f33b3-116">1</span><span class="sxs-lookup"><span data-stu-id="f33b3-116">1</span></span>|<span data-ttu-id="f33b3-117">Необходимо задать пароль, но не существует ограничений на тип.</span><span class="sxs-lookup"><span data-stu-id="f33b3-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="f33b3-118">числовое</span><span class="sxs-lookup"><span data-stu-id="f33b3-118">numeric</span></span>|<span data-ttu-id="f33b3-119">2</span><span class="sxs-lookup"><span data-stu-id="f33b3-119">2</span></span>|<span data-ttu-id="f33b3-120">AT бы числовое.</span><span class="sxs-lookup"><span data-stu-id="f33b3-120">At least numeric.</span></span>|
|<span data-ttu-id="f33b3-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f33b3-121">numericComplex</span></span>|<span data-ttu-id="f33b3-122">3</span><span class="sxs-lookup"><span data-stu-id="f33b3-122">3</span></span>|<span data-ttu-id="f33b3-123">AT бы числовое с последовательности не повторяющиеся или упорядоченном.</span><span class="sxs-lookup"><span data-stu-id="f33b3-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="f33b3-124">к буквам и цифрам</span><span class="sxs-lookup"><span data-stu-id="f33b3-124">alphabetic</span></span>|<span data-ttu-id="f33b3-125">4</span><span class="sxs-lookup"><span data-stu-id="f33b3-125">4</span></span>|<span data-ttu-id="f33b3-126">По крайней мере к буквам и цифрам пароль.</span><span class="sxs-lookup"><span data-stu-id="f33b3-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="f33b3-127">буквенно-цифровые;</span><span class="sxs-lookup"><span data-stu-id="f33b3-127">alphanumeric</span></span>|<span data-ttu-id="f33b3-128">5</span><span class="sxs-lookup"><span data-stu-id="f33b3-128">5</span></span>|<span data-ttu-id="f33b3-129">По крайней мере буквенно-цифровой пароль</span><span class="sxs-lookup"><span data-stu-id="f33b3-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="f33b3-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f33b3-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="f33b3-131">6</span><span class="sxs-lookup"><span data-stu-id="f33b3-131">6</span></span>|<span data-ttu-id="f33b3-132">По крайней мере буквенно-цифровые символы.</span><span class="sxs-lookup"><span data-stu-id="f33b3-132">At least alphanumeric with symbols.</span></span>|





