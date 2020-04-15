---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 433abdb308b838980149e7bf35784159328c6d8d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387243"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="e92fc-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="e92fc-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="e92fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e92fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e92fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e92fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e92fc-106">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="e92fc-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="e92fc-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e92fc-107">Members</span></span>
|<span data-ttu-id="e92fc-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e92fc-108">Member</span></span>|<span data-ttu-id="e92fc-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e92fc-109">Value</span></span>|<span data-ttu-id="e92fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e92fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e92fc-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e92fc-111">unknown</span></span>|<span data-ttu-id="e92fc-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e92fc-112">0</span></span>|<span data-ttu-id="e92fc-113">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="e92fc-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="e92fc-114">усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="e92fc-114">userEnrollment</span></span>|<span data-ttu-id="e92fc-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e92fc-115">1</span></span>|<span data-ttu-id="e92fc-116">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="e92fc-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="e92fc-117">девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="e92fc-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="e92fc-118">2</span><span class="sxs-lookup"><span data-stu-id="e92fc-118">2</span></span>|<span data-ttu-id="e92fc-119">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="e92fc-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="e92fc-120">апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="e92fc-120">appleBulkWithUser</span></span>|<span data-ttu-id="e92fc-121">4</span><span class="sxs-lookup"><span data-stu-id="e92fc-121">3</span></span>|<span data-ttu-id="e92fc-122">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="e92fc-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="e92fc-123">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="e92fc-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="e92fc-124">апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="e92fc-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="e92fc-125">4 </span><span class="sxs-lookup"><span data-stu-id="e92fc-125">4</span></span>|<span data-ttu-id="e92fc-126">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="e92fc-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="e92fc-127">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="e92fc-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="e92fc-128">виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="e92fc-128">windowsAzureADJoin</span></span>|<span data-ttu-id="e92fc-129">5 </span><span class="sxs-lookup"><span data-stu-id="e92fc-129">5</span></span>|<span data-ttu-id="e92fc-130">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e92fc-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="e92fc-131">виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="e92fc-131">windowsBulkUserless</span></span>|<span data-ttu-id="e92fc-132">6 </span><span class="sxs-lookup"><span data-stu-id="e92fc-132">6</span></span>|<span data-ttu-id="e92fc-133">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="e92fc-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="e92fc-134">виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="e92fc-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="e92fc-135">7 </span><span class="sxs-lookup"><span data-stu-id="e92fc-135">7</span></span>|<span data-ttu-id="e92fc-136">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e92fc-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="e92fc-137">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="e92fc-137">(Add work account)</span></span>|
|<span data-ttu-id="e92fc-138">виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="e92fc-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="e92fc-139">8 </span><span class="sxs-lookup"><span data-stu-id="e92fc-139">8</span></span>|<span data-ttu-id="e92fc-140">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e92fc-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="e92fc-141">виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="e92fc-141">windowsCoManagement</span></span>|<span data-ttu-id="e92fc-142">9 </span><span class="sxs-lookup"><span data-stu-id="e92fc-142">9</span></span>|<span data-ttu-id="e92fc-143">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="e92fc-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|







