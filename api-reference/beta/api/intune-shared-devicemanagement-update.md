---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8f8b3171eaabedfa085f7685b2f4f7aa1ad87a3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194595"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="aac21-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="aac21-103">Update deviceManagement</span></span>

> <span data-ttu-id="aac21-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aac21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aac21-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aac21-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aac21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac21-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="aac21-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac21-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aac21-108">Prerequisites</span></span>

<span data-ttu-id="aac21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="aac21-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="aac21-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="aac21-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="aac21-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="aac21-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aac21-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="aac21-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aac21-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="aac21-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="aac21-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="aac21-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="aac21-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="aac21-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="aac21-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="aac21-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="aac21-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-121">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="aac21-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="aac21-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-123">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="aac21-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="aac21-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="aac21-125">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="aac21-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="aac21-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-127">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="aac21-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="aac21-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-129">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="aac21-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="aac21-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-131">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="aac21-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="aac21-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-133">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="aac21-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="aac21-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-135">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="aac21-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="aac21-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-137">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="aac21-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="aac21-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-139">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="aac21-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="aac21-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-141">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="aac21-141">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="aac21-142">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-142">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-143">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="aac21-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="aac21-144">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aac21-144">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="aac21-145">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="aac21-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="aac21-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-147">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="aac21-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="aac21-148">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-148">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-149">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="aac21-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="aac21-150">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-150">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-151">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="aac21-151">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="aac21-152">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-152">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-153">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="aac21-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="aac21-154">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-154">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-155">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aac21-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac21-156">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac21-156">Not supported.</span></span>|
| <span data-ttu-id="aac21-157">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aac21-157">Application</span></span> ||
| <span data-ttu-id="aac21-158">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="aac21-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="aac21-159">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-159">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="aac21-160">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="aac21-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="aac21-161">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-161">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-162">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="aac21-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="aac21-163">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-163">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-164">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="aac21-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="aac21-165">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-165">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-166">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="aac21-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="aac21-167">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-167">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="aac21-168">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="aac21-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="aac21-169">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-169">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-170">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="aac21-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="aac21-171">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-171">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-172">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="aac21-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="aac21-173">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-173">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-174">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="aac21-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="aac21-175">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-175">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-176">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="aac21-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="aac21-177">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-177">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-178">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="aac21-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="aac21-179">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-179">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-180">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="aac21-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="aac21-181">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-181">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-182">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="aac21-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="aac21-183">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-183">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-184">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="aac21-184">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="aac21-185">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-185">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-186">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="aac21-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="aac21-187">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aac21-187">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="aac21-188">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="aac21-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="aac21-189">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-189">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-190">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="aac21-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="aac21-191">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-191">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-192">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="aac21-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="aac21-193">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-193">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-194">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="aac21-194">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="aac21-195">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-195">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="aac21-196">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="aac21-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="aac21-197">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac21-197">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aac21-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aac21-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="aac21-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aac21-199">Request headers</span></span>

|<span data-ttu-id="aac21-200">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aac21-200">Header</span></span>|<span data-ttu-id="aac21-201">Значение</span><span class="sxs-lookup"><span data-stu-id="aac21-201">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac21-202">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aac21-202">Authorization</span></span>|<span data-ttu-id="aac21-203">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aac21-203">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac21-204">Accept</span><span class="sxs-lookup"><span data-stu-id="aac21-204">Accept</span></span>|<span data-ttu-id="aac21-205">application/json</span><span class="sxs-lookup"><span data-stu-id="aac21-205">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac21-206">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aac21-206">Request body</span></span>

<span data-ttu-id="aac21-207">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aac21-207">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="aac21-208">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="aac21-208">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="aac21-209">Свойство</span><span class="sxs-lookup"><span data-stu-id="aac21-209">Property</span></span>|<span data-ttu-id="aac21-210">Тип</span><span class="sxs-lookup"><span data-stu-id="aac21-210">Type</span></span>|<span data-ttu-id="aac21-211">Описание</span><span class="sxs-lookup"><span data-stu-id="aac21-211">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac21-212">id</span><span class="sxs-lookup"><span data-stu-id="aac21-212">id</span></span>|<span data-ttu-id="aac21-213">String</span><span class="sxs-lookup"><span data-stu-id="aac21-213">String</span></span>|<span data-ttu-id="aac21-214">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="aac21-214">Unique identifier for the device.</span></span>|
|<span data-ttu-id="aac21-215">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="aac21-215">**Device configuration**</span></span>|
|<span data-ttu-id="aac21-216">интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="aac21-216">intuneAccountId</span></span>|<span data-ttu-id="aac21-217">GUID</span><span class="sxs-lookup"><span data-stu-id="aac21-217">GUID</span></span>|<span data-ttu-id="aac21-218">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="aac21-218">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="aac21-219">легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="aac21-219">legacyPcManangementEnabled</span></span>|<span data-ttu-id="aac21-220">Boolean.</span><span class="sxs-lookup"><span data-stu-id="aac21-220">Boolean</span></span>|<span data-ttu-id="aac21-221">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="aac21-221">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="aac21-222">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aac21-222">This property is read-only.</span></span>|
|<span data-ttu-id="aac21-223">максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="aac21-223">maximumDepTokens</span></span>|<span data-ttu-id="aac21-224">Int32</span><span class="sxs-lookup"><span data-stu-id="aac21-224">Int32</span></span>|<span data-ttu-id="aac21-225">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="aac21-225">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="aac21-226">settings</span><span class="sxs-lookup"><span data-stu-id="aac21-226">settings</span></span>|[<span data-ttu-id="aac21-227">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="aac21-227">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="aac21-228">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="aac21-228">Account level settings.</span></span>|
|<span data-ttu-id="aac21-229">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="aac21-229">**Device management**</span></span>|
|<span data-ttu-id="aac21-230">аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="aac21-230">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="aac21-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac21-231">DateTimeOffset</span></span>|<span data-ttu-id="aac21-232">Дата & время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="aac21-232">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="aac21-233">adminConsent</span><span class="sxs-lookup"><span data-stu-id="aac21-233">adminConsent</span></span>|[<span data-ttu-id="aac21-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="aac21-234">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="aac21-235">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="aac21-235">Admin consent information.</span></span>|
|<span data-ttu-id="aac21-236">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="aac21-236">deviceProtectionOverview</span></span>|<span data-ttu-id="aac21-237">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="aac21-237">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="aac21-238">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="aac21-238">Device protection overview.</span></span>|
|<span data-ttu-id="aac21-239">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="aac21-239">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="aac21-240">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="aac21-240">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="aac21-241">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="aac21-241">Device cleanup rule</span></span>|
|<span data-ttu-id="aac21-242">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="aac21-242">subscriptionState</span></span>|[<span data-ttu-id="aac21-243">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="aac21-243">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="aac21-244">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="aac21-244">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="aac21-245">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="aac21-245">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="aac21-246">subscriptions</span><span class="sxs-lookup"><span data-stu-id="aac21-246">subscriptions</span></span>|[<span data-ttu-id="aac21-247">девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="aac21-247">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="aac21-248">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="aac21-248">Tenant's Subscription.</span></span> <span data-ttu-id="aac21-249">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="aac21-249">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="aac21-250">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="aac21-250">windowsMalwareOverview</span></span>|[<span data-ttu-id="aac21-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="aac21-251">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="aac21-252">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="aac21-252">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="aac21-253">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="aac21-253">**Onboarding**</span></span>|
|<span data-ttu-id="aac21-254">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="aac21-254">intuneBrand</span></span>|[<span data-ttu-id="aac21-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="aac21-255">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="aac21-256">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="aac21-256">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="aac21-257">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="aac21-257">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="aac21-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac21-258">Response</span></span>
<span data-ttu-id="aac21-259">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aac21-259">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac21-260">Пример</span><span class="sxs-lookup"><span data-stu-id="aac21-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac21-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="aac21-261">Request</span></span>

<span data-ttu-id="aac21-262">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="aac21-262">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="aac21-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac21-263">Response</span></span>

<span data-ttu-id="aac21-264">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aac21-264">Here is an example of the response.</span></span> 

<span data-ttu-id="aac21-265">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="aac21-265">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aac21-266">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="aac21-266">Returned properties vary according to workflow and context.</span></span>

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







