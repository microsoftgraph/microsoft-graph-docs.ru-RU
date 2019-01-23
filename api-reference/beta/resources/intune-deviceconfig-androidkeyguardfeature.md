---
title: Тип перечисления androidKeyguardFeature
description: Функциональная возможность, Android keyguard.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430666"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="212ad-103">Тип перечисления androidKeyguardFeature</span><span class="sxs-lookup"><span data-stu-id="212ad-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="212ad-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="212ad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="212ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="212ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="212ad-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="212ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="212ad-107">Функциональная возможность, Android keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="212ad-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="212ad-108">Members</span></span>
|<span data-ttu-id="212ad-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="212ad-109">Member</span></span>|<span data-ttu-id="212ad-110">Значение</span><span class="sxs-lookup"><span data-stu-id="212ad-110">Value</span></span>|<span data-ttu-id="212ad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="212ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="212ad-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="212ad-112">notConfigured</span></span>|<span data-ttu-id="212ad-113">0</span><span class="sxs-lookup"><span data-stu-id="212ad-113">0</span></span>|<span data-ttu-id="212ad-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="212ad-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="212ad-115">камера</span><span class="sxs-lookup"><span data-stu-id="212ad-115">camera</span></span>|<span data-ttu-id="212ad-116">1</span><span class="sxs-lookup"><span data-stu-id="212ad-116">1</span></span>|<span data-ttu-id="212ad-117">Об использовании камеры при на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="212ad-118">уведомления</span><span class="sxs-lookup"><span data-stu-id="212ad-118">notifications</span></span>|<span data-ttu-id="212ad-119">2</span><span class="sxs-lookup"><span data-stu-id="212ad-119">2</span></span>|<span data-ttu-id="212ad-120">Отображение уведомлений при на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="212ad-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="212ad-121">unredactedNotifications</span></span>|<span data-ttu-id="212ad-122">3</span><span class="sxs-lookup"><span data-stu-id="212ad-122">3</span></span>|<span data-ttu-id="212ad-123">Отображение unredacted уведомлений при на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="212ad-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="212ad-124">trustAgents</span></span>|<span data-ttu-id="212ad-125">4</span><span class="sxs-lookup"><span data-stu-id="212ad-125">4</span></span>|<span data-ttu-id="212ad-126">Можно отметить состояние агента на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="212ad-127">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="212ad-127">fingerprint</span></span>|<span data-ttu-id="212ad-128">5</span><span class="sxs-lookup"><span data-stu-id="212ad-128">5</span></span>|<span data-ttu-id="212ad-129">Отпечаток об использовании датчика на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="212ad-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="212ad-130">remoteInput</span></span>|<span data-ttu-id="212ad-131">6</span><span class="sxs-lookup"><span data-stu-id="212ad-131">6</span></span>|<span data-ttu-id="212ad-132">Запись текста уведомлений при на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="212ad-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="212ad-133">allFeatures</span></span>|<span data-ttu-id="212ad-134">7</span><span class="sxs-lookup"><span data-stu-id="212ad-134">7</span></span>|<span data-ttu-id="212ad-135">Все функции keyguard при на экранах безопасной keyguard.</span><span class="sxs-lookup"><span data-stu-id="212ad-135">All keyguard features when on secure keyguard screens.</span></span>|




