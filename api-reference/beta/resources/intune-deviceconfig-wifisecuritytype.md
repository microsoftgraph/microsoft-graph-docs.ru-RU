---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9144a5761691b0a50e40370b1f4d2d08967f2c28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554844"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="f1559-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f1559-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="f1559-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1559-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1559-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1559-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1559-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="f1559-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="f1559-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f1559-107">Members</span></span>
|<span data-ttu-id="f1559-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f1559-108">Member</span></span>|<span data-ttu-id="f1559-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f1559-109">Value</span></span>|<span data-ttu-id="f1559-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1559-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1559-111">окно</span><span class="sxs-lookup"><span data-stu-id="f1559-111">open</span></span>|<span data-ttu-id="f1559-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f1559-112">0</span></span>|<span data-ttu-id="f1559-113">Открыть (без проверки поДлинности).</span><span class="sxs-lookup"><span data-stu-id="f1559-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="f1559-114">Впаперсонал</span><span class="sxs-lookup"><span data-stu-id="f1559-114">wpaPersonal</span></span>|<span data-ttu-id="f1559-115">1 </span><span class="sxs-lookup"><span data-stu-id="f1559-115">1</span></span>|<span data-ttu-id="f1559-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="f1559-116">WPA-Personal.</span></span>|
|<span data-ttu-id="f1559-117">Впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="f1559-117">wpaEnterprise</span></span>|<span data-ttu-id="f1559-118">2 </span><span class="sxs-lookup"><span data-stu-id="f1559-118">2</span></span>|<span data-ttu-id="f1559-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="f1559-119">WPA-Enterprise.</span></span> <span data-ttu-id="f1559-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1559-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="f1559-121">WEP</span><span class="sxs-lookup"><span data-stu-id="f1559-121">wep</span></span>|<span data-ttu-id="f1559-122">3 </span><span class="sxs-lookup"><span data-stu-id="f1559-122">3</span></span>|<span data-ttu-id="f1559-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="f1559-123">WEP Encryption.</span></span>|
|<span data-ttu-id="f1559-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="f1559-124">wpa2Personal</span></span>|<span data-ttu-id="f1559-125">4 </span><span class="sxs-lookup"><span data-stu-id="f1559-125">4</span></span>|<span data-ttu-id="f1559-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="f1559-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="f1559-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="f1559-127">wpa2Enterprise</span></span>|<span data-ttu-id="f1559-128">5 </span><span class="sxs-lookup"><span data-stu-id="f1559-128">5</span></span>|<span data-ttu-id="f1559-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="f1559-129">WPA2-Enterprise.</span></span> <span data-ttu-id="f1559-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f1559-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





