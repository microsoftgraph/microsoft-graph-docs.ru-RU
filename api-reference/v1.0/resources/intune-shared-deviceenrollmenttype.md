---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae60fd6657cf902eb5bdd0f919d446527b00d9a9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368276"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="16a93-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="16a93-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="16a93-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16a93-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16a93-105">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="16a93-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="16a93-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="16a93-106">Members</span></span>
|<span data-ttu-id="16a93-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="16a93-107">Member</span></span>|<span data-ttu-id="16a93-108">Значение</span><span class="sxs-lookup"><span data-stu-id="16a93-108">Value</span></span>|<span data-ttu-id="16a93-109">Описание</span><span class="sxs-lookup"><span data-stu-id="16a93-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16a93-110">unknown</span><span class="sxs-lookup"><span data-stu-id="16a93-110">unknown</span></span>|<span data-ttu-id="16a93-111">нуль</span><span class="sxs-lookup"><span data-stu-id="16a93-111">0</span></span>|<span data-ttu-id="16a93-112">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="16a93-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="16a93-113">усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="16a93-113">userEnrollment</span></span>|<span data-ttu-id="16a93-114">1,1</span><span class="sxs-lookup"><span data-stu-id="16a93-114">1</span></span>|<span data-ttu-id="16a93-115">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="16a93-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="16a93-116">девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="16a93-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="16a93-117">2</span><span class="sxs-lookup"><span data-stu-id="16a93-117">2</span></span>|<span data-ttu-id="16a93-118">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="16a93-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="16a93-119">апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="16a93-119">appleBulkWithUser</span></span>|<span data-ttu-id="16a93-120">4</span><span class="sxs-lookup"><span data-stu-id="16a93-120">3</span></span>|<span data-ttu-id="16a93-121">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="16a93-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="16a93-122">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="16a93-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="16a93-123">апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="16a93-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="16a93-124">SP4</span><span class="sxs-lookup"><span data-stu-id="16a93-124">4</span></span>|<span data-ttu-id="16a93-125">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="16a93-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="16a93-126">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="16a93-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="16a93-127">виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="16a93-127">windowsAzureADJoin</span></span>|<span data-ttu-id="16a93-128">17:00</span><span class="sxs-lookup"><span data-stu-id="16a93-128">5</span></span>|<span data-ttu-id="16a93-129">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="16a93-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="16a93-130">виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="16a93-130">windowsBulkUserless</span></span>|<span data-ttu-id="16a93-131">6 </span><span class="sxs-lookup"><span data-stu-id="16a93-131">6</span></span>|<span data-ttu-id="16a93-132">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="16a93-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="16a93-133">виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="16a93-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="16a93-134">7 </span><span class="sxs-lookup"><span data-stu-id="16a93-134">7</span></span>|<span data-ttu-id="16a93-135">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="16a93-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="16a93-136">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="16a93-136">(Add work account)</span></span>|
|<span data-ttu-id="16a93-137">виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="16a93-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="16a93-138">8 </span><span class="sxs-lookup"><span data-stu-id="16a93-138">8</span></span>|<span data-ttu-id="16a93-139">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="16a93-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="16a93-140">виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="16a93-140">windowsCoManagement</span></span>|<span data-ttu-id="16a93-141">9 </span><span class="sxs-lookup"><span data-stu-id="16a93-141">9</span></span>|<span data-ttu-id="16a93-142">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="16a93-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




