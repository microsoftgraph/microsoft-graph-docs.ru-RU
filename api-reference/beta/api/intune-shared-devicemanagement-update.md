---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2621df4ec2373c06433df5df4f253971d4280a15
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898488"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="c4346-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c4346-103">Update deviceManagement</span></span>

> <span data-ttu-id="c4346-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4346-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4346-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4346-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4346-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4346-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4346-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c4346-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4346-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c4346-108">Prerequisites</span></span>

<span data-ttu-id="c4346-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4346-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c4346-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c4346-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="c4346-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="c4346-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="c4346-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4346-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="c4346-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4346-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="c4346-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="c4346-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c4346-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="c4346-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="c4346-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c4346-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="c4346-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c4346-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-121">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="c4346-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c4346-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-123">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="c4346-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c4346-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c4346-125">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c4346-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c4346-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-127">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="c4346-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c4346-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-129">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="c4346-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c4346-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-131">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="c4346-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c4346-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-133">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="c4346-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c4346-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-135">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c4346-135">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c4346-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-137">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="c4346-137">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="c4346-138">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-138">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-139">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="c4346-139">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c4346-140">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4346-140">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c4346-141">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="c4346-141">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c4346-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-143">&nbsp;&nbsp; **Управление расходами** по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="c4346-143">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c4346-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-145">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="c4346-145">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="c4346-146">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-146">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-147">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="c4346-147">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c4346-148">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4346-148">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c4346-149">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4346-149">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4346-150">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4346-150">Not supported.</span></span>|
| <span data-ttu-id="c4346-151">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4346-151">Application</span></span> | <span data-ttu-id="c4346-152">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4346-152">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4346-153">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4346-153">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="c4346-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4346-154">Request headers</span></span>

|<span data-ttu-id="c4346-155">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4346-155">Header</span></span>|<span data-ttu-id="c4346-156">Значение</span><span class="sxs-lookup"><span data-stu-id="c4346-156">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4346-157">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4346-157">Authorization</span></span>|<span data-ttu-id="c4346-158">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4346-158">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4346-159">Accept</span><span class="sxs-lookup"><span data-stu-id="c4346-159">Accept</span></span>|<span data-ttu-id="c4346-160">application/json</span><span class="sxs-lookup"><span data-stu-id="c4346-160">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4346-161">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4346-161">Request body</span></span>

<span data-ttu-id="c4346-162">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4346-162">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="c4346-163">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c4346-163">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="c4346-164">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4346-164">Property</span></span>|<span data-ttu-id="c4346-165">Тип</span><span class="sxs-lookup"><span data-stu-id="c4346-165">Type</span></span>|<span data-ttu-id="c4346-166">Описание</span><span class="sxs-lookup"><span data-stu-id="c4346-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4346-167">id</span><span class="sxs-lookup"><span data-stu-id="c4346-167">id</span></span>|<span data-ttu-id="c4346-168">Строка</span><span class="sxs-lookup"><span data-stu-id="c4346-168">String</span></span>|<span data-ttu-id="c4346-169">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c4346-169">Unique identifier for the device.</span></span>|
|<span data-ttu-id="c4346-170">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="c4346-170">**Device configuration**</span></span>|
|<span data-ttu-id="c4346-171">Интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="c4346-171">intuneAccountId</span></span>|<span data-ttu-id="c4346-172">GUID</span><span class="sxs-lookup"><span data-stu-id="c4346-172">GUID</span></span>|<span data-ttu-id="c4346-173">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="c4346-173">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="c4346-174">Легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="c4346-174">legacyPcManangementEnabled</span></span>|<span data-ttu-id="c4346-175">Логический</span><span class="sxs-lookup"><span data-stu-id="c4346-175">Boolean</span></span>|<span data-ttu-id="c4346-176">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c4346-176">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="c4346-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4346-177">This property is read-only.</span></span>|
|<span data-ttu-id="c4346-178">Максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="c4346-178">maximumDepTokens</span></span>|<span data-ttu-id="c4346-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c4346-179">Int32</span></span>|<span data-ttu-id="c4346-180">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="c4346-180">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="c4346-181">settings</span><span class="sxs-lookup"><span data-stu-id="c4346-181">settings</span></span>|[<span data-ttu-id="c4346-182">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c4346-182">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="c4346-183">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c4346-183">Account level settings.</span></span>|
|<span data-ttu-id="c4346-184">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c4346-184">**Device management**</span></span>|
|<span data-ttu-id="c4346-185">Аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="c4346-185">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="c4346-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4346-186">DateTimeOffset</span></span>|<span data-ttu-id="c4346-187">Дата _Амп_ время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="c4346-187">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="c4346-188">adminConsent</span><span class="sxs-lookup"><span data-stu-id="c4346-188">adminConsent</span></span>|[<span data-ttu-id="c4346-189">adminConsent</span><span class="sxs-lookup"><span data-stu-id="c4346-189">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="c4346-190">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="c4346-190">Admin consent information.</span></span>|
|<span data-ttu-id="c4346-191">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="c4346-191">deviceProtectionOverview</span></span>|<span data-ttu-id="c4346-192">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="c4346-192">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="c4346-193">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="c4346-193">Device protection overview.</span></span>|
|<span data-ttu-id="c4346-194">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="c4346-194">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="c4346-195">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="c4346-195">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="c4346-196">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="c4346-196">Device cleanup rule</span></span>|
|<span data-ttu-id="c4346-197">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="c4346-197">subscriptionState</span></span>|[<span data-ttu-id="c4346-198">Девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="c4346-198">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="c4346-199">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4346-199">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="c4346-200">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c4346-200">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="c4346-201">subscriptions</span><span class="sxs-lookup"><span data-stu-id="c4346-201">subscriptions</span></span>|[<span data-ttu-id="c4346-202">Девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="c4346-202">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="c4346-203">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="c4346-203">Tenant's Subscription.</span></span> <span data-ttu-id="c4346-204">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="c4346-204">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="c4346-205">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="c4346-205">windowsMalwareOverview</span></span>|[<span data-ttu-id="c4346-206">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="c4346-206">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="c4346-207">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="c4346-207">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="c4346-208">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c4346-208">**Onboarding**</span></span>|
|<span data-ttu-id="c4346-209">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c4346-209">intuneBrand</span></span>|[<span data-ttu-id="c4346-210">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c4346-210">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="c4346-211">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4346-211">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="c4346-212">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c4346-212">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="c4346-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4346-213">Response</span></span>
<span data-ttu-id="c4346-214">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4346-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4346-215">Пример</span><span class="sxs-lookup"><span data-stu-id="c4346-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4346-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4346-216">Request</span></span>

<span data-ttu-id="c4346-217">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="c4346-217">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="c4346-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4346-218">Response</span></span>

<span data-ttu-id="c4346-219">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4346-219">Here is an example of the response.</span></span> 

<span data-ttu-id="c4346-220">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c4346-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c4346-221">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="c4346-221">Returned properties vary according to workflow and context.</span></span>

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



