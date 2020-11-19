---
title: тип перечисления Вифисекурититипе
description: Wi-Fi типов безопасности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 112612969027be87805b77c5743e1a8d0561c03b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215339"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="3c366-103">тип перечисления Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="3c366-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="3c366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c366-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c366-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c366-107">Wi-Fi типов безопасности.</span><span class="sxs-lookup"><span data-stu-id="3c366-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="3c366-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3c366-108">Members</span></span>
|<span data-ttu-id="3c366-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3c366-109">Member</span></span>|<span data-ttu-id="3c366-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3c366-110">Value</span></span>|<span data-ttu-id="3c366-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c366-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c366-112">окно</span><span class="sxs-lookup"><span data-stu-id="3c366-112">open</span></span>|<span data-ttu-id="3c366-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3c366-113">0</span></span>|<span data-ttu-id="3c366-114">Открыть (без проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="3c366-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="3c366-115">впаперсонал</span><span class="sxs-lookup"><span data-stu-id="3c366-115">wpaPersonal</span></span>|<span data-ttu-id="3c366-116">1,1</span><span class="sxs-lookup"><span data-stu-id="3c366-116">1</span></span>|<span data-ttu-id="3c366-117">WPA – личное.</span><span class="sxs-lookup"><span data-stu-id="3c366-117">WPA-Personal.</span></span>|
|<span data-ttu-id="3c366-118">впаентерприсе</span><span class="sxs-lookup"><span data-stu-id="3c366-118">wpaEnterprise</span></span>|<span data-ttu-id="3c366-119">2</span><span class="sxs-lookup"><span data-stu-id="3c366-119">2</span></span>|<span data-ttu-id="3c366-120">WPA — предприятие.</span><span class="sxs-lookup"><span data-stu-id="3c366-120">WPA-Enterprise.</span></span> <span data-ttu-id="3c366-121">Для настройки параметров предприятия необходимо использовать тип IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c366-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="3c366-122">WEP</span><span class="sxs-lookup"><span data-stu-id="3c366-122">wep</span></span>|<span data-ttu-id="3c366-123">4</span><span class="sxs-lookup"><span data-stu-id="3c366-123">3</span></span>|<span data-ttu-id="3c366-124">WEP-шифрование.</span><span class="sxs-lookup"><span data-stu-id="3c366-124">WEP Encryption.</span></span>|
|<span data-ttu-id="3c366-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="3c366-125">wpa2Personal</span></span>|<span data-ttu-id="3c366-126">4 </span><span class="sxs-lookup"><span data-stu-id="3c366-126">4</span></span>|<span data-ttu-id="3c366-127">WPA2 — личное.</span><span class="sxs-lookup"><span data-stu-id="3c366-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="3c366-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="3c366-128">wpa2Enterprise</span></span>|<span data-ttu-id="3c366-129">5 </span><span class="sxs-lookup"><span data-stu-id="3c366-129">5</span></span>|<span data-ttu-id="3c366-130">WPA2 — предприятие.</span><span class="sxs-lookup"><span data-stu-id="3c366-130">WPA2-Enterprise.</span></span> <span data-ttu-id="3c366-131">Для настройки параметров предприятия необходимо использовать тип Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="3c366-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




