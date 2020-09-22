---
title: тип перечисления Девицеенроллменттипе
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f0e309126d48646fb67446270353566be23ec9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059105"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="d3570-103">тип перечисления Девицеенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="d3570-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="d3570-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3570-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3570-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3570-106">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="d3570-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="d3570-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d3570-107">Members</span></span>
|<span data-ttu-id="d3570-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d3570-108">Member</span></span>|<span data-ttu-id="d3570-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d3570-109">Value</span></span>|<span data-ttu-id="d3570-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3570-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3570-111">unknown</span><span class="sxs-lookup"><span data-stu-id="d3570-111">unknown</span></span>|<span data-ttu-id="d3570-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d3570-112">0</span></span>|<span data-ttu-id="d3570-113">Значение по умолчанию: тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="d3570-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="d3570-114">усеренроллмент</span><span class="sxs-lookup"><span data-stu-id="d3570-114">userEnrollment</span></span>|<span data-ttu-id="d3570-115">1 </span><span class="sxs-lookup"><span data-stu-id="d3570-115">1</span></span>|<span data-ttu-id="d3570-116">Управляемая пользователями регистрация через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="d3570-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="d3570-117">девицеенроллментманажер</span><span class="sxs-lookup"><span data-stu-id="d3570-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="d3570-118">2 </span><span class="sxs-lookup"><span data-stu-id="d3570-118">2</span></span>|<span data-ttu-id="d3570-119">Регистрация пользователей с помощью учетной записи менеджера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="d3570-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="d3570-120">апплебулквисусер</span><span class="sxs-lookup"><span data-stu-id="d3570-120">appleBulkWithUser</span></span>|<span data-ttu-id="d3570-121">4</span><span class="sxs-lookup"><span data-stu-id="d3570-121">3</span></span>|<span data-ttu-id="d3570-122">Массовая регистрация Apple с задачей пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3570-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="d3570-123">(Предотвращение выполнения данных, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="d3570-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="d3570-124">апплебулквисаутусер</span><span class="sxs-lookup"><span data-stu-id="d3570-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="d3570-125">4 </span><span class="sxs-lookup"><span data-stu-id="d3570-125">4</span></span>|<span data-ttu-id="d3570-126">Массовая регистрация Apple без задачи пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3570-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="d3570-127">(Предотвращение выполнения данных, Apple Configurator, Mobile config)</span><span class="sxs-lookup"><span data-stu-id="d3570-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="d3570-128">виндовсазуреаджоин</span><span class="sxs-lookup"><span data-stu-id="d3570-128">windowsAzureADJoin</span></span>|<span data-ttu-id="d3570-129">5 </span><span class="sxs-lookup"><span data-stu-id="d3570-129">5</span></span>|<span data-ttu-id="d3570-130">Присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d3570-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="d3570-131">виндовсбулкусерлесс</span><span class="sxs-lookup"><span data-stu-id="d3570-131">windowsBulkUserless</span></span>|<span data-ttu-id="d3570-132">6 </span><span class="sxs-lookup"><span data-stu-id="d3570-132">6</span></span>|<span data-ttu-id="d3570-133">Массовая регистрация Windows 10 с помощью ICD с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="d3570-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="d3570-134">виндовсаутоенроллмент</span><span class="sxs-lookup"><span data-stu-id="d3570-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="d3570-135">7 </span><span class="sxs-lookup"><span data-stu-id="d3570-135">7</span></span>|<span data-ttu-id="d3570-136">Автоматическая регистрация в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d3570-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="d3570-137">(Добавление рабочей учетной записи)</span><span class="sxs-lookup"><span data-stu-id="d3570-137">(Add work account)</span></span>|
|<span data-ttu-id="d3570-138">виндовсбулказуредомаинжоин</span><span class="sxs-lookup"><span data-stu-id="d3570-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="d3570-139">8 </span><span class="sxs-lookup"><span data-stu-id="d3570-139">8</span></span>|<span data-ttu-id="d3570-140">Массовый присоединение к Windows 10 Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d3570-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="d3570-141">виндовскоманажемент</span><span class="sxs-lookup"><span data-stu-id="d3570-141">windowsCoManagement</span></span>|<span data-ttu-id="d3570-142">9 </span><span class="sxs-lookup"><span data-stu-id="d3570-142">9</span></span>|<span data-ttu-id="d3570-143">Управление с помощью Windows 10 инициировано с помощью автопилота или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="d3570-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|









