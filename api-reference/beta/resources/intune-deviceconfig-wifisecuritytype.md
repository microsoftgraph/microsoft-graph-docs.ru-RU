---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2245069bfda8ced7c16d23465d510c98f1bc5eef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991536"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="94cf4-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="94cf4-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="94cf4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94cf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94cf4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94cf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94cf4-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="94cf4-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="94cf4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="94cf4-107">Members</span></span>
|<span data-ttu-id="94cf4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="94cf4-108">Member</span></span>|<span data-ttu-id="94cf4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="94cf4-109">Value</span></span>|<span data-ttu-id="94cf4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94cf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94cf4-111">окно</span><span class="sxs-lookup"><span data-stu-id="94cf4-111">open</span></span>|<span data-ttu-id="94cf4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="94cf4-112">0</span></span>|<span data-ttu-id="94cf4-113">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="94cf4-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="94cf4-114">Впаперсонал</span><span class="sxs-lookup"><span data-stu-id="94cf4-114">wpaPersonal</span></span>|<span data-ttu-id="94cf4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="94cf4-115">1</span></span>|<span data-ttu-id="94cf4-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="94cf4-116">WPA-Personal.</span></span>|
|<span data-ttu-id="94cf4-117">Впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="94cf4-117">wpaEnterprise</span></span>|<span data-ttu-id="94cf4-118">2</span><span class="sxs-lookup"><span data-stu-id="94cf4-118">2</span></span>|<span data-ttu-id="94cf4-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="94cf4-119">WPA-Enterprise.</span></span> <span data-ttu-id="94cf4-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="94cf4-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="94cf4-121">WEP</span><span class="sxs-lookup"><span data-stu-id="94cf4-121">wep</span></span>|<span data-ttu-id="94cf4-122">4</span><span class="sxs-lookup"><span data-stu-id="94cf4-122">3</span></span>|<span data-ttu-id="94cf4-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="94cf4-123">WEP Encryption.</span></span>|
|<span data-ttu-id="94cf4-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="94cf4-124">wpa2Personal</span></span>|<span data-ttu-id="94cf4-125">SP4</span><span class="sxs-lookup"><span data-stu-id="94cf4-125">4</span></span>|<span data-ttu-id="94cf4-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="94cf4-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="94cf4-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="94cf4-127">wpa2Enterprise</span></span>|<span data-ttu-id="94cf4-128">17:00</span><span class="sxs-lookup"><span data-stu-id="94cf4-128">5</span></span>|<span data-ttu-id="94cf4-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="94cf4-129">WPA2-Enterprise.</span></span> <span data-ttu-id="94cf4-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="94cf4-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





