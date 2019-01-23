---
title: Тип перечисления wiFiSecurityType
description: Типы безопасности Wi-Fi.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422133"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="ca2a2-103">Тип перечисления wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ca2a2-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="ca2a2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca2a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca2a2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca2a2-107">Типы безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="ca2a2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ca2a2-108">Members</span></span>
|<span data-ttu-id="ca2a2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ca2a2-109">Member</span></span>|<span data-ttu-id="ca2a2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ca2a2-110">Value</span></span>|<span data-ttu-id="ca2a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca2a2-112">Откройте</span><span class="sxs-lookup"><span data-stu-id="ca2a2-112">open</span></span>|<span data-ttu-id="ca2a2-113">0</span><span class="sxs-lookup"><span data-stu-id="ca2a2-113">0</span></span>|<span data-ttu-id="ca2a2-114">Откройте (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="ca2a2-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="ca2a2-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="ca2a2-115">wpaPersonal</span></span>|<span data-ttu-id="ca2a2-116">1</span><span class="sxs-lookup"><span data-stu-id="ca2a2-116">1</span></span>|<span data-ttu-id="ca2a2-117">WPA-Personal.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-117">WPA-Personal.</span></span>|
|<span data-ttu-id="ca2a2-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="ca2a2-118">wpaEnterprise</span></span>|<span data-ttu-id="ca2a2-119">2</span><span class="sxs-lookup"><span data-stu-id="ca2a2-119">2</span></span>|<span data-ttu-id="ca2a2-120">WPA-предприятие.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-120">WPA-Enterprise.</span></span> <span data-ttu-id="ca2a2-121">Необходимо использовать тип IOSEnterpriseWifiConfiguration позволяет настроить параметры enterprise.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="ca2a2-122">WEP</span><span class="sxs-lookup"><span data-stu-id="ca2a2-122">wep</span></span>|<span data-ttu-id="ca2a2-123">3</span><span class="sxs-lookup"><span data-stu-id="ca2a2-123">3</span></span>|<span data-ttu-id="ca2a2-124">Шифрования WEP.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-124">WEP Encryption.</span></span>|
|<span data-ttu-id="ca2a2-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="ca2a2-125">wpa2Personal</span></span>|<span data-ttu-id="ca2a2-126">4</span><span class="sxs-lookup"><span data-stu-id="ca2a2-126">4</span></span>|<span data-ttu-id="ca2a2-127">WPA2-личное.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="ca2a2-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="ca2a2-128">wpa2Enterprise</span></span>|<span data-ttu-id="ca2a2-129">5</span><span class="sxs-lookup"><span data-stu-id="ca2a2-129">5</span></span>|<span data-ttu-id="ca2a2-130">WPA2-предприятие.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-130">WPA2-Enterprise.</span></span> <span data-ttu-id="ca2a2-131">Необходимо использовать тип WindowsWifiEnterpriseEAPConfiguration позволяет настроить параметры enterprise.</span><span class="sxs-lookup"><span data-stu-id="ca2a2-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




