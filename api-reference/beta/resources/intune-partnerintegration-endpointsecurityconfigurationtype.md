---
title: тип перечисления Ендпоинтсекуритиконфигуратионтипе
description: Тип политики безопасности конечной точки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ad174c7977f3cc61b40462f2e73b46a4fc298421
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301083"
---
# <a name="endpointsecurityconfigurationtype-enum-type"></a><span data-ttu-id="aeff7-103">тип перечисления Ендпоинтсекуритиконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="aeff7-103">endpointSecurityConfigurationType enum type</span></span>

<span data-ttu-id="aeff7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeff7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aeff7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeff7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aeff7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aeff7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeff7-107">Тип политики безопасности конечной точки.</span><span class="sxs-lookup"><span data-stu-id="aeff7-107">The endpoint security policy type.</span></span>

## <a name="members"></a><span data-ttu-id="aeff7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="aeff7-108">Members</span></span>
|<span data-ttu-id="aeff7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="aeff7-109">Member</span></span>|<span data-ttu-id="aeff7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="aeff7-110">Value</span></span>|<span data-ttu-id="aeff7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aeff7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeff7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="aeff7-112">unknown</span></span>|<span data-ttu-id="aeff7-113">нуль</span><span class="sxs-lookup"><span data-stu-id="aeff7-113">0</span></span>|<span data-ttu-id="aeff7-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="aeff7-114">Unknown.</span></span>|
|<span data-ttu-id="aeff7-115">такую</span><span class="sxs-lookup"><span data-stu-id="aeff7-115">antivirus</span></span>|<span data-ttu-id="aeff7-116">1,1</span><span class="sxs-lookup"><span data-stu-id="aeff7-116">1</span></span>|<span data-ttu-id="aeff7-117">Такую.</span><span class="sxs-lookup"><span data-stu-id="aeff7-117">Antivirus.</span></span>|
|<span data-ttu-id="aeff7-118">дискенкриптион</span><span class="sxs-lookup"><span data-stu-id="aeff7-118">diskEncryption</span></span>|<span data-ttu-id="aeff7-119">2</span><span class="sxs-lookup"><span data-stu-id="aeff7-119">2</span></span>|<span data-ttu-id="aeff7-120">Шифрование дисков.</span><span class="sxs-lookup"><span data-stu-id="aeff7-120">Disk encryption.</span></span>|
|<span data-ttu-id="aeff7-121">брандмауэра</span><span class="sxs-lookup"><span data-stu-id="aeff7-121">firewall</span></span>|<span data-ttu-id="aeff7-122">4</span><span class="sxs-lookup"><span data-stu-id="aeff7-122">3</span></span>|<span data-ttu-id="aeff7-123">Брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="aeff7-123">Firewall.</span></span>|
|<span data-ttu-id="aeff7-124">ендпоинтдетектионандреспонсе</span><span class="sxs-lookup"><span data-stu-id="aeff7-124">endpointDetectionAndResponse</span></span>|<span data-ttu-id="aeff7-125">4 </span><span class="sxs-lookup"><span data-stu-id="aeff7-125">4</span></span>|<span data-ttu-id="aeff7-126">Выявление конечных точек и реагирование на них.</span><span class="sxs-lookup"><span data-stu-id="aeff7-126">Endpoint detection and response.</span></span>|
|<span data-ttu-id="aeff7-127">аттакксурфацередуктион</span><span class="sxs-lookup"><span data-stu-id="aeff7-127">attackSurfaceReduction</span></span>|<span data-ttu-id="aeff7-128">5 </span><span class="sxs-lookup"><span data-stu-id="aeff7-128">5</span></span>|<span data-ttu-id="aeff7-129">Сокращение направлений атак.</span><span class="sxs-lookup"><span data-stu-id="aeff7-129">Attack surface reduction.</span></span>|
|<span data-ttu-id="aeff7-130">аккаунтпротектион</span><span class="sxs-lookup"><span data-stu-id="aeff7-130">accountProtection</span></span>|<span data-ttu-id="aeff7-131">6 </span><span class="sxs-lookup"><span data-stu-id="aeff7-131">6</span></span>|<span data-ttu-id="aeff7-132">Защита учетной записи.</span><span class="sxs-lookup"><span data-stu-id="aeff7-132">Account protection.</span></span>|




