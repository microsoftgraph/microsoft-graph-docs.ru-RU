---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85c317706bb953fdeef202e4df9ec114944a7630
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944441"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="de194-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="de194-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="de194-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de194-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de194-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de194-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de194-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="de194-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="de194-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="de194-107">Members</span></span>
|<span data-ttu-id="de194-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="de194-108">Member</span></span>|<span data-ttu-id="de194-109">Значение</span><span class="sxs-lookup"><span data-stu-id="de194-109">Value</span></span>|<span data-ttu-id="de194-110">Описание</span><span class="sxs-lookup"><span data-stu-id="de194-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de194-111">окно</span><span class="sxs-lookup"><span data-stu-id="de194-111">open</span></span>|<span data-ttu-id="de194-112">нуль</span><span class="sxs-lookup"><span data-stu-id="de194-112">0</span></span>|<span data-ttu-id="de194-113">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="de194-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="de194-114">Впаперсонал</span><span class="sxs-lookup"><span data-stu-id="de194-114">wpaPersonal</span></span>|<span data-ttu-id="de194-115">1,1</span><span class="sxs-lookup"><span data-stu-id="de194-115">1</span></span>|<span data-ttu-id="de194-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="de194-116">WPA-Personal.</span></span>|
|<span data-ttu-id="de194-117">Впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="de194-117">wpaEnterprise</span></span>|<span data-ttu-id="de194-118">2</span><span class="sxs-lookup"><span data-stu-id="de194-118">2</span></span>|<span data-ttu-id="de194-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="de194-119">WPA-Enterprise.</span></span> <span data-ttu-id="de194-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="de194-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="de194-121">WEP</span><span class="sxs-lookup"><span data-stu-id="de194-121">wep</span></span>|<span data-ttu-id="de194-122">4</span><span class="sxs-lookup"><span data-stu-id="de194-122">3</span></span>|<span data-ttu-id="de194-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="de194-123">WEP Encryption.</span></span>|
|<span data-ttu-id="de194-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="de194-124">wpa2Personal</span></span>|<span data-ttu-id="de194-125">SP4</span><span class="sxs-lookup"><span data-stu-id="de194-125">4</span></span>|<span data-ttu-id="de194-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="de194-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="de194-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="de194-127">wpa2Enterprise</span></span>|<span data-ttu-id="de194-128">17:00</span><span class="sxs-lookup"><span data-stu-id="de194-128">5</span></span>|<span data-ttu-id="de194-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="de194-129">WPA2-Enterprise.</span></span> <span data-ttu-id="de194-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="de194-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




