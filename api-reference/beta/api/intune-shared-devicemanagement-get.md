---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 248ed14156ae8c24f70b4ecd0ce1f643d55503db
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194658"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="d5c14-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d5c14-103">Get deviceManagement</span></span>

> <span data-ttu-id="d5c14-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d5c14-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5c14-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5c14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c14-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5c14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5c14-107">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d5c14-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5c14-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5c14-108">Prerequisites</span></span>

<span data-ttu-id="d5c14-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5c14-111">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="d5c14-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="d5c14-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5c14-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="d5c14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5c14-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="d5c14-114">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="d5c14-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d5c14-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-116">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="d5c14-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d5c14-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d5c14-118">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="d5c14-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d5c14-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="d5c14-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d5c14-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-122">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="d5c14-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d5c14-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d5c14-124">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d5c14-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d5c14-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d5c14-126">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="d5c14-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d5c14-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-128">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d5c14-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d5c14-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-130">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="d5c14-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d5c14-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-132">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="d5c14-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d5c14-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-134">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="d5c14-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="d5c14-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-136">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="d5c14-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d5c14-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-138">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d5c14-138">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d5c14-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-140">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="d5c14-140">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="d5c14-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="d5c14-142">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="d5c14-142">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d5c14-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-144">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="d5c14-144">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d5c14-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-146">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="d5c14-146">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="d5c14-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-148">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="d5c14-148">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d5c14-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-150">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d5c14-150">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d5c14-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d5c14-152">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d5c14-152">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d5c14-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d5c14-154">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5c14-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c14-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5c14-155">Not supported.</span></span>|
| <span data-ttu-id="d5c14-156">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5c14-156">Application</span></span> | |
| <span data-ttu-id="d5c14-157">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="d5c14-157">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d5c14-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-159">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="d5c14-159">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d5c14-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d5c14-161">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="d5c14-161">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d5c14-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-163">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="d5c14-163">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d5c14-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-165">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="d5c14-165">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d5c14-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d5c14-167">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d5c14-167">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d5c14-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d5c14-169">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="d5c14-169">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d5c14-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-171">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d5c14-171">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d5c14-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-173">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="d5c14-173">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d5c14-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-175">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="d5c14-175">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d5c14-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-177">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="d5c14-177">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="d5c14-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-179">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="d5c14-179">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d5c14-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-181">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d5c14-181">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d5c14-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-183">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="d5c14-183">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="d5c14-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="d5c14-185">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="d5c14-185">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d5c14-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d5c14-187">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="d5c14-187">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d5c14-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-189">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="d5c14-189">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="d5c14-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-191">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="d5c14-191">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d5c14-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d5c14-193">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d5c14-193">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d5c14-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d5c14-195">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d5c14-195">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d5c14-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c14-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5c14-197">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5c14-197">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5c14-198">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d5c14-198">Optional query parameters</span></span>

<span data-ttu-id="d5c14-199">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d5c14-199">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5c14-200">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5c14-200">Request headers</span></span>
|<span data-ttu-id="d5c14-201">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5c14-201">Header</span></span>|<span data-ttu-id="d5c14-202">Значение</span><span class="sxs-lookup"><span data-stu-id="d5c14-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c14-203">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5c14-203">Authorization</span></span>|<span data-ttu-id="d5c14-204">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5c14-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c14-205">Accept</span><span class="sxs-lookup"><span data-stu-id="d5c14-205">Accept</span></span>|<span data-ttu-id="d5c14-206">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c14-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c14-207">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5c14-207">Request body</span></span>

<span data-ttu-id="d5c14-208">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5c14-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c14-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5c14-209">Response</span></span>

<span data-ttu-id="d5c14-210">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5c14-210">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c14-211">Пример</span><span class="sxs-lookup"><span data-stu-id="d5c14-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5c14-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5c14-212">Request</span></span>

<span data-ttu-id="d5c14-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5c14-213">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="d5c14-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5c14-214">Response</span></span>

<span data-ttu-id="d5c14-215">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5c14-215">Here are example of the response.</span></span> 

<span data-ttu-id="d5c14-216">Note: объекты ответа, показанные здесь, могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="d5c14-216">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="d5c14-217">Возвращаются свойства, подходящие для рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="d5c14-217">Properties appropriate for the workflow are returned.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```







