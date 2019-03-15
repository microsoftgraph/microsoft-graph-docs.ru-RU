---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a71212652d789b08a8cb496b6b98c18b12d3e9c7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571055"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="20d6c-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="20d6c-103">Update deviceManagement</span></span>

> <span data-ttu-id="20d6c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20d6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20d6c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20d6c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20d6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20d6c-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="20d6c-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20d6c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20d6c-108">Prerequisites</span></span>

<span data-ttu-id="20d6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="20d6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

<span data-ttu-id="20d6c-111">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="20d6c-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="20d6c-112">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="20d6c-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="20d6c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20d6c-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="20d6c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20d6c-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="20d6c-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="20d6c-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="20d6c-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="20d6c-117">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="20d6c-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="20d6c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-119">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="20d6c-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="20d6c-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-121">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="20d6c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="20d6c-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-123">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="20d6c-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="20d6c-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-125">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="20d6c-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="20d6c-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-127">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="20d6c-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="20d6c-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-129">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="20d6c-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="20d6c-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-131">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="20d6c-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="20d6c-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-133">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="20d6c-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="20d6c-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-135">&nbsp;&nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="20d6c-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="20d6c-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-137">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="20d6c-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="20d6c-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="20d6c-139">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="20d6c-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="20d6c-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-141">&nbsp;&nbsp; **Управление расходами** по телекоммуникационной связи</span><span class="sxs-lookup"><span data-stu-id="20d6c-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="20d6c-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-143">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="20d6c-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="20d6c-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-145">&nbsp;&nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="20d6c-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="20d6c-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20d6c-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="20d6c-147">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20d6c-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20d6c-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d6c-148">Not supported.</span></span>|
| <span data-ttu-id="20d6c-149">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20d6c-149">Application</span></span> | <span data-ttu-id="20d6c-150">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d6c-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20d6c-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20d6c-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="20d6c-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20d6c-152">Request headers</span></span>

|<span data-ttu-id="20d6c-153">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20d6c-153">Header</span></span>|<span data-ttu-id="20d6c-154">Значение</span><span class="sxs-lookup"><span data-stu-id="20d6c-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20d6c-155">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20d6c-155">Authorization</span></span>|<span data-ttu-id="20d6c-156">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20d6c-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20d6c-157">Accept</span><span class="sxs-lookup"><span data-stu-id="20d6c-157">Accept</span></span>|<span data-ttu-id="20d6c-158">application/json</span><span class="sxs-lookup"><span data-stu-id="20d6c-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20d6c-159">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20d6c-159">Request body</span></span>

<span data-ttu-id="20d6c-160">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20d6c-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="20d6c-161">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="20d6c-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="20d6c-162">Свойство</span><span class="sxs-lookup"><span data-stu-id="20d6c-162">Property</span></span>|<span data-ttu-id="20d6c-163">Тип</span><span class="sxs-lookup"><span data-stu-id="20d6c-163">Type</span></span>|<span data-ttu-id="20d6c-164">Описание</span><span class="sxs-lookup"><span data-stu-id="20d6c-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20d6c-165">id</span><span class="sxs-lookup"><span data-stu-id="20d6c-165">id</span></span>|<span data-ttu-id="20d6c-166">Строка</span><span class="sxs-lookup"><span data-stu-id="20d6c-166">String</span></span>|<span data-ttu-id="20d6c-167">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="20d6c-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="20d6c-168">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="20d6c-168">**Device configuration**</span></span>|
|<span data-ttu-id="20d6c-169">Интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="20d6c-169">intuneAccountId</span></span>|<span data-ttu-id="20d6c-170">GUID</span><span class="sxs-lookup"><span data-stu-id="20d6c-170">GUID</span></span>|<span data-ttu-id="20d6c-171">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="20d6c-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="20d6c-172">Легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="20d6c-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="20d6c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="20d6c-173">Boolean</span></span>|<span data-ttu-id="20d6c-174">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="20d6c-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="20d6c-175">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20d6c-175">This property is read-only.</span></span>|
|<span data-ttu-id="20d6c-176">Максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="20d6c-176">maximumDepTokens</span></span>|<span data-ttu-id="20d6c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="20d6c-177">Int32</span></span>|<span data-ttu-id="20d6c-178">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="20d6c-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="20d6c-179">settings</span><span class="sxs-lookup"><span data-stu-id="20d6c-179">settings</span></span>|[<span data-ttu-id="20d6c-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="20d6c-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="20d6c-181">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="20d6c-181">Account level settings.</span></span>|
|<span data-ttu-id="20d6c-182">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="20d6c-182">**Device management**</span></span>|
|<span data-ttu-id="20d6c-183">Аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="20d6c-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="20d6c-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20d6c-184">DateTimeOffset</span></span>|<span data-ttu-id="20d6c-185">Дата _Амп_ время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="20d6c-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="20d6c-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="20d6c-186">adminConsent</span></span>|[<span data-ttu-id="20d6c-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="20d6c-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="20d6c-188">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="20d6c-188">Admin consent information.</span></span>|
|<span data-ttu-id="20d6c-189">deviceProtectionOverview;</span><span class="sxs-lookup"><span data-stu-id="20d6c-189">deviceProtectionOverview</span></span>|<span data-ttu-id="20d6c-190">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="20d6c-190">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="20d6c-191">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="20d6c-191">Device protection overview.</span></span>|
|<span data-ttu-id="20d6c-192">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="20d6c-192">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="20d6c-193">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="20d6c-193">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="20d6c-194">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="20d6c-194">Device cleanup rule</span></span>|
|<span data-ttu-id="20d6c-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="20d6c-195">subscriptionState</span></span>|[<span data-ttu-id="20d6c-196">Девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="20d6c-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="20d6c-197">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="20d6c-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="20d6c-198">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="20d6c-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="20d6c-199">подписки</span><span class="sxs-lookup"><span data-stu-id="20d6c-199">subscriptions</span></span>|[<span data-ttu-id="20d6c-200">Девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="20d6c-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="20d6c-201">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="20d6c-201">Tenant's Subscription.</span></span> <span data-ttu-id="20d6c-202">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="20d6c-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="20d6c-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="20d6c-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="20d6c-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="20d6c-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="20d6c-205">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="20d6c-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="20d6c-206">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="20d6c-206">**Onboarding**</span></span>|
|<span data-ttu-id="20d6c-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="20d6c-207">intuneBrand</span></span>|[<span data-ttu-id="20d6c-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="20d6c-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="20d6c-209">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="20d6c-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="20d6c-210">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="20d6c-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="20d6c-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="20d6c-211">Response</span></span>
<span data-ttu-id="20d6c-212">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20d6c-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20d6c-213">Пример</span><span class="sxs-lookup"><span data-stu-id="20d6c-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="20d6c-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="20d6c-214">Request</span></span>

<span data-ttu-id="20d6c-215">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="20d6c-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="20d6c-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="20d6c-216">Response</span></span>

<span data-ttu-id="20d6c-217">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20d6c-217">Here is an example of the response.</span></span> 

<span data-ttu-id="20d6c-218">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="20d6c-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="20d6c-219">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="20d6c-219">Returned properties vary according to workflow and context.</span></span>

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



