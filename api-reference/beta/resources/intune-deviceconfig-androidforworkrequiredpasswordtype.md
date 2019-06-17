---
title: тип перечисления Андроидфорворкрекуиредпассвордтипе
description: Для работы Android необходим тип пароля.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab11ed4951fb61e96afc55381986e83fad7ce440
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991060"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="6ddab-103">тип перечисления Андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6ddab-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="6ddab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ddab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ddab-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ddab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ddab-106">Для работы Android необходим тип пароля.</span><span class="sxs-lookup"><span data-stu-id="6ddab-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="6ddab-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6ddab-107">Members</span></span>
|<span data-ttu-id="6ddab-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6ddab-108">Member</span></span>|<span data-ttu-id="6ddab-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6ddab-109">Value</span></span>|<span data-ttu-id="6ddab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ddab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ddab-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="6ddab-111">deviceDefault</span></span>|<span data-ttu-id="6ddab-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6ddab-112">0</span></span>|<span data-ttu-id="6ddab-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="6ddab-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="6ddab-114">Ловсекуритибиометрик</span><span class="sxs-lookup"><span data-stu-id="6ddab-114">lowSecurityBiometric</span></span>|<span data-ttu-id="6ddab-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6ddab-115">1</span></span>|<span data-ttu-id="6ddab-116">Необходим пароль на основе биометрического уровня безопасности.</span><span class="sxs-lookup"><span data-stu-id="6ddab-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="6ddab-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="6ddab-117">required</span></span>|<span data-ttu-id="6ddab-118">2</span><span class="sxs-lookup"><span data-stu-id="6ddab-118">2</span></span>|<span data-ttu-id="6ddab-119">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6ddab-119">Required.</span></span>|
|<span data-ttu-id="6ddab-120">Атлеастнумерик</span><span class="sxs-lookup"><span data-stu-id="6ddab-120">atLeastNumeric</span></span>|<span data-ttu-id="6ddab-121">4</span><span class="sxs-lookup"><span data-stu-id="6ddab-121">3</span></span>|<span data-ttu-id="6ddab-122">Необходим по крайней мере числовой пароль.</span><span class="sxs-lookup"><span data-stu-id="6ddab-122">At least numeric password required.</span></span>|
|<span data-ttu-id="6ddab-123">Нумериккомплекс</span><span class="sxs-lookup"><span data-stu-id="6ddab-123">numericComplex</span></span>|<span data-ttu-id="6ddab-124">SP4</span><span class="sxs-lookup"><span data-stu-id="6ddab-124">4</span></span>|<span data-ttu-id="6ddab-125">Необходим числовой сложный пароль.</span><span class="sxs-lookup"><span data-stu-id="6ddab-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="6ddab-126">Атлеасталфабетик</span><span class="sxs-lookup"><span data-stu-id="6ddab-126">atLeastAlphabetic</span></span>|<span data-ttu-id="6ddab-127">17:00</span><span class="sxs-lookup"><span data-stu-id="6ddab-127">5</span></span>|<span data-ttu-id="6ddab-128">По крайней мере необходимо указать по крайней мере буквенный пароль.</span><span class="sxs-lookup"><span data-stu-id="6ddab-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="6ddab-129">Атлеасталфанумерик</span><span class="sxs-lookup"><span data-stu-id="6ddab-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="6ddab-130">6 </span><span class="sxs-lookup"><span data-stu-id="6ddab-130">6</span></span>|<span data-ttu-id="6ddab-131">Необходимо указать по крайней мере буквенно-цифровые пароли.</span><span class="sxs-lookup"><span data-stu-id="6ddab-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="6ddab-132">Алфанумериквиссимболс</span><span class="sxs-lookup"><span data-stu-id="6ddab-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="6ddab-133">7 </span><span class="sxs-lookup"><span data-stu-id="6ddab-133">7</span></span>|<span data-ttu-id="6ddab-134">По крайней мере буквенно-цифровые символы и пароль не требуются.</span><span class="sxs-lookup"><span data-stu-id="6ddab-134">At least alphanumeric with symbols password required.</span></span>|





