---
title: тип перечисления Вифисекурититипе
description: Типы безопасности Wi/Fi.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c16265ecf9b4fa56536838dde1f4f1f757d8b1f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159047"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="bc252-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="bc252-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="bc252-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc252-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc252-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc252-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc252-106">Типы безопасности Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="bc252-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="bc252-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bc252-107">Members</span></span>
|<span data-ttu-id="bc252-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bc252-108">Member</span></span>|<span data-ttu-id="bc252-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bc252-109">Value</span></span>|<span data-ttu-id="bc252-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc252-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc252-111">окно</span><span class="sxs-lookup"><span data-stu-id="bc252-111">open</span></span>|<span data-ttu-id="bc252-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bc252-112">0</span></span>|<span data-ttu-id="bc252-113">Открыть (без проверки поДлинности).</span><span class="sxs-lookup"><span data-stu-id="bc252-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="bc252-114">Впаперсонал</span><span class="sxs-lookup"><span data-stu-id="bc252-114">wpaPersonal</span></span>|<span data-ttu-id="bc252-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bc252-115">1</span></span>|<span data-ttu-id="bc252-116">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="bc252-116">WPA-Personal.</span></span>|
|<span data-ttu-id="bc252-117">Впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="bc252-117">wpaEnterprise</span></span>|<span data-ttu-id="bc252-118">2</span><span class="sxs-lookup"><span data-stu-id="bc252-118">2</span></span>|<span data-ttu-id="bc252-119">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="bc252-119">WPA-Enterprise.</span></span> <span data-ttu-id="bc252-120">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc252-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="bc252-121">WEP</span><span class="sxs-lookup"><span data-stu-id="bc252-121">wep</span></span>|<span data-ttu-id="bc252-122">4</span><span class="sxs-lookup"><span data-stu-id="bc252-122">3</span></span>|<span data-ttu-id="bc252-123">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="bc252-123">WEP Encryption.</span></span>|
|<span data-ttu-id="bc252-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="bc252-124">wpa2Personal</span></span>|<span data-ttu-id="bc252-125">4</span><span class="sxs-lookup"><span data-stu-id="bc252-125">4</span></span>|<span data-ttu-id="bc252-126">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="bc252-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="bc252-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="bc252-127">wpa2Enterprise</span></span>|<span data-ttu-id="bc252-128">17:00</span><span class="sxs-lookup"><span data-stu-id="bc252-128">5</span></span>|<span data-ttu-id="bc252-129">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="bc252-129">WPA2-Enterprise.</span></span> <span data-ttu-id="bc252-130">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="bc252-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




