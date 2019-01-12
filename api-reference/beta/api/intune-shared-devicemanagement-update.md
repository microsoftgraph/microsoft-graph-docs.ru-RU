---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d8465ee45a2a6c23dedc4fe049ef1f73bb25218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924694"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="be4d4-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="be4d4-103">Update deviceManagement</span></span>

> <span data-ttu-id="be4d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be4d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be4d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be4d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be4d4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be4d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be4d4-107">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="be4d4-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be4d4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="be4d4-108">Prerequisites</span></span>

<span data-ttu-id="be4d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be4d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="be4d4-111">Обратите внимание, что это разрешение различаться в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="be4d4-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="be4d4-112">Разрешение&nbsp;тип&nbsp;(с&nbsp;рабочего процесса)</span><span class="sxs-lookup"><span data-stu-id="be4d4-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="be4d4-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be4d4-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="be4d4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be4d4-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="be4d4-115">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="be4d4-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="be4d4-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="be4d4-117">&nbsp; &nbsp; **аудита;**</span><span class="sxs-lookup"><span data-stu-id="be4d4-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="be4d4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-119">&nbsp;&nbsp; **Компании термины**</span><span class="sxs-lookup"><span data-stu-id="be4d4-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="be4d4-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-121">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="be4d4-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="be4d4-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-123">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="be4d4-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="be4d4-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-125">&nbsp;&nbsp; **Электронных диспетчера установки**</span><span class="sxs-lookup"><span data-stu-id="be4d4-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="be4d4-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-127">&nbsp; &nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="be4d4-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="be4d4-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-129">&nbsp;&nbsp; **Разграничения**</span><span class="sxs-lookup"><span data-stu-id="be4d4-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="be4d4-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-131">&nbsp;&nbsp; **Уведомлений**</span><span class="sxs-lookup"><span data-stu-id="be4d4-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="be4d4-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-133">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="be4d4-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="be4d4-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-135">&nbsp;&nbsp; **Управления доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="be4d4-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="be4d4-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-137">&nbsp;&nbsp; **Удаленного доступа**</span><span class="sxs-lookup"><span data-stu-id="be4d4-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="be4d4-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="be4d4-139">&nbsp;&nbsp; **Удаленный помощник**</span><span class="sxs-lookup"><span data-stu-id="be4d4-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="be4d4-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-141">&nbsp;&nbsp; **Управления расходами телекоммуникации**</span><span class="sxs-lookup"><span data-stu-id="be4d4-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="be4d4-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="be4d4-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="be4d4-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-145">&nbsp;&nbsp; **Защита информации Windows**</span><span class="sxs-lookup"><span data-stu-id="be4d4-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="be4d4-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be4d4-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="be4d4-147">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be4d4-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be4d4-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be4d4-148">Not supported.</span></span>|
| <span data-ttu-id="be4d4-149">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be4d4-149">Application</span></span> | <span data-ttu-id="be4d4-150">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be4d4-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be4d4-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be4d4-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="be4d4-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be4d4-152">Request headers</span></span>

|<span data-ttu-id="be4d4-153">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be4d4-153">Header</span></span>|<span data-ttu-id="be4d4-154">Значение</span><span class="sxs-lookup"><span data-stu-id="be4d4-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be4d4-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="be4d4-155">Authorization</span></span>|<span data-ttu-id="be4d4-156">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be4d4-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be4d4-157">Accept</span><span class="sxs-lookup"><span data-stu-id="be4d4-157">Accept</span></span>|<span data-ttu-id="be4d4-158">application/json</span><span class="sxs-lookup"><span data-stu-id="be4d4-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4d4-159">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be4d4-159">Request body</span></span>

<span data-ttu-id="be4d4-160">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be4d4-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="be4d4-161">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="be4d4-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="be4d4-162">Свойство</span><span class="sxs-lookup"><span data-stu-id="be4d4-162">Property</span></span>|<span data-ttu-id="be4d4-163">Тип</span><span class="sxs-lookup"><span data-stu-id="be4d4-163">Type</span></span>|<span data-ttu-id="be4d4-164">Описание</span><span class="sxs-lookup"><span data-stu-id="be4d4-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be4d4-165">id</span><span class="sxs-lookup"><span data-stu-id="be4d4-165">id</span></span>|<span data-ttu-id="be4d4-166">Строка</span><span class="sxs-lookup"><span data-stu-id="be4d4-166">String</span></span>|<span data-ttu-id="be4d4-167">Уникальный идентификатор для устройства.</span><span class="sxs-lookup"><span data-stu-id="be4d4-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="be4d4-168">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="be4d4-168">**Device configuration**</span></span>|
|<span data-ttu-id="be4d4-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="be4d4-169">intuneAccountId</span></span>|<span data-ttu-id="be4d4-170">GUID</span><span class="sxs-lookup"><span data-stu-id="be4d4-170">GUID</span></span>|<span data-ttu-id="be4d4-171">Идентификатор учетной записи Intune для заданного клиента</span><span class="sxs-lookup"><span data-stu-id="be4d4-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="be4d4-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="be4d4-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="be4d4-173">Логический</span><span class="sxs-lookup"><span data-stu-id="be4d4-173">Boolean</span></span>|<span data-ttu-id="be4d4-174">Свойство для включения не MDM управляемых прежних версий управления ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="be4d4-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="be4d4-175">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be4d4-175">This property is read-only.</span></span>|
|<span data-ttu-id="be4d4-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="be4d4-176">maximumDepTokens</span></span>|<span data-ttu-id="be4d4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="be4d4-177">Int32</span></span>|<span data-ttu-id="be4d4-178">Максимальное число DEP маркеры могут каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="be4d4-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="be4d4-179">settings</span><span class="sxs-lookup"><span data-stu-id="be4d4-179">settings</span></span>|[<span data-ttu-id="be4d4-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="be4d4-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="be4d4-181">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="be4d4-181">Account level settings.</span></span>|
|<span data-ttu-id="be4d4-182">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="be4d4-182">**Device management**</span></span>|
|<span data-ttu-id="be4d4-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="be4d4-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="be4d4-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4d4-184">DateTimeOffset</span></span>|<span data-ttu-id="be4d4-185">Дата и время, когда данные клиента перемещать между ScaleUnits строкового.</span><span class="sxs-lookup"><span data-stu-id="be4d4-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="be4d4-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="be4d4-186">adminConsent</span></span>|[<span data-ttu-id="be4d4-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="be4d4-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="be4d4-188">Сведения о разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="be4d4-188">Admin consent information.</span></span>|
|<span data-ttu-id="be4d4-189">deviceProtectionOverview;</span><span class="sxs-lookup"><span data-stu-id="be4d4-189">deviceProtectionOverview</span></span>|<span data-ttu-id="be4d4-190">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="be4d4-190">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="be4d4-191">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="be4d4-191">Device protection overview.</span></span>|
|<span data-ttu-id="be4d4-192">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="be4d4-192">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="be4d4-193">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="be4d4-193">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="be4d4-194">Правила очистки устройства</span><span class="sxs-lookup"><span data-stu-id="be4d4-194">Device cleanup rule</span></span>|
|<span data-ttu-id="be4d4-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="be4d4-195">subscriptionState</span></span>|[<span data-ttu-id="be4d4-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="be4d4-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="be4d4-197">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="be4d4-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="be4d4-198">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="be4d4-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="be4d4-199">подписки</span><span class="sxs-lookup"><span data-stu-id="be4d4-199">subscriptions</span></span>|[<span data-ttu-id="be4d4-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="be4d4-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="be4d4-201">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="be4d4-201">Tenant's Subscription.</span></span> <span data-ttu-id="be4d4-202">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="be4d4-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="be4d4-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="be4d4-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="be4d4-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="be4d4-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="be4d4-205">Обзор вредоносных программ для устройств windows.</span><span class="sxs-lookup"><span data-stu-id="be4d4-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="be4d4-206">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="be4d4-206">**Onboarding**</span></span>|
|<span data-ttu-id="be4d4-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="be4d4-207">intuneBrand</span></span>|[<span data-ttu-id="be4d4-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="be4d4-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="be4d4-209">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="be4d4-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="be4d4-210">Поддержка свойств текст запроса изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="be4d4-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="be4d4-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="be4d4-211">Response</span></span>
<span data-ttu-id="be4d4-212">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be4d4-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be4d4-213">Пример</span><span class="sxs-lookup"><span data-stu-id="be4d4-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="be4d4-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="be4d4-214">Request</span></span>

<span data-ttu-id="be4d4-215">Ниже приведен пример запроса на следующий рабочий процесс управления устройств:</span><span class="sxs-lookup"><span data-stu-id="be4d4-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="be4d4-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="be4d4-216">Response</span></span>

<span data-ttu-id="be4d4-217">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be4d4-217">Here is an example of the response.</span></span> 

<span data-ttu-id="be4d4-218">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="be4d4-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="be4d4-219">Возвращаемых свойств различаться в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="be4d4-219">Returned properties vary according to workflow and context.</span></span>

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



