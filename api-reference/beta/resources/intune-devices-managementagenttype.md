---
title: Тип перечисления managementAgentType
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1711ad647afabc2b8877bd2f99b049bd1c1dd4e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914285"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="49472-103">Тип перечисления managementAgentType</span><span class="sxs-lookup"><span data-stu-id="49472-103">managementAgentType enum type</span></span>

> <span data-ttu-id="49472-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49472-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49472-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49472-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49472-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49472-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49472-107">Тип агента управления.</span><span class="sxs-lookup"><span data-stu-id="49472-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="49472-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="49472-108">Members</span></span>
|<span data-ttu-id="49472-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="49472-109">Member</span></span>|<span data-ttu-id="49472-110">Значение</span><span class="sxs-lookup"><span data-stu-id="49472-110">Value</span></span>|<span data-ttu-id="49472-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49472-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49472-112">EAS</span><span class="sxs-lookup"><span data-stu-id="49472-112">eas</span></span>|<span data-ttu-id="49472-113">1</span><span class="sxs-lookup"><span data-stu-id="49472-113">1</span></span>|<span data-ttu-id="49472-114">Устройство управляется сервером Exchange server.</span><span class="sxs-lookup"><span data-stu-id="49472-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="49472-115">MDM</span><span class="sxs-lookup"><span data-stu-id="49472-115">mdm</span></span>|<span data-ttu-id="49472-116">2</span><span class="sxs-lookup"><span data-stu-id="49472-116">2</span></span>|<span data-ttu-id="49472-117">Устройство является управляемым путем MDM. Intune</span><span class="sxs-lookup"><span data-stu-id="49472-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="49472-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="49472-118">easMdm</span></span>|<span data-ttu-id="49472-119">3</span><span class="sxs-lookup"><span data-stu-id="49472-119">3</span></span>|<span data-ttu-id="49472-120">Устройство управляется сервером Exchange server и Intune MDM.</span><span class="sxs-lookup"><span data-stu-id="49472-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="49472-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="49472-121">intuneClient</span></span>|<span data-ttu-id="49472-122">4</span><span class="sxs-lookup"><span data-stu-id="49472-122">4</span></span>|<span data-ttu-id="49472-123">Управляемые клиентами Intune.</span><span class="sxs-lookup"><span data-stu-id="49472-123">Intune client managed.</span></span>|
|<span data-ttu-id="49472-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="49472-124">easIntuneClient</span></span>|<span data-ttu-id="49472-125">5</span><span class="sxs-lookup"><span data-stu-id="49472-125">5</span></span>|<span data-ttu-id="49472-126">Устройство является EAS и Intune двойной управляемые клиентами.</span><span class="sxs-lookup"><span data-stu-id="49472-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="49472-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="49472-127">configurationManagerClient</span></span>|<span data-ttu-id="49472-128">8</span><span class="sxs-lookup"><span data-stu-id="49472-128">8</span></span>|<span data-ttu-id="49472-129">Устройство является управляемым, диспетчер конфигураций.</span><span class="sxs-lookup"><span data-stu-id="49472-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="49472-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="49472-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="49472-131">10</span><span class="sxs-lookup"><span data-stu-id="49472-131">10</span></span>|<span data-ttu-id="49472-132">Устройство управляется Configuration Manager и MDM.</span><span class="sxs-lookup"><span data-stu-id="49472-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="49472-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="49472-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="49472-134">11</span><span class="sxs-lookup"><span data-stu-id="49472-134">11</span></span>|<span data-ttu-id="49472-135">Устройство является управляемым, диспетчер конфигураций, MDM и Eas.</span><span class="sxs-lookup"><span data-stu-id="49472-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="49472-136">unknown</span><span class="sxs-lookup"><span data-stu-id="49472-136">unknown</span></span>|<span data-ttu-id="49472-137">16</span><span class="sxs-lookup"><span data-stu-id="49472-137">16</span></span>|<span data-ttu-id="49472-138">Тип агента управления UNKNOWN.</span><span class="sxs-lookup"><span data-stu-id="49472-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="49472-139">jamf</span><span class="sxs-lookup"><span data-stu-id="49472-139">jamf</span></span>|<span data-ttu-id="49472-140">32</span><span class="sxs-lookup"><span data-stu-id="49472-140">32</span></span>|<span data-ttu-id="49472-141">Атрибуты устройства полученные от Jamf.</span><span class="sxs-lookup"><span data-stu-id="49472-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="49472-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="49472-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="49472-143">64</span><span class="sxs-lookup"><span data-stu-id="49472-143">64</span></span>|<span data-ttu-id="49472-144">Устройство управляется CloudDPC компании Google.</span><span class="sxs-lookup"><span data-stu-id="49472-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="49472-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="49472-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="49472-146">258</span><span class="sxs-lookup"><span data-stu-id="49472-146">258</span></span>|<span data-ttu-id="49472-147">Это устройство управляется Microsoft 365 через Intune.</span><span class="sxs-lookup"><span data-stu-id="49472-147">This device is managed by Microsoft 365 through Intune.</span></span>|





