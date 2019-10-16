---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18ba331637a151531e6a4dcec9e794a01c927aef
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538275"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="c87d2-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c87d2-103">Update deviceManagement</span></span>

> <span data-ttu-id="c87d2-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c87d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c87d2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c87d2-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c87d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c87d2-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c87d2-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c87d2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c87d2-108">Prerequisites</span></span>

<span data-ttu-id="c87d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c87d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c87d2-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c87d2-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="c87d2-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="c87d2-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="c87d2-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c87d2-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="c87d2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c87d2-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="c87d2-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="c87d2-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c87d2-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="c87d2-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="c87d2-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c87d2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="c87d2-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c87d2-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-121">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="c87d2-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c87d2-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-123">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="c87d2-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c87d2-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c87d2-125">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c87d2-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c87d2-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-127">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="c87d2-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c87d2-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-129">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="c87d2-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c87d2-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-131">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="c87d2-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c87d2-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-133">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="c87d2-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c87d2-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-135">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="c87d2-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="c87d2-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-137">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c87d2-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c87d2-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-139">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c87d2-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c87d2-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-141">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="c87d2-141">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="c87d2-142">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-142">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-143">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="c87d2-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c87d2-144">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-144">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c87d2-145">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="c87d2-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c87d2-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-147">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c87d2-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c87d2-148">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-148">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-149">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="c87d2-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c87d2-150">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-150">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-151">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="c87d2-151">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="c87d2-152">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-152">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-153">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="c87d2-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c87d2-154">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-154">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-155">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c87d2-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87d2-156">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87d2-156">Not supported.</span></span>|
| <span data-ttu-id="c87d2-157">Приложение</span><span class="sxs-lookup"><span data-stu-id="c87d2-157">Application</span></span> ||
| <span data-ttu-id="c87d2-158">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="c87d2-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c87d2-159">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-159">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="c87d2-160">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="c87d2-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c87d2-161">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-161">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-162">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="c87d2-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c87d2-163">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-163">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-164">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="c87d2-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c87d2-165">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-165">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-166">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="c87d2-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c87d2-167">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-167">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c87d2-168">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c87d2-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c87d2-169">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-169">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-170">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="c87d2-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c87d2-171">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-171">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-172">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="c87d2-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c87d2-173">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-173">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-174">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="c87d2-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c87d2-175">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-175">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-176">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="c87d2-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c87d2-177">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-177">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-178">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="c87d2-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="c87d2-179">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-179">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-180">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c87d2-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c87d2-181">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-181">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-182">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c87d2-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c87d2-183">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-183">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-184">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="c87d2-184">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="c87d2-185">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-185">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-186">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="c87d2-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c87d2-187">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-187">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c87d2-188">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="c87d2-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c87d2-189">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-189">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-190">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c87d2-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c87d2-191">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-191">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-192">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="c87d2-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c87d2-193">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-193">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-194">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="c87d2-194">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="c87d2-195">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-195">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c87d2-196">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="c87d2-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c87d2-197">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c87d2-197">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c87d2-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c87d2-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="c87d2-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c87d2-199">Request headers</span></span>

|<span data-ttu-id="c87d2-200">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c87d2-200">Header</span></span>|<span data-ttu-id="c87d2-201">Значение</span><span class="sxs-lookup"><span data-stu-id="c87d2-201">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c87d2-202">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c87d2-202">Authorization</span></span>|<span data-ttu-id="c87d2-203">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c87d2-203">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c87d2-204">Accept</span><span class="sxs-lookup"><span data-stu-id="c87d2-204">Accept</span></span>|<span data-ttu-id="c87d2-205">application/json</span><span class="sxs-lookup"><span data-stu-id="c87d2-205">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c87d2-206">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c87d2-206">Request body</span></span>

<span data-ttu-id="c87d2-207">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c87d2-207">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="c87d2-208">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c87d2-208">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="c87d2-209">Свойство</span><span class="sxs-lookup"><span data-stu-id="c87d2-209">Property</span></span>|<span data-ttu-id="c87d2-210">Тип</span><span class="sxs-lookup"><span data-stu-id="c87d2-210">Type</span></span>|<span data-ttu-id="c87d2-211">Описание</span><span class="sxs-lookup"><span data-stu-id="c87d2-211">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c87d2-212">id</span><span class="sxs-lookup"><span data-stu-id="c87d2-212">id</span></span>|<span data-ttu-id="c87d2-213">String</span><span class="sxs-lookup"><span data-stu-id="c87d2-213">String</span></span>|<span data-ttu-id="c87d2-214">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c87d2-214">Unique identifier for the device.</span></span>|
|<span data-ttu-id="c87d2-215">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="c87d2-215">**Device configuration**</span></span>|
|<span data-ttu-id="c87d2-216">интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="c87d2-216">intuneAccountId</span></span>|<span data-ttu-id="c87d2-217">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="c87d2-217">GUID</span></span>|<span data-ttu-id="c87d2-218">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="c87d2-218">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="c87d2-219">легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="c87d2-219">legacyPcManangementEnabled</span></span>|<span data-ttu-id="c87d2-220">Логический</span><span class="sxs-lookup"><span data-stu-id="c87d2-220">Boolean</span></span>|<span data-ttu-id="c87d2-221">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c87d2-221">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="c87d2-222">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c87d2-222">This property is read-only.</span></span>|
|<span data-ttu-id="c87d2-223">максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="c87d2-223">maximumDepTokens</span></span>|<span data-ttu-id="c87d2-224">Int32</span><span class="sxs-lookup"><span data-stu-id="c87d2-224">Int32</span></span>|<span data-ttu-id="c87d2-225">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="c87d2-225">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="c87d2-226">settings</span><span class="sxs-lookup"><span data-stu-id="c87d2-226">settings</span></span>|[<span data-ttu-id="c87d2-227">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c87d2-227">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="c87d2-228">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c87d2-228">Account level settings.</span></span>|
|<span data-ttu-id="c87d2-229">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c87d2-229">**Device management**</span></span>|
|<span data-ttu-id="c87d2-230">аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="c87d2-230">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="c87d2-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87d2-231">DateTimeOffset</span></span>|<span data-ttu-id="c87d2-232">Дата & время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="c87d2-232">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="c87d2-233">adminConsent</span><span class="sxs-lookup"><span data-stu-id="c87d2-233">adminConsent</span></span>|[<span data-ttu-id="c87d2-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="c87d2-234">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="c87d2-235">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="c87d2-235">Admin consent information.</span></span>|
|<span data-ttu-id="c87d2-236">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="c87d2-236">deviceProtectionOverview</span></span>|<span data-ttu-id="c87d2-237">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="c87d2-237">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="c87d2-238">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="c87d2-238">Device protection overview.</span></span>|
|<span data-ttu-id="c87d2-239">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="c87d2-239">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="c87d2-240">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="c87d2-240">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="c87d2-241">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="c87d2-241">Device cleanup rule</span></span>|
|<span data-ttu-id="c87d2-242">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="c87d2-242">subscriptionState</span></span>|[<span data-ttu-id="c87d2-243">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="c87d2-243">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="c87d2-244">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="c87d2-244">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="c87d2-245">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c87d2-245">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="c87d2-246">subscriptions</span><span class="sxs-lookup"><span data-stu-id="c87d2-246">subscriptions</span></span>|[<span data-ttu-id="c87d2-247">девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="c87d2-247">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="c87d2-248">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="c87d2-248">Tenant's Subscription.</span></span> <span data-ttu-id="c87d2-249">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="c87d2-249">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="c87d2-250">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="c87d2-250">windowsMalwareOverview</span></span>|[<span data-ttu-id="c87d2-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="c87d2-251">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="c87d2-252">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="c87d2-252">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="c87d2-253">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c87d2-253">**Onboarding**</span></span>|
|<span data-ttu-id="c87d2-254">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c87d2-254">intuneBrand</span></span>|[<span data-ttu-id="c87d2-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c87d2-255">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="c87d2-256">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="c87d2-256">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="c87d2-257">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c87d2-257">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="c87d2-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87d2-258">Response</span></span>
<span data-ttu-id="c87d2-259">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c87d2-259">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c87d2-260">Пример</span><span class="sxs-lookup"><span data-stu-id="c87d2-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="c87d2-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="c87d2-261">Request</span></span>

<span data-ttu-id="c87d2-262">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="c87d2-262">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="c87d2-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87d2-263">Response</span></span>

<span data-ttu-id="c87d2-264">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c87d2-264">Here is an example of the response.</span></span> 

<span data-ttu-id="c87d2-265">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c87d2-265">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c87d2-266">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="c87d2-266">Returned properties vary according to workflow and context.</span></span>

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









