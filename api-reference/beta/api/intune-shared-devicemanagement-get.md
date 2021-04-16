---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab96b68b12f4d61d8fd71f7795df51faee8bcd20
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865987"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="d7395-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d7395-103">Get deviceManagement</span></span>

<span data-ttu-id="d7395-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7395-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7395-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="d7395-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d7395-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7395-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7395-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7395-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7395-108">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d7395-108">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7395-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d7395-109">Prerequisites</span></span>

<span data-ttu-id="d7395-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7395-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7395-112">Тип &nbsp; разрешения &nbsp; &nbsp; (по рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="d7395-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="d7395-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7395-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="d7395-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7395-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="d7395-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="d7395-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d7395-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="d7395-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d7395-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d7395-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="d7395-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d7395-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d7395-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d7395-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-123">&nbsp;&nbsp; **Намерение устройства**</span><span class="sxs-lookup"><span data-stu-id="d7395-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d7395-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d7395-125">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d7395-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d7395-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d7395-127">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="d7395-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d7395-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-129">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d7395-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d7395-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-131">&nbsp;&nbsp; **Фехтования**</span><span class="sxs-lookup"><span data-stu-id="d7395-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d7395-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-133">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="d7395-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d7395-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="d7395-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="d7395-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-137">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d7395-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d7395-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-139">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d7395-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d7395-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-141">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="d7395-141">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="d7395-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="d7395-143">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="d7395-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d7395-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-145">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="d7395-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d7395-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-147">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="d7395-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="d7395-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-149">&nbsp;&nbsp; **Управление расходами телекома**</span><span class="sxs-lookup"><span data-stu-id="d7395-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d7395-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-151">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d7395-151">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d7395-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d7395-153">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d7395-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d7395-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d7395-155">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7395-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7395-156">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7395-156">Not supported.</span></span>|
| <span data-ttu-id="d7395-157">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d7395-157">Application</span></span> | |
| <span data-ttu-id="d7395-158">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="d7395-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d7395-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-160">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="d7395-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d7395-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="d7395-162">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="d7395-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d7395-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-164">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d7395-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d7395-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-166">&nbsp;&nbsp; **Намерение устройства**</span><span class="sxs-lookup"><span data-stu-id="d7395-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d7395-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d7395-168">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d7395-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d7395-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d7395-170">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="d7395-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d7395-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-172">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d7395-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d7395-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-174">&nbsp;&nbsp; **Фехтования**</span><span class="sxs-lookup"><span data-stu-id="d7395-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d7395-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-176">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="d7395-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d7395-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="d7395-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="d7395-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-180">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d7395-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d7395-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-182">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d7395-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d7395-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-184">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="d7395-184">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="d7395-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="d7395-186">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="d7395-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d7395-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7395-188">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="d7395-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d7395-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-190">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="d7395-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="d7395-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-192">&nbsp;&nbsp; **Управление расходами телекома**</span><span class="sxs-lookup"><span data-stu-id="d7395-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d7395-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="d7395-194">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d7395-194">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d7395-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="d7395-196">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d7395-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d7395-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7395-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7395-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7395-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7395-199">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7395-199">Optional query parameters</span></span>

<span data-ttu-id="d7395-200">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7395-200">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7395-201">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7395-201">Request headers</span></span>
|<span data-ttu-id="d7395-202">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7395-202">Header</span></span>|<span data-ttu-id="d7395-203">Значение</span><span class="sxs-lookup"><span data-stu-id="d7395-203">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7395-204">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7395-204">Authorization</span></span>|<span data-ttu-id="d7395-205">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7395-205">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7395-206">Accept</span><span class="sxs-lookup"><span data-stu-id="d7395-206">Accept</span></span>|<span data-ttu-id="d7395-207">application/json</span><span class="sxs-lookup"><span data-stu-id="d7395-207">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7395-208">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7395-208">Request body</span></span>

<span data-ttu-id="d7395-209">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7395-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7395-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7395-210">Response</span></span>

<span data-ttu-id="d7395-211">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7395-211">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7395-212">Пример</span><span class="sxs-lookup"><span data-stu-id="d7395-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7395-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7395-213">Request</span></span>

<span data-ttu-id="d7395-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7395-214">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="d7395-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7395-215">Response</span></span>

<span data-ttu-id="d7395-216">Вот пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d7395-216">Here are example of the response.</span></span> 

<span data-ttu-id="d7395-217">Примечание. Показанные здесь объекты ответа могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="d7395-217">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="d7395-218">Возвращаются свойства, подходящие для рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="d7395-218">Properties appropriate for the workflow are returned.</span></span>

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










