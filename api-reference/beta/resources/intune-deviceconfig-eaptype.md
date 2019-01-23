---
title: Тип перечисления eapType
description: Расширяемые типы конфигурации протокола проверки подлинности (EAP).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 268a3190b06834d24c63d7ca5117a00fe7dc70d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405830"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="a6fde-103">Тип перечисления eapType</span><span class="sxs-lookup"><span data-stu-id="a6fde-103">eapType enum type</span></span>

> <span data-ttu-id="a6fde-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6fde-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6fde-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6fde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6fde-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6fde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6fde-107">Расширяемые типы конфигурации протокола проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="a6fde-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>

## <a name="members"></a><span data-ttu-id="a6fde-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a6fde-108">Members</span></span>
|<span data-ttu-id="a6fde-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a6fde-109">Member</span></span>|<span data-ttu-id="a6fde-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a6fde-110">Value</span></span>|<span data-ttu-id="a6fde-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6fde-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="a6fde-112">eapTls</span></span>|<span data-ttu-id="a6fde-113">13</span><span class="sxs-lookup"><span data-stu-id="a6fde-113">13</span></span>|<span data-ttu-id="a6fde-114">Поставщик внешних Приложений Transport Layer Security (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="a6fde-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="a6fde-115">рост</span><span class="sxs-lookup"><span data-stu-id="a6fde-115">leap</span></span>|<span data-ttu-id="a6fde-116">17</span><span class="sxs-lookup"><span data-stu-id="a6fde-116">17</span></span>|<span data-ttu-id="a6fde-117">Протокол Lightweight расширенной проверки подлинности (шаг).</span><span class="sxs-lookup"><span data-stu-id="a6fde-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="a6fde-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="a6fde-118">eapSim</span></span>|<span data-ttu-id="a6fde-119">18</span><span class="sxs-lookup"><span data-stu-id="a6fde-119">18</span></span>|<span data-ttu-id="a6fde-120">Поставщик внешних Приложений с модулем удостоверения подписчика GSM (EAP-диспетчер установки).</span><span class="sxs-lookup"><span data-stu-id="a6fde-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="a6fde-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="a6fde-121">eapTtls</span></span>|<span data-ttu-id="a6fde-122">21</span><span class="sxs-lookup"><span data-stu-id="a6fde-122">21</span></span>|<span data-ttu-id="a6fde-123">Туннелирование EAP Transport Layer Security (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="a6fde-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="a6fde-124">PEAP</span><span class="sxs-lookup"><span data-stu-id="a6fde-124">peap</span></span>|<span data-ttu-id="a6fde-125">25</span><span class="sxs-lookup"><span data-stu-id="a6fde-125">25</span></span>|<span data-ttu-id="a6fde-126">Протокол расширенной проверки подлинности (PEAP).</span><span class="sxs-lookup"><span data-stu-id="a6fde-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="a6fde-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="a6fde-127">eapFast</span></span>|<span data-ttu-id="a6fde-128">43</span><span class="sxs-lookup"><span data-stu-id="a6fde-128">43</span></span>|<span data-ttu-id="a6fde-129">Гибкие EAP проверки подлинности с помощью Secure туннелирование (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="a6fde-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|




