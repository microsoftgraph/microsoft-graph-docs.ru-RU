---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24fb0361bfbf8bc12c62f232d08c54eca033b915
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466325"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="4d821-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="4d821-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="4d821-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d821-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d821-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d821-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d821-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d821-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d821-107">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="4d821-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="4d821-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4d821-108">Members</span></span>
|<span data-ttu-id="4d821-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4d821-109">Member</span></span>|<span data-ttu-id="4d821-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4d821-110">Value</span></span>|<span data-ttu-id="4d821-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4d821-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d821-112">окно</span><span class="sxs-lookup"><span data-stu-id="4d821-112">open</span></span>|<span data-ttu-id="4d821-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4d821-113">0</span></span>|<span data-ttu-id="4d821-114">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="4d821-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="4d821-115">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="4d821-115">wpaPersonal</span></span>|<span data-ttu-id="4d821-116">1,1</span><span class="sxs-lookup"><span data-stu-id="4d821-116">1</span></span>|<span data-ttu-id="4d821-117">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="4d821-117">WPA-Personal.</span></span>|
|<span data-ttu-id="4d821-118">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="4d821-118">wpaEnterprise</span></span>|<span data-ttu-id="4d821-119">2</span><span class="sxs-lookup"><span data-stu-id="4d821-119">2</span></span>|<span data-ttu-id="4d821-120">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="4d821-120">WPA-Enterprise.</span></span> <span data-ttu-id="4d821-121">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4d821-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="4d821-122">WEP</span><span class="sxs-lookup"><span data-stu-id="4d821-122">wep</span></span>|<span data-ttu-id="4d821-123">4</span><span class="sxs-lookup"><span data-stu-id="4d821-123">3</span></span>|<span data-ttu-id="4d821-124">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="4d821-124">WEP Encryption.</span></span>|
|<span data-ttu-id="4d821-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="4d821-125">wpa2Personal</span></span>|<span data-ttu-id="4d821-126">4 </span><span class="sxs-lookup"><span data-stu-id="4d821-126">4</span></span>|<span data-ttu-id="4d821-127">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="4d821-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="4d821-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="4d821-128">wpa2Enterprise</span></span>|<span data-ttu-id="4d821-129">5 </span><span class="sxs-lookup"><span data-stu-id="4d821-129">5</span></span>|<span data-ttu-id="4d821-130">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="4d821-130">WPA2-Enterprise.</span></span> <span data-ttu-id="4d821-131">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4d821-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



