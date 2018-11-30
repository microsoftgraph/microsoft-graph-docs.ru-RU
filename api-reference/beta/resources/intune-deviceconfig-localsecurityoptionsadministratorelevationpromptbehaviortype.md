---
title: Тип перечисления localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Возможные значения для LocalSecurityOptionsAdministratorElevationPromptBehavior
ms.openlocfilehash: 2959aebbb12bc567427c8a9b06a5ce2380933241
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078265"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="393ee-103">Тип перечисления localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="393ee-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="393ee-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="393ee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="393ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="393ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="393ee-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="393ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="393ee-107">Возможные значения для LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="393ee-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="393ee-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="393ee-108">Members</span></span>
|<span data-ttu-id="393ee-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="393ee-109">Member</span></span>|<span data-ttu-id="393ee-110">Значение</span><span class="sxs-lookup"><span data-stu-id="393ee-110">Value</span></span>|<span data-ttu-id="393ee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="393ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393ee-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="393ee-112">notConfigured</span></span>|<span data-ttu-id="393ee-113">0</span><span class="sxs-lookup"><span data-stu-id="393ee-113">0</span></span>|<span data-ttu-id="393ee-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="393ee-114">Not Configured</span></span>|
|<span data-ttu-id="393ee-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="393ee-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="393ee-116">1</span><span class="sxs-lookup"><span data-stu-id="393ee-116">1</span></span>|<span data-ttu-id="393ee-117">Повышение без запроса.</span><span class="sxs-lookup"><span data-stu-id="393ee-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="393ee-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="393ee-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="393ee-119">2</span><span class="sxs-lookup"><span data-stu-id="393ee-119">2</span></span>|<span data-ttu-id="393ee-120">Запрос учетных данных в системе безопасности</span><span class="sxs-lookup"><span data-stu-id="393ee-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="393ee-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="393ee-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="393ee-122">3</span><span class="sxs-lookup"><span data-stu-id="393ee-122">3</span></span>|<span data-ttu-id="393ee-123">Запрос согласия рабочий стол</span><span class="sxs-lookup"><span data-stu-id="393ee-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="393ee-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="393ee-124">promptForCredentials</span></span>|<span data-ttu-id="393ee-125">4</span><span class="sxs-lookup"><span data-stu-id="393ee-125">4</span></span>|<span data-ttu-id="393ee-126">Запрос учетных данных</span><span class="sxs-lookup"><span data-stu-id="393ee-126">Prompt for credentials</span></span>|
|<span data-ttu-id="393ee-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="393ee-127">promptForConsent</span></span>|<span data-ttu-id="393ee-128">5</span><span class="sxs-lookup"><span data-stu-id="393ee-128">5</span></span>|<span data-ttu-id="393ee-129">Запрашивать согласие</span><span class="sxs-lookup"><span data-stu-id="393ee-129">Prompt for consent</span></span>|
|<span data-ttu-id="393ee-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="393ee-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="393ee-131">6</span><span class="sxs-lookup"><span data-stu-id="393ee-131">6</span></span>|<span data-ttu-id="393ee-132">Запрос согласия для двоичных файлов отличных от Windows</span><span class="sxs-lookup"><span data-stu-id="393ee-132">Prompt for consent for non-Windows binaries</span></span>|





