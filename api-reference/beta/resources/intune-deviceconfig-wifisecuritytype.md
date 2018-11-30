---
title: Тип перечисления wiFiSecurityType
description: Типы безопасности Wi-Fi.
ms.openlocfilehash: ee6afc55b4ccf8550c9df5c790cd325561cb6f3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080788"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="06733-103">Тип перечисления wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="06733-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="06733-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06733-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06733-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06733-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06733-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06733-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06733-107">Типы безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="06733-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="06733-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="06733-108">Members</span></span>
|<span data-ttu-id="06733-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="06733-109">Member</span></span>|<span data-ttu-id="06733-110">Значение</span><span class="sxs-lookup"><span data-stu-id="06733-110">Value</span></span>|<span data-ttu-id="06733-111">Description</span><span class="sxs-lookup"><span data-stu-id="06733-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06733-112">Откройте</span><span class="sxs-lookup"><span data-stu-id="06733-112">open</span></span>|<span data-ttu-id="06733-113">0</span><span class="sxs-lookup"><span data-stu-id="06733-113">0</span></span>|<span data-ttu-id="06733-114">Откройте (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="06733-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="06733-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="06733-115">wpaPersonal</span></span>|<span data-ttu-id="06733-116">1</span><span class="sxs-lookup"><span data-stu-id="06733-116">1</span></span>|<span data-ttu-id="06733-117">WPA-Personal.</span><span class="sxs-lookup"><span data-stu-id="06733-117">WPA-Personal.</span></span>|
|<span data-ttu-id="06733-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="06733-118">wpaEnterprise</span></span>|<span data-ttu-id="06733-119">2</span><span class="sxs-lookup"><span data-stu-id="06733-119">2</span></span>|<span data-ttu-id="06733-120">WPA-предприятие.</span><span class="sxs-lookup"><span data-stu-id="06733-120">WPA-Enterprise.</span></span> <span data-ttu-id="06733-121">Необходимо использовать тип IOSEnterpriseWifiConfiguration позволяет настроить параметры enterprise.</span><span class="sxs-lookup"><span data-stu-id="06733-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="06733-122">WEP</span><span class="sxs-lookup"><span data-stu-id="06733-122">wep</span></span>|<span data-ttu-id="06733-123">3</span><span class="sxs-lookup"><span data-stu-id="06733-123">3</span></span>|<span data-ttu-id="06733-124">Шифрования WEP.</span><span class="sxs-lookup"><span data-stu-id="06733-124">WEP Encryption.</span></span>|
|<span data-ttu-id="06733-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="06733-125">wpa2Personal</span></span>|<span data-ttu-id="06733-126">4</span><span class="sxs-lookup"><span data-stu-id="06733-126">4</span></span>|<span data-ttu-id="06733-127">WPA2-личное.</span><span class="sxs-lookup"><span data-stu-id="06733-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="06733-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="06733-128">wpa2Enterprise</span></span>|<span data-ttu-id="06733-129">5</span><span class="sxs-lookup"><span data-stu-id="06733-129">5</span></span>|<span data-ttu-id="06733-130">WPA2-предприятие.</span><span class="sxs-lookup"><span data-stu-id="06733-130">WPA2-Enterprise.</span></span> <span data-ttu-id="06733-131">Необходимо использовать тип WindowsWifiEnterpriseEAPConfiguration позволяет настроить параметры enterprise.</span><span class="sxs-lookup"><span data-stu-id="06733-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





