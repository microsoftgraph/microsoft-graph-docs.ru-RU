---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 33d7116bb686945672d96d20035d18ed1df3ee9e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525707"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="8813c-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="8813c-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="8813c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8813c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8813c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8813c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8813c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8813c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8813c-107">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="8813c-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="8813c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8813c-108">Members</span></span>
|<span data-ttu-id="8813c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8813c-109">Member</span></span>|<span data-ttu-id="8813c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8813c-110">Value</span></span>|<span data-ttu-id="8813c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8813c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8813c-112">окно</span><span class="sxs-lookup"><span data-stu-id="8813c-112">open</span></span>|<span data-ttu-id="8813c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8813c-113">0</span></span>|<span data-ttu-id="8813c-114">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="8813c-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="8813c-115">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="8813c-115">wpaPersonal</span></span>|<span data-ttu-id="8813c-116">1 </span><span class="sxs-lookup"><span data-stu-id="8813c-116">1</span></span>|<span data-ttu-id="8813c-117">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="8813c-117">WPA-Personal.</span></span>|
|<span data-ttu-id="8813c-118">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="8813c-118">wpaEnterprise</span></span>|<span data-ttu-id="8813c-119">2 </span><span class="sxs-lookup"><span data-stu-id="8813c-119">2</span></span>|<span data-ttu-id="8813c-120">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="8813c-120">WPA-Enterprise.</span></span> <span data-ttu-id="8813c-121">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8813c-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="8813c-122">WEP</span><span class="sxs-lookup"><span data-stu-id="8813c-122">wep</span></span>|<span data-ttu-id="8813c-123">3 </span><span class="sxs-lookup"><span data-stu-id="8813c-123">3</span></span>|<span data-ttu-id="8813c-124">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="8813c-124">WEP Encryption.</span></span>|
|<span data-ttu-id="8813c-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="8813c-125">wpa2Personal</span></span>|<span data-ttu-id="8813c-126">4 </span><span class="sxs-lookup"><span data-stu-id="8813c-126">4</span></span>|<span data-ttu-id="8813c-127">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="8813c-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="8813c-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="8813c-128">wpa2Enterprise</span></span>|<span data-ttu-id="8813c-129">5 </span><span class="sxs-lookup"><span data-stu-id="8813c-129">5</span></span>|<span data-ttu-id="8813c-130">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="8813c-130">WPA2-Enterprise.</span></span> <span data-ttu-id="8813c-131">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="8813c-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



