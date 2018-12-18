---
title: Тип перечисления eapType
description: Расширяемые типы конфигурации протокола проверки подлинности (EAP).
author: tfitzmac
ms.openlocfilehash: e95924209b8137a1c5d35896c0195e9e962d7af9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319546"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="e724c-103">Тип перечисления eapType</span><span class="sxs-lookup"><span data-stu-id="e724c-103">eapType enum type</span></span>

> <span data-ttu-id="e724c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e724c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e724c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e724c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e724c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e724c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e724c-107">Расширяемые типы конфигурации протокола проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="e724c-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="e724c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e724c-108">Members</span></span>
|<span data-ttu-id="e724c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e724c-109">Member</span></span>|<span data-ttu-id="e724c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e724c-110">Value</span></span>|<span data-ttu-id="e724c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e724c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e724c-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="e724c-112">eapTls</span></span>|<span data-ttu-id="e724c-113">13</span><span class="sxs-lookup"><span data-stu-id="e724c-113">13</span></span>|<span data-ttu-id="e724c-114">Поставщик внешних Приложений Transport Layer Security (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="e724c-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="e724c-115">рост</span><span class="sxs-lookup"><span data-stu-id="e724c-115">leap</span></span>|<span data-ttu-id="e724c-116">17</span><span class="sxs-lookup"><span data-stu-id="e724c-116">17</span></span>|<span data-ttu-id="e724c-117">Протокол Lightweight расширенной проверки подлинности (шаг).</span><span class="sxs-lookup"><span data-stu-id="e724c-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="e724c-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="e724c-118">eapSim</span></span>|<span data-ttu-id="e724c-119">18</span><span class="sxs-lookup"><span data-stu-id="e724c-119">18</span></span>|<span data-ttu-id="e724c-120">Поставщик внешних Приложений с модулем удостоверения подписчика GSM (EAP-диспетчер установки).</span><span class="sxs-lookup"><span data-stu-id="e724c-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="e724c-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="e724c-121">eapTtls</span></span>|<span data-ttu-id="e724c-122">21</span><span class="sxs-lookup"><span data-stu-id="e724c-122">21</span></span>|<span data-ttu-id="e724c-123">Туннелирование EAP Transport Layer Security (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="e724c-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="e724c-124">PEAP</span><span class="sxs-lookup"><span data-stu-id="e724c-124">peap</span></span>|<span data-ttu-id="e724c-125">25</span><span class="sxs-lookup"><span data-stu-id="e724c-125">25</span></span>|<span data-ttu-id="e724c-126">Протокол расширенной проверки подлинности (PEAP).</span><span class="sxs-lookup"><span data-stu-id="e724c-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="e724c-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="e724c-127">eapFast</span></span>|<span data-ttu-id="e724c-128">43</span><span class="sxs-lookup"><span data-stu-id="e724c-128">43</span></span>|<span data-ttu-id="e724c-129">Гибкие EAP проверки подлинности с помощью Secure туннелирование (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="e724c-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





