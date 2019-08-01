---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: afb007893ac0b41d4439635ed78b528058d41364
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036962"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="a1ab2-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="a1ab2-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="a1ab2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1ab2-105">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="a1ab2-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a1ab2-106">Members</span></span>
|<span data-ttu-id="a1ab2-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a1ab2-107">Member</span></span>|<span data-ttu-id="a1ab2-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a1ab2-108">Value</span></span>|<span data-ttu-id="a1ab2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ab2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ab2-110">unknown</span><span class="sxs-lookup"><span data-stu-id="a1ab2-110">unknown</span></span>|<span data-ttu-id="a1ab2-111">нуль</span><span class="sxs-lookup"><span data-stu-id="a1ab2-111">0</span></span>|<span data-ttu-id="a1ab2-112">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="a1ab2-113">Усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="a1ab2-113">userEnrollment</span></span>|<span data-ttu-id="a1ab2-114">1,1</span><span class="sxs-lookup"><span data-stu-id="a1ab2-114">1</span></span>|<span data-ttu-id="a1ab2-115">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="a1ab2-116">Девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="a1ab2-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="a1ab2-117">2</span><span class="sxs-lookup"><span data-stu-id="a1ab2-117">2</span></span>|<span data-ttu-id="a1ab2-118">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="a1ab2-119">Апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="a1ab2-119">appleBulkWithUser</span></span>|<span data-ttu-id="a1ab2-120">4</span><span class="sxs-lookup"><span data-stu-id="a1ab2-120">3</span></span>|<span data-ttu-id="a1ab2-121">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="a1ab2-122">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="a1ab2-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="a1ab2-123">Апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="a1ab2-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="a1ab2-124">SP4</span><span class="sxs-lookup"><span data-stu-id="a1ab2-124">4</span></span>|<span data-ttu-id="a1ab2-125">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="a1ab2-126">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="a1ab2-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="a1ab2-127">Виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="a1ab2-127">windowsAzureADJoin</span></span>|<span data-ttu-id="a1ab2-128">17:00</span><span class="sxs-lookup"><span data-stu-id="a1ab2-128">5</span></span>|<span data-ttu-id="a1ab2-129">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="a1ab2-130">Виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="a1ab2-130">windowsBulkUserless</span></span>|<span data-ttu-id="a1ab2-131">6 </span><span class="sxs-lookup"><span data-stu-id="a1ab2-131">6</span></span>|<span data-ttu-id="a1ab2-132">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="a1ab2-133">Виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="a1ab2-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="a1ab2-134">7 </span><span class="sxs-lookup"><span data-stu-id="a1ab2-134">7</span></span>|<span data-ttu-id="a1ab2-135">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="a1ab2-136">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="a1ab2-136">(Add work account)</span></span>|
|<span data-ttu-id="a1ab2-137">Виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="a1ab2-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="a1ab2-138">8 </span><span class="sxs-lookup"><span data-stu-id="a1ab2-138">8</span></span>|<span data-ttu-id="a1ab2-139">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="a1ab2-140">Виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="a1ab2-140">windowsCoManagement</span></span>|<span data-ttu-id="a1ab2-141">9 </span><span class="sxs-lookup"><span data-stu-id="a1ab2-141">9</span></span>|<span data-ttu-id="a1ab2-142">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a1ab2-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



