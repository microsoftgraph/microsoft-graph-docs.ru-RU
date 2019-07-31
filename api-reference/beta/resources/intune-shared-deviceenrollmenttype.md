---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89efb76eb78121937dd2f0558986af0df1750aa9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967471"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="ce808-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="ce808-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="ce808-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce808-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce808-106">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="ce808-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="ce808-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ce808-107">Members</span></span>
|<span data-ttu-id="ce808-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ce808-108">Member</span></span>|<span data-ttu-id="ce808-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ce808-109">Value</span></span>|<span data-ttu-id="ce808-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ce808-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce808-111">unknown</span><span class="sxs-lookup"><span data-stu-id="ce808-111">unknown</span></span>|<span data-ttu-id="ce808-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ce808-112">0</span></span>|<span data-ttu-id="ce808-113">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="ce808-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="ce808-114">Усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="ce808-114">userEnrollment</span></span>|<span data-ttu-id="ce808-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ce808-115">1</span></span>|<span data-ttu-id="ce808-116">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="ce808-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="ce808-117">Девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="ce808-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="ce808-118">2</span><span class="sxs-lookup"><span data-stu-id="ce808-118">2</span></span>|<span data-ttu-id="ce808-119">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="ce808-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="ce808-120">Апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="ce808-120">appleBulkWithUser</span></span>|<span data-ttu-id="ce808-121">4</span><span class="sxs-lookup"><span data-stu-id="ce808-121">3</span></span>|<span data-ttu-id="ce808-122">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce808-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="ce808-123">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="ce808-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="ce808-124">Апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="ce808-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="ce808-125">SP4</span><span class="sxs-lookup"><span data-stu-id="ce808-125">4</span></span>|<span data-ttu-id="ce808-126">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce808-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="ce808-127">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="ce808-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="ce808-128">Виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="ce808-128">windowsAzureADJoin</span></span>|<span data-ttu-id="ce808-129">17:00</span><span class="sxs-lookup"><span data-stu-id="ce808-129">5</span></span>|<span data-ttu-id="ce808-130">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce808-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="ce808-131">Виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="ce808-131">windowsBulkUserless</span></span>|<span data-ttu-id="ce808-132">6 </span><span class="sxs-lookup"><span data-stu-id="ce808-132">6</span></span>|<span data-ttu-id="ce808-133">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="ce808-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="ce808-134">Виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="ce808-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="ce808-135">7 </span><span class="sxs-lookup"><span data-stu-id="ce808-135">7</span></span>|<span data-ttu-id="ce808-136">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ce808-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="ce808-137">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="ce808-137">(Add work account)</span></span>|
|<span data-ttu-id="ce808-138">Виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="ce808-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="ce808-139">8 </span><span class="sxs-lookup"><span data-stu-id="ce808-139">8</span></span>|<span data-ttu-id="ce808-140">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce808-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="ce808-141">Виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="ce808-141">windowsCoManagement</span></span>|<span data-ttu-id="ce808-142">9 </span><span class="sxs-lookup"><span data-stu-id="ce808-142">9</span></span>|<span data-ttu-id="ce808-143">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="ce808-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|





