---
title: тип перечисления Андроидкэйгуардфеатуре
description: Функция Android кэйгуард.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 46acc2917c8534a58221ba31f23690f84b716f81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527324"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="32122-103">тип перечисления Андроидкэйгуардфеатуре</span><span class="sxs-lookup"><span data-stu-id="32122-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="32122-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32122-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32122-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32122-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32122-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32122-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32122-107">Функция Android кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="32122-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="32122-108">Members</span></span>
|<span data-ttu-id="32122-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="32122-109">Member</span></span>|<span data-ttu-id="32122-110">Значение</span><span class="sxs-lookup"><span data-stu-id="32122-110">Value</span></span>|<span data-ttu-id="32122-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32122-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32122-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="32122-112">notConfigured</span></span>|<span data-ttu-id="32122-113">нуль</span><span class="sxs-lookup"><span data-stu-id="32122-113">0</span></span>|<span data-ttu-id="32122-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="32122-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="32122-115">видеокамер</span><span class="sxs-lookup"><span data-stu-id="32122-115">camera</span></span>|<span data-ttu-id="32122-116">1 </span><span class="sxs-lookup"><span data-stu-id="32122-116">1</span></span>|<span data-ttu-id="32122-117">Использование камеры в защищенных экранах кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="32122-118">уведомления</span><span class="sxs-lookup"><span data-stu-id="32122-118">notifications</span></span>|<span data-ttu-id="32122-119">2 </span><span class="sxs-lookup"><span data-stu-id="32122-119">2</span></span>|<span data-ttu-id="32122-120">Отображение уведомлений при использовании экранов безопасного кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="32122-121">унредактеднотификатионс</span><span class="sxs-lookup"><span data-stu-id="32122-121">unredactedNotifications</span></span>|<span data-ttu-id="32122-122">3 </span><span class="sxs-lookup"><span data-stu-id="32122-122">3</span></span>|<span data-ttu-id="32122-123">Отображение уведомлений унредактед при использовании безопасного экрана кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="32122-124">трустажентс</span><span class="sxs-lookup"><span data-stu-id="32122-124">trustAgents</span></span>|<span data-ttu-id="32122-125">4 </span><span class="sxs-lookup"><span data-stu-id="32122-125">4</span></span>|<span data-ttu-id="32122-126">Состояние агента доверия при использовании экранов безопасного кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="32122-127">распознавания</span><span class="sxs-lookup"><span data-stu-id="32122-127">fingerprint</span></span>|<span data-ttu-id="32122-128">5 </span><span class="sxs-lookup"><span data-stu-id="32122-128">5</span></span>|<span data-ttu-id="32122-129">Использование датчиков отпечатков пальцев в защищенных экранах кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="32122-130">ремотеинпут</span><span class="sxs-lookup"><span data-stu-id="32122-130">remoteInput</span></span>|<span data-ttu-id="32122-131">6 </span><span class="sxs-lookup"><span data-stu-id="32122-131">6</span></span>|<span data-ttu-id="32122-132">Ввод текста уведомления при использовании экранов безопасного кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="32122-133">аллфеатурес</span><span class="sxs-lookup"><span data-stu-id="32122-133">allFeatures</span></span>|<span data-ttu-id="32122-134">7 </span><span class="sxs-lookup"><span data-stu-id="32122-134">7</span></span>|<span data-ttu-id="32122-135">Все компоненты кэйгуард, когда на экранах безопасности кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="32122-135">All keyguard features when on secure keyguard screens.</span></span>|



