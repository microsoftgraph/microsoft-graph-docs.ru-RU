---
title: Тип перечисления localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Возможные значения для LocalSecurityOptionsAdministratorElevationPromptBehavior
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 978436bca4ac0ca281fde61e046e854ba3725c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413761"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="89d23-103">Тип перечисления localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="89d23-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="89d23-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89d23-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="89d23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89d23-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89d23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d23-107">Возможные значения для LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="89d23-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="89d23-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="89d23-108">Members</span></span>
|<span data-ttu-id="89d23-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="89d23-109">Member</span></span>|<span data-ttu-id="89d23-110">Значение</span><span class="sxs-lookup"><span data-stu-id="89d23-110">Value</span></span>|<span data-ttu-id="89d23-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89d23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d23-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="89d23-112">notConfigured</span></span>|<span data-ttu-id="89d23-113">0</span><span class="sxs-lookup"><span data-stu-id="89d23-113">0</span></span>|<span data-ttu-id="89d23-114">Не настроен</span><span class="sxs-lookup"><span data-stu-id="89d23-114">Not Configured</span></span>|
|<span data-ttu-id="89d23-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="89d23-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="89d23-116">1</span><span class="sxs-lookup"><span data-stu-id="89d23-116">1</span></span>|<span data-ttu-id="89d23-117">Повышение без запроса.</span><span class="sxs-lookup"><span data-stu-id="89d23-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="89d23-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="89d23-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="89d23-119">2</span><span class="sxs-lookup"><span data-stu-id="89d23-119">2</span></span>|<span data-ttu-id="89d23-120">Запрос учетных данных в системе безопасности</span><span class="sxs-lookup"><span data-stu-id="89d23-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="89d23-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="89d23-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="89d23-122">3</span><span class="sxs-lookup"><span data-stu-id="89d23-122">3</span></span>|<span data-ttu-id="89d23-123">Запрос согласия рабочий стол</span><span class="sxs-lookup"><span data-stu-id="89d23-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="89d23-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="89d23-124">promptForCredentials</span></span>|<span data-ttu-id="89d23-125">4</span><span class="sxs-lookup"><span data-stu-id="89d23-125">4</span></span>|<span data-ttu-id="89d23-126">Запрос учетных данных</span><span class="sxs-lookup"><span data-stu-id="89d23-126">Prompt for credentials</span></span>|
|<span data-ttu-id="89d23-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="89d23-127">promptForConsent</span></span>|<span data-ttu-id="89d23-128">5</span><span class="sxs-lookup"><span data-stu-id="89d23-128">5</span></span>|<span data-ttu-id="89d23-129">Запрашивать согласие</span><span class="sxs-lookup"><span data-stu-id="89d23-129">Prompt for consent</span></span>|
|<span data-ttu-id="89d23-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="89d23-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="89d23-131">6</span><span class="sxs-lookup"><span data-stu-id="89d23-131">6</span></span>|<span data-ttu-id="89d23-132">Запрос согласия для двоичных файлов отличных от Windows</span><span class="sxs-lookup"><span data-stu-id="89d23-132">Prompt for consent for non-Windows binaries</span></span>|




