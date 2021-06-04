---
title: тип enum deviceEnrollmentType
description: Возможные способы добавления мобильного устройства в управление.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f0e309126d48646fb67446270353566be23ec9a
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732757"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="bb5f0-103">тип enum deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bb5f0-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="bb5f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb5f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb5f0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb5f0-106">Возможные способы добавления мобильного устройства в управление.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="bb5f0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bb5f0-107">Members</span></span>
|<span data-ttu-id="bb5f0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bb5f0-108">Member</span></span>|<span data-ttu-id="bb5f0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bb5f0-109">Value</span></span>|<span data-ttu-id="bb5f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb5f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb5f0-111">unknown</span><span class="sxs-lookup"><span data-stu-id="bb5f0-111">unknown</span></span>|<span data-ttu-id="bb5f0-112">0</span><span class="sxs-lookup"><span data-stu-id="bb5f0-112">0</span></span>|<span data-ttu-id="bb5f0-113">Значение по умолчанию, тип регистрации не был собран.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="bb5f0-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="bb5f0-114">userEnrollment</span></span>|<span data-ttu-id="bb5f0-115">1</span><span class="sxs-lookup"><span data-stu-id="bb5f0-115">1</span></span>|<span data-ttu-id="bb5f0-116">Регистрация по инициативе пользователя через канал BYOD.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="bb5f0-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="bb5f0-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="bb5f0-118">2</span><span class="sxs-lookup"><span data-stu-id="bb5f0-118">2</span></span>|<span data-ttu-id="bb5f0-119">Регистрация пользователей с учетной записью диспетчера регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="bb5f0-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="bb5f0-120">appleBulkWithUser</span></span>|<span data-ttu-id="bb5f0-121">3</span><span class="sxs-lookup"><span data-stu-id="bb5f0-121">3</span></span>|<span data-ttu-id="bb5f0-122">Массовое зачисление Apple с проблемой пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="bb5f0-123">(DEP, настраиваемый Apple)</span><span class="sxs-lookup"><span data-stu-id="bb5f0-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="bb5f0-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="bb5f0-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="bb5f0-125">4 </span><span class="sxs-lookup"><span data-stu-id="bb5f0-125">4</span></span>|<span data-ttu-id="bb5f0-126">Массовое зачисление Apple без проблем пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="bb5f0-127">(DEP, Apple Configurator, Mobile Config)</span><span class="sxs-lookup"><span data-stu-id="bb5f0-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="bb5f0-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="bb5f0-128">windowsAzureADJoin</span></span>|<span data-ttu-id="bb5f0-129">5 </span><span class="sxs-lookup"><span data-stu-id="bb5f0-129">5</span></span>|<span data-ttu-id="bb5f0-130">Windows 10 Присоединиться к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="bb5f0-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="bb5f0-131">windowsBulkUserless</span></span>|<span data-ttu-id="bb5f0-132">6 </span><span class="sxs-lookup"><span data-stu-id="bb5f0-132">6</span></span>|<span data-ttu-id="bb5f0-133">Windows 10 Массовая регистрация через ICD с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="bb5f0-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="bb5f0-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="bb5f0-135">7 </span><span class="sxs-lookup"><span data-stu-id="bb5f0-135">7</span></span>|<span data-ttu-id="bb5f0-136">Windows 10 автоматической регистрации.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="bb5f0-137">(Добавление учетной записи работы)</span><span class="sxs-lookup"><span data-stu-id="bb5f0-137">(Add work account)</span></span>|
|<span data-ttu-id="bb5f0-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="bb5f0-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="bb5f0-139">8 </span><span class="sxs-lookup"><span data-stu-id="bb5f0-139">8</span></span>|<span data-ttu-id="bb5f0-140">Windows 10 Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="bb5f0-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="bb5f0-141">windowsCoManagement</span></span>|<span data-ttu-id="bb5f0-142">9 </span><span class="sxs-lookup"><span data-stu-id="bb5f0-142">9</span></span>|<span data-ttu-id="bb5f0-143">Windows 10 Co-Management с помощью autoPilot или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="bb5f0-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|









