---
title: тип перечисления Андроидкэйгуардфеатуре
description: Функция Android кэйгуард.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15e0c8f1dc14dae41b917e85867020fb4d57571f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690716"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="3b46b-103">тип перечисления Андроидкэйгуардфеатуре</span><span class="sxs-lookup"><span data-stu-id="3b46b-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="3b46b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b46b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b46b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b46b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b46b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b46b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b46b-107">Функция Android кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="3b46b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3b46b-108">Members</span></span>
|<span data-ttu-id="3b46b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3b46b-109">Member</span></span>|<span data-ttu-id="3b46b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3b46b-110">Value</span></span>|<span data-ttu-id="3b46b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3b46b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b46b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3b46b-112">notConfigured</span></span>|<span data-ttu-id="3b46b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3b46b-113">0</span></span>|<span data-ttu-id="3b46b-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="3b46b-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="3b46b-115">видеокамер</span><span class="sxs-lookup"><span data-stu-id="3b46b-115">camera</span></span>|<span data-ttu-id="3b46b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="3b46b-116">1</span></span>|<span data-ttu-id="3b46b-117">Использование камеры в защищенных экранах кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3b46b-118">уведомления</span><span class="sxs-lookup"><span data-stu-id="3b46b-118">notifications</span></span>|<span data-ttu-id="3b46b-119">2</span><span class="sxs-lookup"><span data-stu-id="3b46b-119">2</span></span>|<span data-ttu-id="3b46b-120">Отображение уведомлений при использовании экранов безопасного кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3b46b-121">унредактеднотификатионс</span><span class="sxs-lookup"><span data-stu-id="3b46b-121">unredactedNotifications</span></span>|<span data-ttu-id="3b46b-122">4</span><span class="sxs-lookup"><span data-stu-id="3b46b-122">3</span></span>|<span data-ttu-id="3b46b-123">Отображение уведомлений унредактед при использовании безопасного экрана кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3b46b-124">трустажентс</span><span class="sxs-lookup"><span data-stu-id="3b46b-124">trustAgents</span></span>|<span data-ttu-id="3b46b-125">4 </span><span class="sxs-lookup"><span data-stu-id="3b46b-125">4</span></span>|<span data-ttu-id="3b46b-126">Состояние агента доверия при использовании экранов безопасного кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3b46b-127">распознавания</span><span class="sxs-lookup"><span data-stu-id="3b46b-127">fingerprint</span></span>|<span data-ttu-id="3b46b-128">5 </span><span class="sxs-lookup"><span data-stu-id="3b46b-128">5</span></span>|<span data-ttu-id="3b46b-129">Использование датчиков отпечатков пальцев в защищенных экранах кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3b46b-130">ремотеинпут</span><span class="sxs-lookup"><span data-stu-id="3b46b-130">remoteInput</span></span>|<span data-ttu-id="3b46b-131">6 </span><span class="sxs-lookup"><span data-stu-id="3b46b-131">6</span></span>|<span data-ttu-id="3b46b-132">Ввод текста уведомления при использовании экранов безопасного кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="3b46b-133">аллфеатурес</span><span class="sxs-lookup"><span data-stu-id="3b46b-133">allFeatures</span></span>|<span data-ttu-id="3b46b-134">7 </span><span class="sxs-lookup"><span data-stu-id="3b46b-134">7</span></span>|<span data-ttu-id="3b46b-135">Все компоненты кэйгуард, когда на экранах безопасности кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3b46b-135">All keyguard features when on secure keyguard screens.</span></span>|





