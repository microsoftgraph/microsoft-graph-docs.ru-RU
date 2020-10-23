---
title: тип перечисления Вифисекурититипе
description: Wi-Fi типов безопасности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e01faac094cd2ae040137b251d30006883388173
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732532"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="42cbe-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="42cbe-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="42cbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42cbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42cbe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42cbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42cbe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42cbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42cbe-107">Wi-Fi типов безопасности.</span><span class="sxs-lookup"><span data-stu-id="42cbe-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="42cbe-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="42cbe-108">Members</span></span>
|<span data-ttu-id="42cbe-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="42cbe-109">Member</span></span>|<span data-ttu-id="42cbe-110">Значение</span><span class="sxs-lookup"><span data-stu-id="42cbe-110">Value</span></span>|<span data-ttu-id="42cbe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="42cbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42cbe-112">окно</span><span class="sxs-lookup"><span data-stu-id="42cbe-112">open</span></span>|<span data-ttu-id="42cbe-113">нуль</span><span class="sxs-lookup"><span data-stu-id="42cbe-113">0</span></span>|<span data-ttu-id="42cbe-114">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="42cbe-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="42cbe-115">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="42cbe-115">wpaPersonal</span></span>|<span data-ttu-id="42cbe-116">1,1</span><span class="sxs-lookup"><span data-stu-id="42cbe-116">1</span></span>|<span data-ttu-id="42cbe-117">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="42cbe-117">WPA-Personal.</span></span>|
|<span data-ttu-id="42cbe-118">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="42cbe-118">wpaEnterprise</span></span>|<span data-ttu-id="42cbe-119">2</span><span class="sxs-lookup"><span data-stu-id="42cbe-119">2</span></span>|<span data-ttu-id="42cbe-120">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="42cbe-120">WPA-Enterprise.</span></span> <span data-ttu-id="42cbe-121">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="42cbe-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="42cbe-122">WEP</span><span class="sxs-lookup"><span data-stu-id="42cbe-122">wep</span></span>|<span data-ttu-id="42cbe-123">4</span><span class="sxs-lookup"><span data-stu-id="42cbe-123">3</span></span>|<span data-ttu-id="42cbe-124">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="42cbe-124">WEP Encryption.</span></span>|
|<span data-ttu-id="42cbe-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="42cbe-125">wpa2Personal</span></span>|<span data-ttu-id="42cbe-126">4 </span><span class="sxs-lookup"><span data-stu-id="42cbe-126">4</span></span>|<span data-ttu-id="42cbe-127">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="42cbe-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="42cbe-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="42cbe-128">wpa2Enterprise</span></span>|<span data-ttu-id="42cbe-129">5 </span><span class="sxs-lookup"><span data-stu-id="42cbe-129">5</span></span>|<span data-ttu-id="42cbe-130">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="42cbe-130">WPA2-Enterprise.</span></span> <span data-ttu-id="42cbe-131">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="42cbe-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





