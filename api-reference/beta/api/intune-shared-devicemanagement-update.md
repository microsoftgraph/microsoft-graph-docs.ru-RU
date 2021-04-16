---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80f5fc4065d8db2f0bbb7659f244a14c9ef9331d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867527"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="89446-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="89446-103">Update deviceManagement</span></span>

<span data-ttu-id="89446-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89446-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89446-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="89446-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="89446-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89446-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89446-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89446-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89446-108">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="89446-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89446-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89446-109">Prerequisites</span></span>

<span data-ttu-id="89446-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89446-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="89446-112">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="89446-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="89446-113">Тип &nbsp; разрешения &nbsp; &nbsp; (по рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="89446-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="89446-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89446-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="89446-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89446-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="89446-116">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="89446-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="89446-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="89446-118">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="89446-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="89446-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-120">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="89446-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="89446-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="89446-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="89446-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-124">&nbsp;&nbsp; **Намерение устройства**</span><span class="sxs-lookup"><span data-stu-id="89446-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="89446-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="89446-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="89446-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="89446-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-128">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="89446-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="89446-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-130">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="89446-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="89446-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-132">&nbsp;&nbsp; **Фехтования**</span><span class="sxs-lookup"><span data-stu-id="89446-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="89446-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-134">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="89446-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="89446-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="89446-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="89446-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-138">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="89446-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="89446-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-140">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="89446-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="89446-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-142">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="89446-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="89446-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-144">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="89446-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="89446-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89446-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="89446-146">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="89446-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="89446-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-148">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="89446-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="89446-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-150">&nbsp;&nbsp; **Управление расходами телекома**</span><span class="sxs-lookup"><span data-stu-id="89446-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="89446-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="89446-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="89446-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-154">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="89446-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="89446-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-156">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89446-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89446-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89446-157">Not supported.</span></span>|
| <span data-ttu-id="89446-158">Для приложения</span><span class="sxs-lookup"><span data-stu-id="89446-158">Application</span></span> ||
| <span data-ttu-id="89446-159">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="89446-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="89446-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="89446-161">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="89446-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="89446-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-163">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="89446-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="89446-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-165">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="89446-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="89446-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-167">&nbsp;&nbsp; **Намерение устройства**</span><span class="sxs-lookup"><span data-stu-id="89446-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="89446-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="89446-169">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="89446-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="89446-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-171">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="89446-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="89446-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-173">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="89446-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="89446-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-175">&nbsp;&nbsp; **Фехтования**</span><span class="sxs-lookup"><span data-stu-id="89446-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="89446-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-177">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="89446-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="89446-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="89446-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="89446-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-181">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="89446-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="89446-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-183">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="89446-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="89446-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-185">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="89446-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="89446-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-187">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="89446-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="89446-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89446-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="89446-189">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="89446-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="89446-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-191">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="89446-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="89446-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-193">&nbsp;&nbsp; **Управление расходами телекома**</span><span class="sxs-lookup"><span data-stu-id="89446-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="89446-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="89446-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="89446-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="89446-197">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="89446-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="89446-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89446-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89446-199">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89446-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="89446-200">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89446-200">Request headers</span></span>

|<span data-ttu-id="89446-201">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89446-201">Header</span></span>|<span data-ttu-id="89446-202">Значение</span><span class="sxs-lookup"><span data-stu-id="89446-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89446-203">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89446-203">Authorization</span></span>|<span data-ttu-id="89446-204">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89446-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89446-205">Accept</span><span class="sxs-lookup"><span data-stu-id="89446-205">Accept</span></span>|<span data-ttu-id="89446-206">application/json</span><span class="sxs-lookup"><span data-stu-id="89446-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89446-207">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89446-207">Request body</span></span>

<span data-ttu-id="89446-208">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89446-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="89446-209">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="89446-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="89446-210">Свойство</span><span class="sxs-lookup"><span data-stu-id="89446-210">Property</span></span>|<span data-ttu-id="89446-211">Тип</span><span class="sxs-lookup"><span data-stu-id="89446-211">Type</span></span>|<span data-ttu-id="89446-212">Описание</span><span class="sxs-lookup"><span data-stu-id="89446-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89446-213">id</span><span class="sxs-lookup"><span data-stu-id="89446-213">id</span></span>|<span data-ttu-id="89446-214">String</span><span class="sxs-lookup"><span data-stu-id="89446-214">String</span></span>|<span data-ttu-id="89446-215">Уникальный идентификатор для устройства.</span><span class="sxs-lookup"><span data-stu-id="89446-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="89446-216">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="89446-216">**Device configuration**</span></span>|
|<span data-ttu-id="89446-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="89446-217">intuneAccountId</span></span>|<span data-ttu-id="89446-218">GUID</span><span class="sxs-lookup"><span data-stu-id="89446-218">GUID</span></span>|<span data-ttu-id="89446-219">ID учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="89446-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="89446-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="89446-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="89446-221">Логический</span><span class="sxs-lookup"><span data-stu-id="89446-221">Boolean</span></span>|<span data-ttu-id="89446-222">Свойство, чтобы включить для этой учетной записи управление устаревшим КОМПЬЮТЕРом без MDM.</span><span class="sxs-lookup"><span data-stu-id="89446-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="89446-223">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89446-223">This property is read-only.</span></span>|
|<span data-ttu-id="89446-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="89446-224">maximumDepTokens</span></span>|<span data-ttu-id="89446-225">Int32</span><span class="sxs-lookup"><span data-stu-id="89446-225">Int32</span></span>|<span data-ttu-id="89446-226">Максимальное количество маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="89446-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="89446-227">settings</span><span class="sxs-lookup"><span data-stu-id="89446-227">settings</span></span>|[<span data-ttu-id="89446-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="89446-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="89446-229">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="89446-229">Account level settings.</span></span>|
|<span data-ttu-id="89446-230">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="89446-230">**Device management**</span></span>|
|<span data-ttu-id="89446-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="89446-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="89446-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89446-232">DateTimeOffset</span></span>|<span data-ttu-id="89446-233">Дата &, когда данные клиента перемещаются между scaleunits.</span><span class="sxs-lookup"><span data-stu-id="89446-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="89446-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="89446-234">adminConsent</span></span>|[<span data-ttu-id="89446-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="89446-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="89446-236">Сведения о согласии администратора.</span><span class="sxs-lookup"><span data-stu-id="89446-236">Admin consent information.</span></span>|
|<span data-ttu-id="89446-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="89446-237">deviceProtectionOverview</span></span>|<span data-ttu-id="89446-238">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="89446-238">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="89446-239">Обзор защиты устройств.</span><span class="sxs-lookup"><span data-stu-id="89446-239">Device protection overview.</span></span>|
|<span data-ttu-id="89446-240">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="89446-240">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="89446-241">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="89446-241">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="89446-242">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="89446-242">Device cleanup rule</span></span>|
|<span data-ttu-id="89446-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="89446-243">subscriptionState</span></span>|[<span data-ttu-id="89446-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="89446-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="89446-245">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="89446-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="89446-246">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="89446-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="89446-247">subscriptions</span><span class="sxs-lookup"><span data-stu-id="89446-247">subscriptions</span></span>|[<span data-ttu-id="89446-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="89446-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="89446-249">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="89446-249">Tenant's Subscription.</span></span> <span data-ttu-id="89446-250">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="89446-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="89446-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="89446-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="89446-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="89446-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="89446-253">Обзор вредоносных программ для устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="89446-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="89446-254">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="89446-254">**Onboarding**</span></span>|
|<span data-ttu-id="89446-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="89446-255">intuneBrand</span></span>|[<span data-ttu-id="89446-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="89446-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="89446-257">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="89446-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="89446-258">Поддержка свойств тела запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="89446-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="89446-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="89446-259">Response</span></span>
<span data-ttu-id="89446-260">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89446-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89446-261">Пример</span><span class="sxs-lookup"><span data-stu-id="89446-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="89446-262">Запрос</span><span class="sxs-lookup"><span data-stu-id="89446-262">Request</span></span>

<span data-ttu-id="89446-263">Вот пример запроса, следующего за процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="89446-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="89446-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="89446-264">Response</span></span>

<span data-ttu-id="89446-265">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89446-265">Here is an example of the response.</span></span> 

<span data-ttu-id="89446-266">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="89446-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="89446-267">Возвращенные свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="89446-267">Returned properties vary according to workflow and context.</span></span>

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










