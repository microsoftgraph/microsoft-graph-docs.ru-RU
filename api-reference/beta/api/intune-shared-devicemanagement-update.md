---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4ef1c7eb4711afd2aa29071f160f440dceefba3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960407"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="64bfb-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="64bfb-103">Update deviceManagement</span></span>

> <span data-ttu-id="64bfb-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64bfb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64bfb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64bfb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64bfb-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64bfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64bfb-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="64bfb-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64bfb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64bfb-108">Prerequisites</span></span>

<span data-ttu-id="64bfb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64bfb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="64bfb-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="64bfb-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="64bfb-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="64bfb-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="64bfb-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64bfb-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="64bfb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64bfb-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="64bfb-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="64bfb-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="64bfb-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="64bfb-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="64bfb-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="64bfb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="64bfb-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="64bfb-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-121">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="64bfb-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="64bfb-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-123">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="64bfb-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="64bfb-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-125">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="64bfb-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="64bfb-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-127">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="64bfb-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="64bfb-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-129">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="64bfb-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="64bfb-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-131">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="64bfb-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="64bfb-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-133">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="64bfb-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="64bfb-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-135">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="64bfb-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="64bfb-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-137">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="64bfb-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="64bfb-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="64bfb-139">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="64bfb-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="64bfb-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-141">&nbsp;&nbsp; **Управление расходами** по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="64bfb-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="64bfb-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-143">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="64bfb-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="64bfb-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-145">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="64bfb-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="64bfb-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bfb-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="64bfb-147">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64bfb-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64bfb-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64bfb-148">Not supported.</span></span>|
| <span data-ttu-id="64bfb-149">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64bfb-149">Application</span></span> | <span data-ttu-id="64bfb-150">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64bfb-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64bfb-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64bfb-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="64bfb-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64bfb-152">Request headers</span></span>

|<span data-ttu-id="64bfb-153">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64bfb-153">Header</span></span>|<span data-ttu-id="64bfb-154">Значение</span><span class="sxs-lookup"><span data-stu-id="64bfb-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64bfb-155">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64bfb-155">Authorization</span></span>|<span data-ttu-id="64bfb-156">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64bfb-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64bfb-157">Accept</span><span class="sxs-lookup"><span data-stu-id="64bfb-157">Accept</span></span>|<span data-ttu-id="64bfb-158">application/json</span><span class="sxs-lookup"><span data-stu-id="64bfb-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64bfb-159">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64bfb-159">Request body</span></span>

<span data-ttu-id="64bfb-160">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64bfb-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="64bfb-161">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="64bfb-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="64bfb-162">Свойство</span><span class="sxs-lookup"><span data-stu-id="64bfb-162">Property</span></span>|<span data-ttu-id="64bfb-163">Тип</span><span class="sxs-lookup"><span data-stu-id="64bfb-163">Type</span></span>|<span data-ttu-id="64bfb-164">Описание</span><span class="sxs-lookup"><span data-stu-id="64bfb-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64bfb-165">id</span><span class="sxs-lookup"><span data-stu-id="64bfb-165">id</span></span>|<span data-ttu-id="64bfb-166">String</span><span class="sxs-lookup"><span data-stu-id="64bfb-166">String</span></span>|<span data-ttu-id="64bfb-167">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="64bfb-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="64bfb-168">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="64bfb-168">**Device configuration**</span></span>|
|<span data-ttu-id="64bfb-169">Интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="64bfb-169">intuneAccountId</span></span>|<span data-ttu-id="64bfb-170">GUID</span><span class="sxs-lookup"><span data-stu-id="64bfb-170">GUID</span></span>|<span data-ttu-id="64bfb-171">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="64bfb-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="64bfb-172">Легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="64bfb-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="64bfb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="64bfb-173">Boolean</span></span>|<span data-ttu-id="64bfb-174">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="64bfb-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="64bfb-175">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64bfb-175">This property is read-only.</span></span>|
|<span data-ttu-id="64bfb-176">Максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="64bfb-176">maximumDepTokens</span></span>|<span data-ttu-id="64bfb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="64bfb-177">Int32</span></span>|<span data-ttu-id="64bfb-178">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="64bfb-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="64bfb-179">settings</span><span class="sxs-lookup"><span data-stu-id="64bfb-179">settings</span></span>|[<span data-ttu-id="64bfb-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="64bfb-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="64bfb-181">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="64bfb-181">Account level settings.</span></span>|
|<span data-ttu-id="64bfb-182">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="64bfb-182">**Device management**</span></span>|
|<span data-ttu-id="64bfb-183">Аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="64bfb-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="64bfb-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64bfb-184">DateTimeOffset</span></span>|<span data-ttu-id="64bfb-185">Дата _Амп_ время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="64bfb-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="64bfb-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="64bfb-186">adminConsent</span></span>|[<span data-ttu-id="64bfb-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="64bfb-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="64bfb-188">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="64bfb-188">Admin consent information.</span></span>|
|<span data-ttu-id="64bfb-189">deviceProtectionOverview;</span><span class="sxs-lookup"><span data-stu-id="64bfb-189">deviceProtectionOverview</span></span>|<span data-ttu-id="64bfb-190">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="64bfb-190">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="64bfb-191">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="64bfb-191">Device protection overview.</span></span>|
|<span data-ttu-id="64bfb-192">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="64bfb-192">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="64bfb-193">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="64bfb-193">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="64bfb-194">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="64bfb-194">Device cleanup rule</span></span>|
|<span data-ttu-id="64bfb-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="64bfb-195">subscriptionState</span></span>|[<span data-ttu-id="64bfb-196">Девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="64bfb-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="64bfb-197">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="64bfb-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="64bfb-198">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="64bfb-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="64bfb-199">subscriptions</span><span class="sxs-lookup"><span data-stu-id="64bfb-199">subscriptions</span></span>|[<span data-ttu-id="64bfb-200">Девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="64bfb-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="64bfb-201">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="64bfb-201">Tenant's Subscription.</span></span> <span data-ttu-id="64bfb-202">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="64bfb-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="64bfb-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="64bfb-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="64bfb-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="64bfb-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="64bfb-205">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="64bfb-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="64bfb-206">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="64bfb-206">**Onboarding**</span></span>|
|<span data-ttu-id="64bfb-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="64bfb-207">intuneBrand</span></span>|[<span data-ttu-id="64bfb-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="64bfb-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="64bfb-209">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="64bfb-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="64bfb-210">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="64bfb-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="64bfb-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="64bfb-211">Response</span></span>
<span data-ttu-id="64bfb-212">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64bfb-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64bfb-213">Пример</span><span class="sxs-lookup"><span data-stu-id="64bfb-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="64bfb-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="64bfb-214">Request</span></span>

<span data-ttu-id="64bfb-215">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="64bfb-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="64bfb-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="64bfb-216">Response</span></span>

<span data-ttu-id="64bfb-217">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64bfb-217">Here is an example of the response.</span></span> 

<span data-ttu-id="64bfb-218">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="64bfb-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="64bfb-219">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="64bfb-219">Returned properties vary according to workflow and context.</span></span>

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



