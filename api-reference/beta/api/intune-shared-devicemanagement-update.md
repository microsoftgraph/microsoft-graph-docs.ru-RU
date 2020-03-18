---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0aecca341cef5b88794f20a9d037b340c33bf97b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801035"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="2f361-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f361-103">Update deviceManagement</span></span>

> <span data-ttu-id="2f361-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f361-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f361-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f361-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f361-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f361-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2f361-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f361-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f361-108">Prerequisites</span></span>

<span data-ttu-id="2f361-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f361-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2f361-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="2f361-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="2f361-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="2f361-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="2f361-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f361-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="2f361-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f361-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="2f361-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="2f361-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="2f361-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="2f361-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="2f361-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="2f361-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="2f361-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="2f361-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="2f361-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2f361-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-123">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="2f361-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="2f361-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2f361-125">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2f361-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2f361-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-127">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="2f361-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="2f361-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-129">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="2f361-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="2f361-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-131">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="2f361-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="2f361-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-133">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="2f361-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="2f361-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-135">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="2f361-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="2f361-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-137">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2f361-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2f361-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-139">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2f361-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2f361-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-141">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2f361-141">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2f361-142">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-142">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-143">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="2f361-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="2f361-144">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f361-144">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="2f361-145">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="2f361-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="2f361-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-147">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="2f361-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="2f361-148">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-148">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-149">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="2f361-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="2f361-150">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-150">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-151">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="2f361-151">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="2f361-152">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-152">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-153">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="2f361-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="2f361-154">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-154">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-155">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f361-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f361-156">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f361-156">Not supported.</span></span>|
| <span data-ttu-id="2f361-157">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f361-157">Application</span></span> ||
| <span data-ttu-id="2f361-158">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="2f361-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="2f361-159">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-159">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="2f361-160">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="2f361-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="2f361-161">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-161">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-162">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="2f361-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="2f361-163">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-163">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-164">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="2f361-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2f361-165">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-165">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-166">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="2f361-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="2f361-167">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-167">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2f361-168">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2f361-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2f361-169">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-169">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-170">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="2f361-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="2f361-171">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-171">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-172">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="2f361-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="2f361-173">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-173">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-174">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="2f361-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="2f361-175">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-175">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-176">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="2f361-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="2f361-177">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-177">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-178">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="2f361-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="2f361-179">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-179">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-180">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2f361-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2f361-181">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-181">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-182">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2f361-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2f361-183">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-183">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-184">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2f361-184">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2f361-185">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-185">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-186">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="2f361-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="2f361-187">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f361-187">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="2f361-188">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="2f361-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="2f361-189">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-189">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-190">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="2f361-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="2f361-191">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-191">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-192">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="2f361-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="2f361-193">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-193">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-194">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="2f361-194">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="2f361-195">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-195">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2f361-196">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="2f361-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="2f361-197">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f361-197">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f361-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f361-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="2f361-199">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f361-199">Request headers</span></span>

|<span data-ttu-id="2f361-200">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f361-200">Header</span></span>|<span data-ttu-id="2f361-201">Значение</span><span class="sxs-lookup"><span data-stu-id="2f361-201">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f361-202">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f361-202">Authorization</span></span>|<span data-ttu-id="2f361-203">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f361-203">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f361-204">Accept</span><span class="sxs-lookup"><span data-stu-id="2f361-204">Accept</span></span>|<span data-ttu-id="2f361-205">application/json</span><span class="sxs-lookup"><span data-stu-id="2f361-205">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f361-206">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f361-206">Request body</span></span>

<span data-ttu-id="2f361-207">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f361-207">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="2f361-208">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2f361-208">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="2f361-209">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f361-209">Property</span></span>|<span data-ttu-id="2f361-210">Тип</span><span class="sxs-lookup"><span data-stu-id="2f361-210">Type</span></span>|<span data-ttu-id="2f361-211">Описание</span><span class="sxs-lookup"><span data-stu-id="2f361-211">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f361-212">id</span><span class="sxs-lookup"><span data-stu-id="2f361-212">id</span></span>|<span data-ttu-id="2f361-213">String</span><span class="sxs-lookup"><span data-stu-id="2f361-213">String</span></span>|<span data-ttu-id="2f361-214">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="2f361-214">Unique identifier for the device.</span></span>|
|<span data-ttu-id="2f361-215">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="2f361-215">**Device configuration**</span></span>|
|<span data-ttu-id="2f361-216">интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="2f361-216">intuneAccountId</span></span>|<span data-ttu-id="2f361-217">GUID</span><span class="sxs-lookup"><span data-stu-id="2f361-217">GUID</span></span>|<span data-ttu-id="2f361-218">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="2f361-218">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="2f361-219">легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="2f361-219">legacyPcManangementEnabled</span></span>|<span data-ttu-id="2f361-220">Логический</span><span class="sxs-lookup"><span data-stu-id="2f361-220">Boolean</span></span>|<span data-ttu-id="2f361-221">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2f361-221">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="2f361-222">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f361-222">This property is read-only.</span></span>|
|<span data-ttu-id="2f361-223">максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="2f361-223">maximumDepTokens</span></span>|<span data-ttu-id="2f361-224">Int32</span><span class="sxs-lookup"><span data-stu-id="2f361-224">Int32</span></span>|<span data-ttu-id="2f361-225">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="2f361-225">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="2f361-226">settings</span><span class="sxs-lookup"><span data-stu-id="2f361-226">settings</span></span>|[<span data-ttu-id="2f361-227">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2f361-227">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="2f361-228">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2f361-228">Account level settings.</span></span>|
|<span data-ttu-id="2f361-229">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2f361-229">**Device management**</span></span>|
|<span data-ttu-id="2f361-230">аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="2f361-230">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="2f361-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f361-231">DateTimeOffset</span></span>|<span data-ttu-id="2f361-232">Дата & время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="2f361-232">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="2f361-233">adminConsent</span><span class="sxs-lookup"><span data-stu-id="2f361-233">adminConsent</span></span>|[<span data-ttu-id="2f361-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="2f361-234">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="2f361-235">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="2f361-235">Admin consent information.</span></span>|
|<span data-ttu-id="2f361-236">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="2f361-236">deviceProtectionOverview</span></span>|<span data-ttu-id="2f361-237">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="2f361-237">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="2f361-238">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="2f361-238">Device protection overview.</span></span>|
|<span data-ttu-id="2f361-239">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="2f361-239">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="2f361-240">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="2f361-240">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="2f361-241">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="2f361-241">Device cleanup rule</span></span>|
|<span data-ttu-id="2f361-242">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="2f361-242">subscriptionState</span></span>|[<span data-ttu-id="2f361-243">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="2f361-243">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="2f361-244">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f361-244">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="2f361-245">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="2f361-245">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="2f361-246">subscriptions</span><span class="sxs-lookup"><span data-stu-id="2f361-246">subscriptions</span></span>|[<span data-ttu-id="2f361-247">девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="2f361-247">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="2f361-248">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="2f361-248">Tenant's Subscription.</span></span> <span data-ttu-id="2f361-249">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="2f361-249">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="2f361-250">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="2f361-250">windowsMalwareOverview</span></span>|[<span data-ttu-id="2f361-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="2f361-251">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="2f361-252">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="2f361-252">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="2f361-253">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="2f361-253">**Onboarding**</span></span>|
|<span data-ttu-id="2f361-254">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="2f361-254">intuneBrand</span></span>|[<span data-ttu-id="2f361-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="2f361-255">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="2f361-256">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="2f361-256">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="2f361-257">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="2f361-257">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="2f361-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f361-258">Response</span></span>
<span data-ttu-id="2f361-259">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f361-259">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f361-260">Пример</span><span class="sxs-lookup"><span data-stu-id="2f361-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f361-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f361-261">Request</span></span>

<span data-ttu-id="2f361-262">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="2f361-262">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="2f361-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f361-263">Response</span></span>

<span data-ttu-id="2f361-264">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f361-264">Here is an example of the response.</span></span> 

<span data-ttu-id="2f361-265">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2f361-265">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2f361-266">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="2f361-266">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```










