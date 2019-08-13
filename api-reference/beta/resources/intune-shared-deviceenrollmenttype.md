---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b53d279863ad3e17691b9e4d0397ba5f7d1b408
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372085"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="4d0cb-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="4d0cb-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="4d0cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d0cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d0cb-106">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="4d0cb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4d0cb-107">Members</span></span>
|<span data-ttu-id="4d0cb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4d0cb-108">Member</span></span>|<span data-ttu-id="4d0cb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4d0cb-109">Value</span></span>|<span data-ttu-id="4d0cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4d0cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d0cb-111">unknown</span><span class="sxs-lookup"><span data-stu-id="4d0cb-111">unknown</span></span>|<span data-ttu-id="4d0cb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4d0cb-112">0</span></span>|<span data-ttu-id="4d0cb-113">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="4d0cb-114">усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="4d0cb-114">userEnrollment</span></span>|<span data-ttu-id="4d0cb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4d0cb-115">1</span></span>|<span data-ttu-id="4d0cb-116">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="4d0cb-117">девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="4d0cb-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="4d0cb-118">2</span><span class="sxs-lookup"><span data-stu-id="4d0cb-118">2</span></span>|<span data-ttu-id="4d0cb-119">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="4d0cb-120">апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="4d0cb-120">appleBulkWithUser</span></span>|<span data-ttu-id="4d0cb-121">4</span><span class="sxs-lookup"><span data-stu-id="4d0cb-121">3</span></span>|<span data-ttu-id="4d0cb-122">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="4d0cb-123">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="4d0cb-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="4d0cb-124">апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="4d0cb-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="4d0cb-125">SP4</span><span class="sxs-lookup"><span data-stu-id="4d0cb-125">4</span></span>|<span data-ttu-id="4d0cb-126">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="4d0cb-127">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="4d0cb-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="4d0cb-128">виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="4d0cb-128">windowsAzureADJoin</span></span>|<span data-ttu-id="4d0cb-129">17:00</span><span class="sxs-lookup"><span data-stu-id="4d0cb-129">5</span></span>|<span data-ttu-id="4d0cb-130">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="4d0cb-131">виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="4d0cb-131">windowsBulkUserless</span></span>|<span data-ttu-id="4d0cb-132">6 </span><span class="sxs-lookup"><span data-stu-id="4d0cb-132">6</span></span>|<span data-ttu-id="4d0cb-133">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="4d0cb-134">виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="4d0cb-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="4d0cb-135">7 </span><span class="sxs-lookup"><span data-stu-id="4d0cb-135">7</span></span>|<span data-ttu-id="4d0cb-136">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="4d0cb-137">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="4d0cb-137">(Add work account)</span></span>|
|<span data-ttu-id="4d0cb-138">виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="4d0cb-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="4d0cb-139">8 </span><span class="sxs-lookup"><span data-stu-id="4d0cb-139">8</span></span>|<span data-ttu-id="4d0cb-140">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="4d0cb-141">виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="4d0cb-141">windowsCoManagement</span></span>|<span data-ttu-id="4d0cb-142">9 </span><span class="sxs-lookup"><span data-stu-id="4d0cb-142">9</span></span>|<span data-ttu-id="4d0cb-143">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="4d0cb-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



