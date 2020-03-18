---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c770ce8d3e00a8d7997b2b72fcd18eb9007ba83
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787238"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="62199-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="62199-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="62199-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62199-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62199-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62199-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62199-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="62199-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="62199-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="62199-107">Members</span></span>
|<span data-ttu-id="62199-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="62199-108">Member</span></span>|<span data-ttu-id="62199-109">Значение</span><span class="sxs-lookup"><span data-stu-id="62199-109">Value</span></span>|<span data-ttu-id="62199-110">Описание</span><span class="sxs-lookup"><span data-stu-id="62199-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62199-111">окно</span><span class="sxs-lookup"><span data-stu-id="62199-111">open</span></span>|<span data-ttu-id="62199-112">нуль</span><span class="sxs-lookup"><span data-stu-id="62199-112">0</span></span>|<span data-ttu-id="62199-113">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="62199-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="62199-114">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="62199-114">wpaPersonal</span></span>|<span data-ttu-id="62199-115">1,1</span><span class="sxs-lookup"><span data-stu-id="62199-115">1</span></span>|<span data-ttu-id="62199-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="62199-116">WPA-Personal.</span></span>|
|<span data-ttu-id="62199-117">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="62199-117">wpaEnterprise</span></span>|<span data-ttu-id="62199-118">2</span><span class="sxs-lookup"><span data-stu-id="62199-118">2</span></span>|<span data-ttu-id="62199-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="62199-119">WPA-Enterprise.</span></span> <span data-ttu-id="62199-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="62199-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="62199-121">WEP</span><span class="sxs-lookup"><span data-stu-id="62199-121">wep</span></span>|<span data-ttu-id="62199-122">4</span><span class="sxs-lookup"><span data-stu-id="62199-122">3</span></span>|<span data-ttu-id="62199-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="62199-123">WEP Encryption.</span></span>|
|<span data-ttu-id="62199-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="62199-124">wpa2Personal</span></span>|<span data-ttu-id="62199-125">4 </span><span class="sxs-lookup"><span data-stu-id="62199-125">4</span></span>|<span data-ttu-id="62199-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="62199-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="62199-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="62199-127">wpa2Enterprise</span></span>|<span data-ttu-id="62199-128">5 </span><span class="sxs-lookup"><span data-stu-id="62199-128">5</span></span>|<span data-ttu-id="62199-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="62199-129">WPA2-Enterprise.</span></span> <span data-ttu-id="62199-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="62199-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



