---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 33e0e615a62f62a565196ba3a6c9c814695040e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000538"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="ba1ef-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ba1ef-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="ba1ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1ef-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="ba1ef-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ba1ef-107">Members</span></span>
|<span data-ttu-id="ba1ef-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ba1ef-108">Member</span></span>|<span data-ttu-id="ba1ef-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ba1ef-109">Value</span></span>|<span data-ttu-id="ba1ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba1ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba1ef-111">окно</span><span class="sxs-lookup"><span data-stu-id="ba1ef-111">open</span></span>|<span data-ttu-id="ba1ef-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ba1ef-112">0</span></span>|<span data-ttu-id="ba1ef-113">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="ba1ef-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="ba1ef-114">Впаперсонал</span><span class="sxs-lookup"><span data-stu-id="ba1ef-114">wpaPersonal</span></span>|<span data-ttu-id="ba1ef-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ba1ef-115">1</span></span>|<span data-ttu-id="ba1ef-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-116">WPA-Personal.</span></span>|
|<span data-ttu-id="ba1ef-117">Впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="ba1ef-117">wpaEnterprise</span></span>|<span data-ttu-id="ba1ef-118">2</span><span class="sxs-lookup"><span data-stu-id="ba1ef-118">2</span></span>|<span data-ttu-id="ba1ef-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-119">WPA-Enterprise.</span></span> <span data-ttu-id="ba1ef-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="ba1ef-121">WEP</span><span class="sxs-lookup"><span data-stu-id="ba1ef-121">wep</span></span>|<span data-ttu-id="ba1ef-122">4</span><span class="sxs-lookup"><span data-stu-id="ba1ef-122">3</span></span>|<span data-ttu-id="ba1ef-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-123">WEP Encryption.</span></span>|
|<span data-ttu-id="ba1ef-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="ba1ef-124">wpa2Personal</span></span>|<span data-ttu-id="ba1ef-125">SP4</span><span class="sxs-lookup"><span data-stu-id="ba1ef-125">4</span></span>|<span data-ttu-id="ba1ef-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="ba1ef-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="ba1ef-127">wpa2Enterprise</span></span>|<span data-ttu-id="ba1ef-128">17:00</span><span class="sxs-lookup"><span data-stu-id="ba1ef-128">5</span></span>|<span data-ttu-id="ba1ef-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-129">WPA2-Enterprise.</span></span> <span data-ttu-id="ba1ef-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="ba1ef-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





