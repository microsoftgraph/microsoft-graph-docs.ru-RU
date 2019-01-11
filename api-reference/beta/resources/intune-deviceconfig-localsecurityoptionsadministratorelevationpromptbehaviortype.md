---
title: Тип перечисления localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Возможные значения для LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 424c1193015d688019892d66ed07588358dcb8c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870884"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="a5981-103">Тип перечисления localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="a5981-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="a5981-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5981-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5981-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5981-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5981-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a5981-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5981-107">Возможные значения для LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="a5981-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="a5981-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a5981-108">Members</span></span>
|<span data-ttu-id="a5981-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a5981-109">Member</span></span>|<span data-ttu-id="a5981-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a5981-110">Value</span></span>|<span data-ttu-id="a5981-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5981-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5981-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a5981-112">notConfigured</span></span>|<span data-ttu-id="a5981-113">0</span><span class="sxs-lookup"><span data-stu-id="a5981-113">0</span></span>|<span data-ttu-id="a5981-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="a5981-114">Not Configured</span></span>|
|<span data-ttu-id="a5981-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="a5981-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="a5981-116">1</span><span class="sxs-lookup"><span data-stu-id="a5981-116">1</span></span>|<span data-ttu-id="a5981-117">Повышение без запроса.</span><span class="sxs-lookup"><span data-stu-id="a5981-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="a5981-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="a5981-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="a5981-119">2</span><span class="sxs-lookup"><span data-stu-id="a5981-119">2</span></span>|<span data-ttu-id="a5981-120">Запрос учетных данных в системе безопасности</span><span class="sxs-lookup"><span data-stu-id="a5981-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="a5981-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="a5981-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="a5981-122">3</span><span class="sxs-lookup"><span data-stu-id="a5981-122">3</span></span>|<span data-ttu-id="a5981-123">Запрос согласия рабочий стол</span><span class="sxs-lookup"><span data-stu-id="a5981-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="a5981-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="a5981-124">promptForCredentials</span></span>|<span data-ttu-id="a5981-125">4</span><span class="sxs-lookup"><span data-stu-id="a5981-125">4</span></span>|<span data-ttu-id="a5981-126">Запрос учетных данных</span><span class="sxs-lookup"><span data-stu-id="a5981-126">Prompt for credentials</span></span>|
|<span data-ttu-id="a5981-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="a5981-127">promptForConsent</span></span>|<span data-ttu-id="a5981-128">5</span><span class="sxs-lookup"><span data-stu-id="a5981-128">5</span></span>|<span data-ttu-id="a5981-129">Запрашивать согласие</span><span class="sxs-lookup"><span data-stu-id="a5981-129">Prompt for consent</span></span>|
|<span data-ttu-id="a5981-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="a5981-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="a5981-131">6</span><span class="sxs-lookup"><span data-stu-id="a5981-131">6</span></span>|<span data-ttu-id="a5981-132">Запрос согласия для двоичных файлов отличных от Windows</span><span class="sxs-lookup"><span data-stu-id="a5981-132">Prompt for consent for non-Windows binaries</span></span>|





