---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22dd7bf07e6355dd92f04461120e3afb142d6d9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048878"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="e6973-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="e6973-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="e6973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6973-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6973-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6973-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6973-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6973-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6973-107">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="e6973-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="e6973-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e6973-108">Members</span></span>
|<span data-ttu-id="e6973-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e6973-109">Member</span></span>|<span data-ttu-id="e6973-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e6973-110">Value</span></span>|<span data-ttu-id="e6973-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e6973-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6973-112">окно</span><span class="sxs-lookup"><span data-stu-id="e6973-112">open</span></span>|<span data-ttu-id="e6973-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e6973-113">0</span></span>|<span data-ttu-id="e6973-114">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="e6973-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="e6973-115">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="e6973-115">wpaPersonal</span></span>|<span data-ttu-id="e6973-116">1 </span><span class="sxs-lookup"><span data-stu-id="e6973-116">1</span></span>|<span data-ttu-id="e6973-117">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="e6973-117">WPA-Personal.</span></span>|
|<span data-ttu-id="e6973-118">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="e6973-118">wpaEnterprise</span></span>|<span data-ttu-id="e6973-119">2 </span><span class="sxs-lookup"><span data-stu-id="e6973-119">2</span></span>|<span data-ttu-id="e6973-120">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="e6973-120">WPA-Enterprise.</span></span> <span data-ttu-id="e6973-121">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e6973-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="e6973-122">WEP</span><span class="sxs-lookup"><span data-stu-id="e6973-122">wep</span></span>|<span data-ttu-id="e6973-123">4</span><span class="sxs-lookup"><span data-stu-id="e6973-123">3</span></span>|<span data-ttu-id="e6973-124">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="e6973-124">WEP Encryption.</span></span>|
|<span data-ttu-id="e6973-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="e6973-125">wpa2Personal</span></span>|<span data-ttu-id="e6973-126">4 </span><span class="sxs-lookup"><span data-stu-id="e6973-126">4</span></span>|<span data-ttu-id="e6973-127">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="e6973-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="e6973-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="e6973-128">wpa2Enterprise</span></span>|<span data-ttu-id="e6973-129">5 </span><span class="sxs-lookup"><span data-stu-id="e6973-129">5</span></span>|<span data-ttu-id="e6973-130">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="e6973-130">WPA2-Enterprise.</span></span> <span data-ttu-id="e6973-131">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="e6973-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|






