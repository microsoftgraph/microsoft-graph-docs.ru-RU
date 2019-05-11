---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9c5c5fbdd68af1c78e55fc023a8c85642928889
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940017"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="1e21c-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="1e21c-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="1e21c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e21c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e21c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e21c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e21c-106">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="1e21c-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="1e21c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1e21c-107">Members</span></span>
|<span data-ttu-id="1e21c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1e21c-108">Member</span></span>|<span data-ttu-id="1e21c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1e21c-109">Value</span></span>|<span data-ttu-id="1e21c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1e21c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e21c-111">unknown</span><span class="sxs-lookup"><span data-stu-id="1e21c-111">unknown</span></span>|<span data-ttu-id="1e21c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1e21c-112">0</span></span>|<span data-ttu-id="1e21c-113">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="1e21c-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="1e21c-114">Усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="1e21c-114">userEnrollment</span></span>|<span data-ttu-id="1e21c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1e21c-115">1</span></span>|<span data-ttu-id="1e21c-116">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="1e21c-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="1e21c-117">Девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="1e21c-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="1e21c-118">2</span><span class="sxs-lookup"><span data-stu-id="1e21c-118">2</span></span>|<span data-ttu-id="1e21c-119">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="1e21c-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="1e21c-120">Апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="1e21c-120">appleBulkWithUser</span></span>|<span data-ttu-id="1e21c-121">4</span><span class="sxs-lookup"><span data-stu-id="1e21c-121">3</span></span>|<span data-ttu-id="1e21c-122">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e21c-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="1e21c-123">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="1e21c-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="1e21c-124">Апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="1e21c-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="1e21c-125">SP4</span><span class="sxs-lookup"><span data-stu-id="1e21c-125">4</span></span>|<span data-ttu-id="1e21c-126">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e21c-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="1e21c-127">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="1e21c-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="1e21c-128">Виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="1e21c-128">windowsAzureADJoin</span></span>|<span data-ttu-id="1e21c-129">17:00</span><span class="sxs-lookup"><span data-stu-id="1e21c-129">5</span></span>|<span data-ttu-id="1e21c-130">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e21c-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="1e21c-131">Виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="1e21c-131">windowsBulkUserless</span></span>|<span data-ttu-id="1e21c-132">6 </span><span class="sxs-lookup"><span data-stu-id="1e21c-132">6</span></span>|<span data-ttu-id="1e21c-133">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="1e21c-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="1e21c-134">Виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="1e21c-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="1e21c-135">7 </span><span class="sxs-lookup"><span data-stu-id="1e21c-135">7</span></span>|<span data-ttu-id="1e21c-136">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1e21c-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="1e21c-137">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="1e21c-137">(Add work account)</span></span>|
|<span data-ttu-id="1e21c-138">Виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="1e21c-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="1e21c-139">8 </span><span class="sxs-lookup"><span data-stu-id="1e21c-139">8</span></span>|<span data-ttu-id="1e21c-140">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e21c-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="1e21c-141">Виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="1e21c-141">windowsCoManagement</span></span>|<span data-ttu-id="1e21c-142">9 </span><span class="sxs-lookup"><span data-stu-id="1e21c-142">9</span></span>|<span data-ttu-id="1e21c-143">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="1e21c-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




