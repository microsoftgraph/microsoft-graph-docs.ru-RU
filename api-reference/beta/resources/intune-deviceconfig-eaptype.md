---
title: тип перечисления Еаптипе
description: Типы конфигурации протокола EAP (Extensible Authentication Protocol).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0d67147c281805e6d626f3f5e12fb5346ca90356
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712031"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="98f9a-103">тип перечисления Еаптипе</span><span class="sxs-lookup"><span data-stu-id="98f9a-103">eapType enum type</span></span>

<span data-ttu-id="98f9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98f9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98f9a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98f9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98f9a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98f9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98f9a-107">Типы конфигурации протокола EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="98f9a-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>

## <a name="members"></a><span data-ttu-id="98f9a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="98f9a-108">Members</span></span>
|<span data-ttu-id="98f9a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="98f9a-109">Member</span></span>|<span data-ttu-id="98f9a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="98f9a-110">Value</span></span>|<span data-ttu-id="98f9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98f9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98f9a-112">еаптлс</span><span class="sxs-lookup"><span data-stu-id="98f9a-112">eapTls</span></span>|<span data-ttu-id="98f9a-113">13 </span><span class="sxs-lookup"><span data-stu-id="98f9a-113">13</span></span>|<span data-ttu-id="98f9a-114">EAP-Transport уровня безопасности (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="98f9a-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="98f9a-115">LEAP</span><span class="sxs-lookup"><span data-stu-id="98f9a-115">leap</span></span>|<span data-ttu-id="98f9a-116">17 </span><span class="sxs-lookup"><span data-stu-id="98f9a-116">17</span></span>|<span data-ttu-id="98f9a-117">Облегченный протокол проверки подлинности (LEAP).</span><span class="sxs-lookup"><span data-stu-id="98f9a-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="98f9a-118">еапсим</span><span class="sxs-lookup"><span data-stu-id="98f9a-118">eapSim</span></span>|<span data-ttu-id="98f9a-119">18 </span><span class="sxs-lookup"><span data-stu-id="98f9a-119">18</span></span>|<span data-ttu-id="98f9a-120">EAP для модуля удостоверения абонента GSM (EAP-SIM).</span><span class="sxs-lookup"><span data-stu-id="98f9a-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="98f9a-121">еапттлс</span><span class="sxs-lookup"><span data-stu-id="98f9a-121">eapTtls</span></span>|<span data-ttu-id="98f9a-122">21</span><span class="sxs-lookup"><span data-stu-id="98f9a-122">21</span></span>|<span data-ttu-id="98f9a-123">EAP-Tunneled TLS (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="98f9a-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="98f9a-124">протокола</span><span class="sxs-lookup"><span data-stu-id="98f9a-124">peap</span></span>|<span data-ttu-id="98f9a-125">25</span><span class="sxs-lookup"><span data-stu-id="98f9a-125">25</span></span>|<span data-ttu-id="98f9a-126">Протокол PEAP (protected Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="98f9a-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="98f9a-127">еапфаст</span><span class="sxs-lookup"><span data-stu-id="98f9a-127">eapFast</span></span>|<span data-ttu-id="98f9a-128">43</span><span class="sxs-lookup"><span data-stu-id="98f9a-128">43</span></span>|<span data-ttu-id="98f9a-129">Проверка подлинности EAP-Flexible с помощью безопасного туннелирования (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="98f9a-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





