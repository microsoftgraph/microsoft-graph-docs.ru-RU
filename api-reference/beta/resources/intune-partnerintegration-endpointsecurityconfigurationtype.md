---
title: тип перечисления Ендпоинтсекуритиконфигуратионтипе
description: Тип политики безопасности конечной точки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8eabd459e8816b38d1e908d0da9c0723dca5a16
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48718471"
---
# <a name="endpointsecurityconfigurationtype-enum-type"></a><span data-ttu-id="a21d3-103">тип перечисления Ендпоинтсекуритиконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="a21d3-103">endpointSecurityConfigurationType enum type</span></span>

<span data-ttu-id="a21d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a21d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a21d3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a21d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a21d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a21d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a21d3-107">Тип политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="a21d3-107">The endpoint security policy type.</span></span>

## <a name="members"></a><span data-ttu-id="a21d3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a21d3-108">Members</span></span>
|<span data-ttu-id="a21d3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a21d3-109">Member</span></span>|<span data-ttu-id="a21d3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a21d3-110">Value</span></span>|<span data-ttu-id="a21d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a21d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a21d3-112">unknown</span><span class="sxs-lookup"><span data-stu-id="a21d3-112">unknown</span></span>|<span data-ttu-id="a21d3-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a21d3-113">0</span></span>|<span data-ttu-id="a21d3-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="a21d3-114">Unknown.</span></span>|
|<span data-ttu-id="a21d3-115">такую</span><span class="sxs-lookup"><span data-stu-id="a21d3-115">antivirus</span></span>|<span data-ttu-id="a21d3-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a21d3-116">1</span></span>|<span data-ttu-id="a21d3-117">Такую.</span><span class="sxs-lookup"><span data-stu-id="a21d3-117">Antivirus.</span></span>|
|<span data-ttu-id="a21d3-118">дискенкриптион</span><span class="sxs-lookup"><span data-stu-id="a21d3-118">diskEncryption</span></span>|<span data-ttu-id="a21d3-119">2</span><span class="sxs-lookup"><span data-stu-id="a21d3-119">2</span></span>|<span data-ttu-id="a21d3-120">Шифрование дисков.</span><span class="sxs-lookup"><span data-stu-id="a21d3-120">Disk encryption.</span></span>|
|<span data-ttu-id="a21d3-121">брандмауэра</span><span class="sxs-lookup"><span data-stu-id="a21d3-121">firewall</span></span>|<span data-ttu-id="a21d3-122">4</span><span class="sxs-lookup"><span data-stu-id="a21d3-122">3</span></span>|<span data-ttu-id="a21d3-123">Брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="a21d3-123">Firewall.</span></span>|
|<span data-ttu-id="a21d3-124">ендпоинтдетектионандреспонсе</span><span class="sxs-lookup"><span data-stu-id="a21d3-124">endpointDetectionAndResponse</span></span>|<span data-ttu-id="a21d3-125">4 </span><span class="sxs-lookup"><span data-stu-id="a21d3-125">4</span></span>|<span data-ttu-id="a21d3-126">Выявление конечных точек и реагирование на них.</span><span class="sxs-lookup"><span data-stu-id="a21d3-126">Endpoint detection and response.</span></span>|
|<span data-ttu-id="a21d3-127">аттакксурфацередуктион</span><span class="sxs-lookup"><span data-stu-id="a21d3-127">attackSurfaceReduction</span></span>|<span data-ttu-id="a21d3-128">5 </span><span class="sxs-lookup"><span data-stu-id="a21d3-128">5</span></span>|<span data-ttu-id="a21d3-129">Сокращение направлений атак.</span><span class="sxs-lookup"><span data-stu-id="a21d3-129">Attack surface reduction.</span></span>|
|<span data-ttu-id="a21d3-130">аккаунтпротектион</span><span class="sxs-lookup"><span data-stu-id="a21d3-130">accountProtection</span></span>|<span data-ttu-id="a21d3-131">6 </span><span class="sxs-lookup"><span data-stu-id="a21d3-131">6</span></span>|<span data-ttu-id="a21d3-132">Защита учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a21d3-132">Account protection.</span></span>|





