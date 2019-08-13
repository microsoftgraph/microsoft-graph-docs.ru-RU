---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8bfe6184b2427584c54094636ef7c71f857ec1f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369404"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="814a8-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="814a8-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="814a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="814a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="814a8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="814a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="814a8-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="814a8-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="814a8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="814a8-107">Members</span></span>
|<span data-ttu-id="814a8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="814a8-108">Member</span></span>|<span data-ttu-id="814a8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="814a8-109">Value</span></span>|<span data-ttu-id="814a8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="814a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="814a8-111">окно</span><span class="sxs-lookup"><span data-stu-id="814a8-111">open</span></span>|<span data-ttu-id="814a8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="814a8-112">0</span></span>|<span data-ttu-id="814a8-113">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="814a8-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="814a8-114">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="814a8-114">wpaPersonal</span></span>|<span data-ttu-id="814a8-115">1,1</span><span class="sxs-lookup"><span data-stu-id="814a8-115">1</span></span>|<span data-ttu-id="814a8-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="814a8-116">WPA-Personal.</span></span>|
|<span data-ttu-id="814a8-117">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="814a8-117">wpaEnterprise</span></span>|<span data-ttu-id="814a8-118">2</span><span class="sxs-lookup"><span data-stu-id="814a8-118">2</span></span>|<span data-ttu-id="814a8-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="814a8-119">WPA-Enterprise.</span></span> <span data-ttu-id="814a8-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="814a8-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="814a8-121">WEP</span><span class="sxs-lookup"><span data-stu-id="814a8-121">wep</span></span>|<span data-ttu-id="814a8-122">4</span><span class="sxs-lookup"><span data-stu-id="814a8-122">3</span></span>|<span data-ttu-id="814a8-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="814a8-123">WEP Encryption.</span></span>|
|<span data-ttu-id="814a8-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="814a8-124">wpa2Personal</span></span>|<span data-ttu-id="814a8-125">SP4</span><span class="sxs-lookup"><span data-stu-id="814a8-125">4</span></span>|<span data-ttu-id="814a8-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="814a8-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="814a8-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="814a8-127">wpa2Enterprise</span></span>|<span data-ttu-id="814a8-128">17:00</span><span class="sxs-lookup"><span data-stu-id="814a8-128">5</span></span>|<span data-ttu-id="814a8-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="814a8-129">WPA2-Enterprise.</span></span> <span data-ttu-id="814a8-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="814a8-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



