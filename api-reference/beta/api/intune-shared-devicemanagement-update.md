---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75bca64ce38779e0e9c1f905525414e5b0308f81
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390054"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="09c59-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="09c59-103">Update deviceManagement</span></span>

<span data-ttu-id="09c59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09c59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09c59-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="09c59-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09c59-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09c59-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09c59-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09c59-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09c59-108">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="09c59-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09c59-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09c59-109">Prerequisites</span></span>

<span data-ttu-id="09c59-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09c59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="09c59-112">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="09c59-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="09c59-113">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="09c59-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="09c59-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09c59-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="09c59-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09c59-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="09c59-116">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="09c59-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="09c59-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="09c59-118">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="09c59-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="09c59-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-120">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="09c59-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="09c59-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="09c59-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="09c59-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-124">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="09c59-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="09c59-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="09c59-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="09c59-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="09c59-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-128">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="09c59-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="09c59-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-130">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="09c59-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="09c59-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-132">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="09c59-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="09c59-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-134">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="09c59-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="09c59-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-136">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="09c59-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="09c59-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-138">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="09c59-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="09c59-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-140">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="09c59-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="09c59-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-142">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="09c59-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="09c59-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-144">&nbsp;&nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="09c59-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="09c59-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09c59-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="09c59-146">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="09c59-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="09c59-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-148">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="09c59-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="09c59-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-150">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="09c59-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="09c59-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-152">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="09c59-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="09c59-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-154">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="09c59-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="09c59-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-156">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09c59-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09c59-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09c59-157">Not supported.</span></span>|
| <span data-ttu-id="09c59-158">Для приложения</span><span class="sxs-lookup"><span data-stu-id="09c59-158">Application</span></span> ||
| <span data-ttu-id="09c59-159">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="09c59-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="09c59-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="09c59-161">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="09c59-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="09c59-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-163">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="09c59-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="09c59-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-165">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="09c59-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="09c59-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-167">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="09c59-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="09c59-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="09c59-169">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="09c59-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="09c59-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-171">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="09c59-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="09c59-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-173">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="09c59-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="09c59-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-175">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="09c59-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="09c59-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-177">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="09c59-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="09c59-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-179">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="09c59-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="09c59-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-181">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="09c59-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="09c59-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-183">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="09c59-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="09c59-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-185">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="09c59-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="09c59-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-187">&nbsp;&nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="09c59-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="09c59-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09c59-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="09c59-189">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="09c59-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="09c59-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-191">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="09c59-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="09c59-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-193">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="09c59-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="09c59-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-195">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="09c59-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="09c59-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="09c59-197">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="09c59-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="09c59-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c59-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09c59-199">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09c59-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="09c59-200">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09c59-200">Request headers</span></span>

|<span data-ttu-id="09c59-201">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09c59-201">Header</span></span>|<span data-ttu-id="09c59-202">Значение</span><span class="sxs-lookup"><span data-stu-id="09c59-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09c59-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="09c59-203">Authorization</span></span>|<span data-ttu-id="09c59-204">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09c59-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09c59-205">Accept</span><span class="sxs-lookup"><span data-stu-id="09c59-205">Accept</span></span>|<span data-ttu-id="09c59-206">application/json</span><span class="sxs-lookup"><span data-stu-id="09c59-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09c59-207">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09c59-207">Request body</span></span>

<span data-ttu-id="09c59-208">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09c59-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="09c59-209">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="09c59-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="09c59-210">Свойство</span><span class="sxs-lookup"><span data-stu-id="09c59-210">Property</span></span>|<span data-ttu-id="09c59-211">Тип</span><span class="sxs-lookup"><span data-stu-id="09c59-211">Type</span></span>|<span data-ttu-id="09c59-212">Описание</span><span class="sxs-lookup"><span data-stu-id="09c59-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09c59-213">id</span><span class="sxs-lookup"><span data-stu-id="09c59-213">id</span></span>|<span data-ttu-id="09c59-214">String</span><span class="sxs-lookup"><span data-stu-id="09c59-214">String</span></span>|<span data-ttu-id="09c59-215">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="09c59-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="09c59-216">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="09c59-216">**Device configuration**</span></span>|
|<span data-ttu-id="09c59-217">интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="09c59-217">intuneAccountId</span></span>|<span data-ttu-id="09c59-218">GUID</span><span class="sxs-lookup"><span data-stu-id="09c59-218">GUID</span></span>|<span data-ttu-id="09c59-219">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="09c59-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="09c59-220">легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="09c59-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="09c59-221">Логическое</span><span class="sxs-lookup"><span data-stu-id="09c59-221">Boolean</span></span>|<span data-ttu-id="09c59-222">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="09c59-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="09c59-223">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09c59-223">This property is read-only.</span></span>|
|<span data-ttu-id="09c59-224">максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="09c59-224">maximumDepTokens</span></span>|<span data-ttu-id="09c59-225">Int32</span><span class="sxs-lookup"><span data-stu-id="09c59-225">Int32</span></span>|<span data-ttu-id="09c59-226">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="09c59-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="09c59-227">settings</span><span class="sxs-lookup"><span data-stu-id="09c59-227">settings</span></span>|[<span data-ttu-id="09c59-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="09c59-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="09c59-229">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="09c59-229">Account level settings.</span></span>|
|<span data-ttu-id="09c59-230">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="09c59-230">**Device management**</span></span>|
|<span data-ttu-id="09c59-231">аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="09c59-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="09c59-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09c59-232">DateTimeOffset</span></span>|<span data-ttu-id="09c59-233">Дата & время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="09c59-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="09c59-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="09c59-234">adminConsent</span></span>|[<span data-ttu-id="09c59-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="09c59-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="09c59-236">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="09c59-236">Admin consent information.</span></span>|
|<span data-ttu-id="09c59-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="09c59-237">deviceProtectionOverview</span></span>|<span data-ttu-id="09c59-238">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="09c59-238">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="09c59-239">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="09c59-239">Device protection overview.</span></span>|
|<span data-ttu-id="09c59-240">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="09c59-240">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="09c59-241">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="09c59-241">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="09c59-242">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="09c59-242">Device cleanup rule</span></span>|
|<span data-ttu-id="09c59-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="09c59-243">subscriptionState</span></span>|[<span data-ttu-id="09c59-244">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="09c59-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="09c59-245">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="09c59-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="09c59-246">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="09c59-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="09c59-247">subscriptions</span><span class="sxs-lookup"><span data-stu-id="09c59-247">subscriptions</span></span>|[<span data-ttu-id="09c59-248">девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="09c59-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="09c59-249">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="09c59-249">Tenant's Subscription.</span></span> <span data-ttu-id="09c59-250">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="09c59-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="09c59-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="09c59-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="09c59-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="09c59-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="09c59-253">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="09c59-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="09c59-254">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="09c59-254">**Onboarding**</span></span>|
|<span data-ttu-id="09c59-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="09c59-255">intuneBrand</span></span>|[<span data-ttu-id="09c59-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="09c59-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="09c59-257">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="09c59-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="09c59-258">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="09c59-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="09c59-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="09c59-259">Response</span></span>
<span data-ttu-id="09c59-260">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="09c59-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09c59-261">Пример</span><span class="sxs-lookup"><span data-stu-id="09c59-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="09c59-262">Запрос</span><span class="sxs-lookup"><span data-stu-id="09c59-262">Request</span></span>

<span data-ttu-id="09c59-263">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="09c59-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="09c59-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="09c59-264">Response</span></span>

<span data-ttu-id="09c59-265">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09c59-265">Here is an example of the response.</span></span> 

<span data-ttu-id="09c59-266">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="09c59-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="09c59-267">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="09c59-267">Returned properties vary according to workflow and context.</span></span>

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









