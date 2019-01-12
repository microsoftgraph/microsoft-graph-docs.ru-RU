---
title: Тип перечисления eapType
description: Расширяемые типы конфигурации протокола проверки подлинности (EAP).
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e894e10356711fd4522ff816750e986d8b8e57d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957811"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="0ce3d-103">Тип перечисления eapType</span><span class="sxs-lookup"><span data-stu-id="0ce3d-103">eapType enum type</span></span>

> <span data-ttu-id="0ce3d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ce3d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ce3d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ce3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ce3d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ce3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ce3d-107">Расширяемые типы конфигурации протокола проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="0ce3d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0ce3d-108">Members</span></span>
|<span data-ttu-id="0ce3d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0ce3d-109">Member</span></span>|<span data-ttu-id="0ce3d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0ce3d-110">Value</span></span>|<span data-ttu-id="0ce3d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ce3d-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="0ce3d-112">eapTls</span></span>|<span data-ttu-id="0ce3d-113">13</span><span class="sxs-lookup"><span data-stu-id="0ce3d-113">13</span></span>|<span data-ttu-id="0ce3d-114">Поставщик внешних Приложений Transport Layer Security (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="0ce3d-115">рост</span><span class="sxs-lookup"><span data-stu-id="0ce3d-115">leap</span></span>|<span data-ttu-id="0ce3d-116">17</span><span class="sxs-lookup"><span data-stu-id="0ce3d-116">17</span></span>|<span data-ttu-id="0ce3d-117">Протокол Lightweight расширенной проверки подлинности (шаг).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="0ce3d-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="0ce3d-118">eapSim</span></span>|<span data-ttu-id="0ce3d-119">18</span><span class="sxs-lookup"><span data-stu-id="0ce3d-119">18</span></span>|<span data-ttu-id="0ce3d-120">Поставщик внешних Приложений с модулем удостоверения подписчика GSM (EAP-диспетчер установки).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="0ce3d-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="0ce3d-121">eapTtls</span></span>|<span data-ttu-id="0ce3d-122">21</span><span class="sxs-lookup"><span data-stu-id="0ce3d-122">21</span></span>|<span data-ttu-id="0ce3d-123">Туннелирование EAP Transport Layer Security (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="0ce3d-124">PEAP</span><span class="sxs-lookup"><span data-stu-id="0ce3d-124">peap</span></span>|<span data-ttu-id="0ce3d-125">25</span><span class="sxs-lookup"><span data-stu-id="0ce3d-125">25</span></span>|<span data-ttu-id="0ce3d-126">Протокол расширенной проверки подлинности (PEAP).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="0ce3d-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="0ce3d-127">eapFast</span></span>|<span data-ttu-id="0ce3d-128">43</span><span class="sxs-lookup"><span data-stu-id="0ce3d-128">43</span></span>|<span data-ttu-id="0ce3d-129">Гибкие EAP проверки подлинности с помощью Secure туннелирование (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="0ce3d-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





