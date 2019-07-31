---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43672e497640f64e8efb98edf8f752a0c2415d63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979766"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="2af9c-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2af9c-103">Update deviceManagement</span></span>

> <span data-ttu-id="2af9c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2af9c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2af9c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2af9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2af9c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2af9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2af9c-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2af9c-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2af9c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2af9c-108">Prerequisites</span></span>

<span data-ttu-id="2af9c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2af9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2af9c-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="2af9c-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="2af9c-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="2af9c-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="2af9c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2af9c-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="2af9c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2af9c-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="2af9c-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="2af9c-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="2af9c-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="2af9c-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="2af9c-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="2af9c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="2af9c-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="2af9c-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-121">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="2af9c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2af9c-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-123">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="2af9c-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="2af9c-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2af9c-125">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2af9c-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2af9c-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-127">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="2af9c-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="2af9c-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-129">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="2af9c-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="2af9c-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-131">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="2af9c-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="2af9c-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-133">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="2af9c-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="2af9c-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-135">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="2af9c-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="2af9c-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-137">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="2af9c-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2af9c-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-139">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2af9c-139">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2af9c-140">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-140">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-141">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="2af9c-141">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="2af9c-142">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-142">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="2af9c-143">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="2af9c-143">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="2af9c-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-145">&nbsp;&nbsp; **Управление расходами** по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="2af9c-145">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="2af9c-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-147">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="2af9c-147">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="2af9c-148">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-148">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-149">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="2af9c-149">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="2af9c-150">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af9c-150">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2af9c-151">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2af9c-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2af9c-152">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2af9c-152">Not supported.</span></span>|
| <span data-ttu-id="2af9c-153">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2af9c-153">Application</span></span> | <span data-ttu-id="2af9c-154">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2af9c-154">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2af9c-155">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2af9c-155">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="2af9c-156">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2af9c-156">Request headers</span></span>

|<span data-ttu-id="2af9c-157">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2af9c-157">Header</span></span>|<span data-ttu-id="2af9c-158">Значение</span><span class="sxs-lookup"><span data-stu-id="2af9c-158">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2af9c-159">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2af9c-159">Authorization</span></span>|<span data-ttu-id="2af9c-160">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2af9c-160">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2af9c-161">Accept</span><span class="sxs-lookup"><span data-stu-id="2af9c-161">Accept</span></span>|<span data-ttu-id="2af9c-162">application/json</span><span class="sxs-lookup"><span data-stu-id="2af9c-162">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2af9c-163">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2af9c-163">Request body</span></span>

<span data-ttu-id="2af9c-164">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2af9c-164">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="2af9c-165">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2af9c-165">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="2af9c-166">Свойство</span><span class="sxs-lookup"><span data-stu-id="2af9c-166">Property</span></span>|<span data-ttu-id="2af9c-167">Тип</span><span class="sxs-lookup"><span data-stu-id="2af9c-167">Type</span></span>|<span data-ttu-id="2af9c-168">Описание</span><span class="sxs-lookup"><span data-stu-id="2af9c-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2af9c-169">id</span><span class="sxs-lookup"><span data-stu-id="2af9c-169">id</span></span>|<span data-ttu-id="2af9c-170">String</span><span class="sxs-lookup"><span data-stu-id="2af9c-170">String</span></span>|<span data-ttu-id="2af9c-171">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="2af9c-171">Unique identifier for the device.</span></span>|
|<span data-ttu-id="2af9c-172">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="2af9c-172">**Device configuration**</span></span>|
|<span data-ttu-id="2af9c-173">Интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="2af9c-173">intuneAccountId</span></span>|<span data-ttu-id="2af9c-174">GUID</span><span class="sxs-lookup"><span data-stu-id="2af9c-174">GUID</span></span>|<span data-ttu-id="2af9c-175">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="2af9c-175">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="2af9c-176">Легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="2af9c-176">legacyPcManangementEnabled</span></span>|<span data-ttu-id="2af9c-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="2af9c-177">Boolean</span></span>|<span data-ttu-id="2af9c-178">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2af9c-178">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="2af9c-179">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2af9c-179">This property is read-only.</span></span>|
|<span data-ttu-id="2af9c-180">Максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="2af9c-180">maximumDepTokens</span></span>|<span data-ttu-id="2af9c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="2af9c-181">Int32</span></span>|<span data-ttu-id="2af9c-182">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="2af9c-182">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="2af9c-183">settings</span><span class="sxs-lookup"><span data-stu-id="2af9c-183">settings</span></span>|[<span data-ttu-id="2af9c-184">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2af9c-184">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="2af9c-185">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2af9c-185">Account level settings.</span></span>|
|<span data-ttu-id="2af9c-186">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2af9c-186">**Device management**</span></span>|
|<span data-ttu-id="2af9c-187">Аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="2af9c-187">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="2af9c-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2af9c-188">DateTimeOffset</span></span>|<span data-ttu-id="2af9c-189">Дата & время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="2af9c-189">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="2af9c-190">adminConsent</span><span class="sxs-lookup"><span data-stu-id="2af9c-190">adminConsent</span></span>|[<span data-ttu-id="2af9c-191">adminConsent</span><span class="sxs-lookup"><span data-stu-id="2af9c-191">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="2af9c-192">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="2af9c-192">Admin consent information.</span></span>|
|<span data-ttu-id="2af9c-193">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="2af9c-193">deviceProtectionOverview</span></span>|<span data-ttu-id="2af9c-194">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="2af9c-194">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="2af9c-195">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="2af9c-195">Device protection overview.</span></span>|
|<span data-ttu-id="2af9c-196">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="2af9c-196">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="2af9c-197">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="2af9c-197">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="2af9c-198">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="2af9c-198">Device cleanup rule</span></span>|
|<span data-ttu-id="2af9c-199">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="2af9c-199">subscriptionState</span></span>|[<span data-ttu-id="2af9c-200">Девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="2af9c-200">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="2af9c-201">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="2af9c-201">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="2af9c-202">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="2af9c-202">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="2af9c-203">subscriptions</span><span class="sxs-lookup"><span data-stu-id="2af9c-203">subscriptions</span></span>|[<span data-ttu-id="2af9c-204">Девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="2af9c-204">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="2af9c-205">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="2af9c-205">Tenant's Subscription.</span></span> <span data-ttu-id="2af9c-206">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="2af9c-206">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="2af9c-207">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="2af9c-207">windowsMalwareOverview</span></span>|[<span data-ttu-id="2af9c-208">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="2af9c-208">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="2af9c-209">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="2af9c-209">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="2af9c-210">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="2af9c-210">**Onboarding**</span></span>|
|<span data-ttu-id="2af9c-211">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="2af9c-211">intuneBrand</span></span>|[<span data-ttu-id="2af9c-212">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="2af9c-212">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="2af9c-213">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="2af9c-213">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="2af9c-214">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="2af9c-214">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="2af9c-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="2af9c-215">Response</span></span>
<span data-ttu-id="2af9c-216">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2af9c-216">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2af9c-217">Пример</span><span class="sxs-lookup"><span data-stu-id="2af9c-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="2af9c-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="2af9c-218">Request</span></span>

<span data-ttu-id="2af9c-219">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="2af9c-219">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="2af9c-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="2af9c-220">Response</span></span>

<span data-ttu-id="2af9c-221">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2af9c-221">Here is an example of the response.</span></span> 

<span data-ttu-id="2af9c-222">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2af9c-222">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2af9c-223">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="2af9c-223">Returned properties vary according to workflow and context.</span></span>

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



