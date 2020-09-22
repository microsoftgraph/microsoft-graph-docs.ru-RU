---
title: тип перечисления Ендпоинтсекуритиконфигуратионтипе
description: Тип политики безопасности конечной точки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6f46b07f62591b33f34b8e847b406763a0047f15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993639"
---
# <a name="endpointsecurityconfigurationtype-enum-type"></a><span data-ttu-id="3168c-103">тип перечисления Ендпоинтсекуритиконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="3168c-103">endpointSecurityConfigurationType enum type</span></span>

<span data-ttu-id="3168c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3168c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3168c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3168c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3168c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3168c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3168c-107">Тип политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="3168c-107">The endpoint security policy type.</span></span>

## <a name="members"></a><span data-ttu-id="3168c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3168c-108">Members</span></span>
|<span data-ttu-id="3168c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3168c-109">Member</span></span>|<span data-ttu-id="3168c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3168c-110">Value</span></span>|<span data-ttu-id="3168c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3168c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3168c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3168c-112">unknown</span></span>|<span data-ttu-id="3168c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3168c-113">0</span></span>|<span data-ttu-id="3168c-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="3168c-114">Unknown.</span></span>|
|<span data-ttu-id="3168c-115">такую</span><span class="sxs-lookup"><span data-stu-id="3168c-115">antivirus</span></span>|<span data-ttu-id="3168c-116">1 </span><span class="sxs-lookup"><span data-stu-id="3168c-116">1</span></span>|<span data-ttu-id="3168c-117">Такую.</span><span class="sxs-lookup"><span data-stu-id="3168c-117">Antivirus.</span></span>|
|<span data-ttu-id="3168c-118">дискенкриптион</span><span class="sxs-lookup"><span data-stu-id="3168c-118">diskEncryption</span></span>|<span data-ttu-id="3168c-119">2 </span><span class="sxs-lookup"><span data-stu-id="3168c-119">2</span></span>|<span data-ttu-id="3168c-120">Шифрование дисков.</span><span class="sxs-lookup"><span data-stu-id="3168c-120">Disk encryption.</span></span>|
|<span data-ttu-id="3168c-121">брандмауэра</span><span class="sxs-lookup"><span data-stu-id="3168c-121">firewall</span></span>|<span data-ttu-id="3168c-122">4</span><span class="sxs-lookup"><span data-stu-id="3168c-122">3</span></span>|<span data-ttu-id="3168c-123">Брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="3168c-123">Firewall.</span></span>|
|<span data-ttu-id="3168c-124">ендпоинтдетектионандреспонсе</span><span class="sxs-lookup"><span data-stu-id="3168c-124">endpointDetectionAndResponse</span></span>|<span data-ttu-id="3168c-125">4 </span><span class="sxs-lookup"><span data-stu-id="3168c-125">4</span></span>|<span data-ttu-id="3168c-126">Выявление конечных точек и реагирование на них.</span><span class="sxs-lookup"><span data-stu-id="3168c-126">Endpoint detection and response.</span></span>|
|<span data-ttu-id="3168c-127">аттакксурфацередуктион</span><span class="sxs-lookup"><span data-stu-id="3168c-127">attackSurfaceReduction</span></span>|<span data-ttu-id="3168c-128">5 </span><span class="sxs-lookup"><span data-stu-id="3168c-128">5</span></span>|<span data-ttu-id="3168c-129">Сокращение направлений атак.</span><span class="sxs-lookup"><span data-stu-id="3168c-129">Attack surface reduction.</span></span>|
|<span data-ttu-id="3168c-130">аккаунтпротектион</span><span class="sxs-lookup"><span data-stu-id="3168c-130">accountProtection</span></span>|<span data-ttu-id="3168c-131">6 </span><span class="sxs-lookup"><span data-stu-id="3168c-131">6</span></span>|<span data-ttu-id="3168c-132">Защита учетной записи.</span><span class="sxs-lookup"><span data-stu-id="3168c-132">Account protection.</span></span>|






