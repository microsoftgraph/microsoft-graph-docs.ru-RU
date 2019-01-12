---
title: Тип перечисления deviceEnrollmentType
description: Возможные способы добавления мобильного устройства для управления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987757"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="807e1-103">Тип перечисления deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="807e1-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="807e1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="807e1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="807e1-105">Возможные способы добавления мобильного устройства для управления.</span><span class="sxs-lookup"><span data-stu-id="807e1-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="807e1-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="807e1-106">Members</span></span>
|<span data-ttu-id="807e1-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="807e1-107">Member</span></span>|<span data-ttu-id="807e1-108">Значение</span><span class="sxs-lookup"><span data-stu-id="807e1-108">Value</span></span>|<span data-ttu-id="807e1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="807e1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="807e1-110">unknown</span><span class="sxs-lookup"><span data-stu-id="807e1-110">unknown</span></span>|<span data-ttu-id="807e1-111">0</span><span class="sxs-lookup"><span data-stu-id="807e1-111">0</span></span>|<span data-ttu-id="807e1-112">Тип регистрации значения по умолчанию не собираются.</span><span class="sxs-lookup"><span data-stu-id="807e1-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="807e1-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="807e1-113">userEnrollment</span></span>|<span data-ttu-id="807e1-114">1</span><span class="sxs-lookup"><span data-stu-id="807e1-114">1</span></span>|<span data-ttu-id="807e1-115">Регистрация управляемых пользователя по каналу BYOD.</span><span class="sxs-lookup"><span data-stu-id="807e1-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="807e1-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="807e1-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="807e1-117">2</span><span class="sxs-lookup"><span data-stu-id="807e1-117">2</span></span>|<span data-ttu-id="807e1-118">Регистрация пользователя с учетной записью диспетчера устройств заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="807e1-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="807e1-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="807e1-119">appleBulkWithUser</span></span>|<span data-ttu-id="807e1-120">3</span><span class="sxs-lookup"><span data-stu-id="807e1-120">3</span></span>|<span data-ttu-id="807e1-121">Регистрация массового Apple с задачей пользователя (DEP, Apple Configurator).</span><span class="sxs-lookup"><span data-stu-id="807e1-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="807e1-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="807e1-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="807e1-123">4</span><span class="sxs-lookup"><span data-stu-id="807e1-123">4</span></span>|<span data-ttu-id="807e1-124">Apple массового заявок через Интернет без запроса пользователя (Config Mobile DEP конфигуратора Apple).</span><span class="sxs-lookup"><span data-stu-id="807e1-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="807e1-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="807e1-125">windowsAzureADJoin</span></span>|<span data-ttu-id="807e1-126">5</span><span class="sxs-lookup"><span data-stu-id="807e1-126">5</span></span>|<span data-ttu-id="807e1-127">Присоединение к Windows Azure AD 10.</span><span class="sxs-lookup"><span data-stu-id="807e1-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="807e1-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="807e1-128">windowsBulkUserless</span></span>|<span data-ttu-id="807e1-129">6</span><span class="sxs-lookup"><span data-stu-id="807e1-129">6</span></span>|<span data-ttu-id="807e1-130">Массовое 10 Windows подачи заявок через ICD с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="807e1-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="807e1-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="807e1-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="807e1-132">7</span><span class="sxs-lookup"><span data-stu-id="807e1-132">7</span></span>|<span data-ttu-id="807e1-133">Windows 10 автоматической подачи заявок.</span><span class="sxs-lookup"><span data-stu-id="807e1-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="807e1-134">(Добавление учетной записи работы)</span><span class="sxs-lookup"><span data-stu-id="807e1-134">(Add work account)</span></span>|
|<span data-ttu-id="807e1-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="807e1-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="807e1-136">8</span><span class="sxs-lookup"><span data-stu-id="807e1-136">8</span></span>|<span data-ttu-id="807e1-137">Windows 10 в пакетном режиме присоединиться к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="807e1-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="807e1-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="807e1-138">windowsCoManagement</span></span>|<span data-ttu-id="807e1-139">9</span><span class="sxs-lookup"><span data-stu-id="807e1-139">9</span></span>|<span data-ttu-id="807e1-140">Windows 10 совместного управления, вызванные автопилот или групповой политики.</span><span class="sxs-lookup"><span data-stu-id="807e1-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



