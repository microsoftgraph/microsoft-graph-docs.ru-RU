---
title: Тип перечисления deviceEnrollmentType
description: Возможные способы добавления мобильного устройства для управления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399292"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="1a38d-103">Тип перечисления deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1a38d-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="1a38d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a38d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a38d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a38d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a38d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a38d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a38d-107">Возможные способы добавления мобильного устройства для управления.</span><span class="sxs-lookup"><span data-stu-id="1a38d-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="1a38d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1a38d-108">Members</span></span>
|<span data-ttu-id="1a38d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1a38d-109">Member</span></span>|<span data-ttu-id="1a38d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1a38d-110">Value</span></span>|<span data-ttu-id="1a38d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a38d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a38d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1a38d-112">unknown</span></span>|<span data-ttu-id="1a38d-113">0</span><span class="sxs-lookup"><span data-stu-id="1a38d-113">0</span></span>|<span data-ttu-id="1a38d-114">Тип регистрации значения по умолчанию не собираются.</span><span class="sxs-lookup"><span data-stu-id="1a38d-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="1a38d-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="1a38d-115">userEnrollment</span></span>|<span data-ttu-id="1a38d-116">1</span><span class="sxs-lookup"><span data-stu-id="1a38d-116">1</span></span>|<span data-ttu-id="1a38d-117">Регистрация управляемых пользователя по каналу BYOD.</span><span class="sxs-lookup"><span data-stu-id="1a38d-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="1a38d-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="1a38d-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="1a38d-119">2</span><span class="sxs-lookup"><span data-stu-id="1a38d-119">2</span></span>|<span data-ttu-id="1a38d-120">Регистрация пользователя с учетной записью диспетчера устройств заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="1a38d-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="1a38d-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="1a38d-121">appleBulkWithUser</span></span>|<span data-ttu-id="1a38d-122">3</span><span class="sxs-lookup"><span data-stu-id="1a38d-122">3</span></span>|<span data-ttu-id="1a38d-123">Регистрация массового Apple с запрос пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a38d-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="1a38d-124">(DEP конфигуратора Apple)</span><span class="sxs-lookup"><span data-stu-id="1a38d-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="1a38d-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="1a38d-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="1a38d-126">4</span><span class="sxs-lookup"><span data-stu-id="1a38d-126">4</span></span>|<span data-ttu-id="1a38d-127">Apple массового заявок через Интернет без запроса пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a38d-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="1a38d-128">(DEP конфигуратора Apple мобильных Config)</span><span class="sxs-lookup"><span data-stu-id="1a38d-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="1a38d-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="1a38d-129">windowsAzureADJoin</span></span>|<span data-ttu-id="1a38d-130">5</span><span class="sxs-lookup"><span data-stu-id="1a38d-130">5</span></span>|<span data-ttu-id="1a38d-131">Присоединение к Windows Azure AD 10.</span><span class="sxs-lookup"><span data-stu-id="1a38d-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="1a38d-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="1a38d-132">windowsBulkUserless</span></span>|<span data-ttu-id="1a38d-133">6</span><span class="sxs-lookup"><span data-stu-id="1a38d-133">6</span></span>|<span data-ttu-id="1a38d-134">Массовое 10 Windows подачи заявок через ICD с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="1a38d-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="1a38d-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="1a38d-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="1a38d-136">7</span><span class="sxs-lookup"><span data-stu-id="1a38d-136">7</span></span>|<span data-ttu-id="1a38d-137">Windows 10 автоматической подачи заявок.</span><span class="sxs-lookup"><span data-stu-id="1a38d-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="1a38d-138">(Добавление учетной записи работы)</span><span class="sxs-lookup"><span data-stu-id="1a38d-138">(Add work account)</span></span>|
|<span data-ttu-id="1a38d-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="1a38d-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="1a38d-140">8</span><span class="sxs-lookup"><span data-stu-id="1a38d-140">8</span></span>|<span data-ttu-id="1a38d-141">Windows 10 в пакетном режиме присоединиться к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a38d-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="1a38d-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="1a38d-142">windowsCoManagement</span></span>|<span data-ttu-id="1a38d-143">9</span><span class="sxs-lookup"><span data-stu-id="1a38d-143">9</span></span>|<span data-ttu-id="1a38d-144">10 совместного управления Windows активировать по автопилот или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="1a38d-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




