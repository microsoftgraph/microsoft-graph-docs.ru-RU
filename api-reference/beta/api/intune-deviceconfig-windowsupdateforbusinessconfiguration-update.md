---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 519be5fca82292360710fcfbee3a52f35b2ed1dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918828"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="8fea2-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fea2-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="8fea2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8fea2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fea2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fea2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fea2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8fea2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fea2-107">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fea2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8fea2-108">Prerequisites</span></span>
<span data-ttu-id="8fea2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fea2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fea2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fea2-111">Permission type</span></span>|<span data-ttu-id="8fea2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fea2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fea2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fea2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fea2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fea2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fea2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fea2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fea2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fea2-116">Not supported.</span></span>|
|<span data-ttu-id="8fea2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fea2-117">Application</span></span>|<span data-ttu-id="8fea2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fea2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fea2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fea2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8fea2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fea2-120">Request headers</span></span>
|<span data-ttu-id="8fea2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fea2-121">Header</span></span>|<span data-ttu-id="8fea2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8fea2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fea2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fea2-123">Authorization</span></span>|<span data-ttu-id="8fea2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8fea2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fea2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8fea2-125">Accept</span></span>|<span data-ttu-id="8fea2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fea2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fea2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8fea2-127">Request body</span></span>
<span data-ttu-id="8fea2-128">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fea2-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="8fea2-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="8fea2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fea2-130">Property</span></span>|<span data-ttu-id="8fea2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8fea2-131">Type</span></span>|<span data-ttu-id="8fea2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8fea2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fea2-133">id</span><span class="sxs-lookup"><span data-stu-id="8fea2-133">id</span></span>|<span data-ttu-id="8fea2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8fea2-134">String</span></span>|<span data-ttu-id="8fea2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8fea2-135">Key of the entity.</span></span> <span data-ttu-id="8fea2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8fea2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fea2-138">DateTimeOffset</span></span>|<span data-ttu-id="8fea2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8fea2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8fea2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8fea2-141">roleScopeTagIds</span></span>|<span data-ttu-id="8fea2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8fea2-142">String collection</span></span>|<span data-ttu-id="8fea2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8fea2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8fea2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8fea2-145">supportsScopeTags</span></span>|<span data-ttu-id="8fea2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8fea2-146">Boolean</span></span>|<span data-ttu-id="8fea2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="8fea2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8fea2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="8fea2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8fea2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8fea2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8fea2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fea2-150">This property is read-only.</span></span> <span data-ttu-id="8fea2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-152">createdDateTime</span></span>|<span data-ttu-id="8fea2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fea2-153">DateTimeOffset</span></span>|<span data-ttu-id="8fea2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8fea2-154">DateTime the object was created.</span></span> <span data-ttu-id="8fea2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-156">описание</span><span class="sxs-lookup"><span data-stu-id="8fea2-156">description</span></span>|<span data-ttu-id="8fea2-157">Строка</span><span class="sxs-lookup"><span data-stu-id="8fea2-157">String</span></span>|<span data-ttu-id="8fea2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8fea2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8fea2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8fea2-160">displayName</span></span>|<span data-ttu-id="8fea2-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8fea2-161">String</span></span>|<span data-ttu-id="8fea2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8fea2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8fea2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-164">version</span><span class="sxs-lookup"><span data-stu-id="8fea2-164">version</span></span>|<span data-ttu-id="8fea2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-165">Int32</span></span>|<span data-ttu-id="8fea2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8fea2-166">Version of the device configuration.</span></span> <span data-ttu-id="8fea2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fea2-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="8fea2-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="8fea2-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="8fea2-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="8fea2-170">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="8fea2-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="8fea2-171">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="8fea2-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="8fea2-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="8fea2-172">prereleaseFeatures</span></span>|[<span data-ttu-id="8fea2-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="8fea2-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="8fea2-174">Экспериментальные функции.</span><span class="sxs-lookup"><span data-stu-id="8fea2-174">The pre-release features.</span></span> <span data-ttu-id="8fea2-175">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="8fea2-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="8fea2-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="8fea2-176">automaticUpdateMode</span></span>|[<span data-ttu-id="8fea2-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="8fea2-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="8fea2-178">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="8fea2-178">Automatic update mode.</span></span> <span data-ttu-id="8fea2-179">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="8fea2-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="8fea2-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="8fea2-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="8fea2-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fea2-181">Boolean</span></span>|<span data-ttu-id="8fea2-182">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8fea2-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="8fea2-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="8fea2-183">driversExcluded</span></span>|<span data-ttu-id="8fea2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fea2-184">Boolean</span></span>|<span data-ttu-id="8fea2-185">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="8fea2-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="8fea2-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="8fea2-186">installationSchedule</span></span>|[<span data-ttu-id="8fea2-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="8fea2-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="8fea2-188">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="8fea2-188">Installation schedule</span></span>|
|<span data-ttu-id="8fea2-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="8fea2-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="8fea2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-190">Int32</span></span>|<span data-ttu-id="8fea2-191">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="8fea2-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="8fea2-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="8fea2-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="8fea2-193">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-193">Int32</span></span>|<span data-ttu-id="8fea2-194">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="8fea2-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="8fea2-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="8fea2-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="8fea2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fea2-196">Boolean</span></span>|<span data-ttu-id="8fea2-197">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="8fea2-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="8fea2-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="8fea2-198">featureUpdatesPaused</span></span>|<span data-ttu-id="8fea2-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fea2-199">Boolean</span></span>|<span data-ttu-id="8fea2-200">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="8fea2-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="8fea2-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="8fea2-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fea2-202">DateTimeOffset</span></span>|<span data-ttu-id="8fea2-203">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="8fea2-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="8fea2-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="8fea2-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fea2-205">DateTimeOffset</span></span>|<span data-ttu-id="8fea2-206">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="8fea2-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="8fea2-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="8fea2-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="8fea2-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="8fea2-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="8fea2-209">Определяет, какие устройства филиала будет получать обновления из.</span><span class="sxs-lookup"><span data-stu-id="8fea2-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="8fea2-210">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="8fea2-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="8fea2-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="8fea2-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="8fea2-212">Логический</span><span class="sxs-lookup"><span data-stu-id="8fea2-212">Boolean</span></span>|<span data-ttu-id="8fea2-213">Задайте для всех проверку перед перезагрузкой: уровень батарей = 40%, сведения о присутствии пользователя необходимости отображения, режиме презентации, полноэкранный режим, состояние телефонный звонок, режим игры и т.д.</span><span class="sxs-lookup"><span data-stu-id="8fea2-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="8fea2-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="8fea2-214">updateWeeks</span></span>|[<span data-ttu-id="8fea2-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="8fea2-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="8fea2-216">Планирование установки обновления на недели, месяца.</span><span class="sxs-lookup"><span data-stu-id="8fea2-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="8fea2-217">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="8fea2-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="8fea2-218">qualityUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-218">qualityUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="8fea2-219">Строка</span><span class="sxs-lookup"><span data-stu-id="8fea2-219">String</span></span>|<span data-ttu-id="8fea2-220">Запуск обновления приостановить datetime качества</span><span class="sxs-lookup"><span data-stu-id="8fea2-220">Quality Updates Pause Start datetime</span></span>|
|<span data-ttu-id="8fea2-221">featureUpdatesPauseStartDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-221">featureUpdatesPauseStartDateTime</span></span>|<span data-ttu-id="8fea2-222">Строка</span><span class="sxs-lookup"><span data-stu-id="8fea2-222">String</span></span>|<span data-ttu-id="8fea2-223">Функция начать приостановить обновления даты и времени</span><span class="sxs-lookup"><span data-stu-id="8fea2-223">Feature Updates Pause Start datetime</span></span>|
|<span data-ttu-id="8fea2-224">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="8fea2-224">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="8fea2-225">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-225">Int32</span></span>|<span data-ttu-id="8fea2-226">Число дней после обновления компонента, для которого отката является допустимым</span><span class="sxs-lookup"><span data-stu-id="8fea2-226">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="8fea2-227">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="8fea2-227">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="8fea2-228">Логический</span><span class="sxs-lookup"><span data-stu-id="8fea2-228">Boolean</span></span>|<span data-ttu-id="8fea2-229">Определяет, будет ли отката обновлений качества на следующего устройства проверку</span><span class="sxs-lookup"><span data-stu-id="8fea2-229">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="8fea2-230">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="8fea2-230">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="8fea2-231">Логический</span><span class="sxs-lookup"><span data-stu-id="8fea2-231">Boolean</span></span>|<span data-ttu-id="8fea2-232">Определяет, нужно ли выполнить откат обновления компонента на следующего устройства проверку</span><span class="sxs-lookup"><span data-stu-id="8fea2-232">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="8fea2-233">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-233">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="8fea2-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fea2-234">DateTimeOffset</span></span>|<span data-ttu-id="8fea2-235">Качество запуск отката обновления даты и времени</span><span class="sxs-lookup"><span data-stu-id="8fea2-235">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="8fea2-236">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="8fea2-236">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="8fea2-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fea2-237">DateTimeOffset</span></span>|<span data-ttu-id="8fea2-238">Запуск отката обновления даты и времени в функциях</span><span class="sxs-lookup"><span data-stu-id="8fea2-238">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="8fea2-239">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="8fea2-239">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="8fea2-240">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-240">Int32</span></span>|<span data-ttu-id="8fea2-241">Крайний срок в днях, прежде чем автоматически планирование и выполнение отложенная перезагрузка active часы с допустимый диапазон от 2 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="8fea2-241">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="8fea2-242">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="8fea2-242">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="8fea2-243">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-243">Int32</span></span>|<span data-ttu-id="8fea2-244">Количество дней, пользователь может отложить выполняет перезапуск почте напоминания с допустимые значения от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="8fea2-244">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="8fea2-245">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="8fea2-245">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="8fea2-246">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-246">Int32</span></span>|<span data-ttu-id="8fea2-247">Количество дней до переход от автоматически перезапустит вне active часов выполняет перезапуск, с помощью которого пользователь может планировать с допустимый диапазон: от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="8fea2-247">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="8fea2-248">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="8fea2-248">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="8fea2-249">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="8fea2-249">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="8fea2-250">Выбор метода, с помощью которого перезапуск обязательные закрытия уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8fea2-250">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="8fea2-251">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8fea2-251">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="8fea2-252">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="8fea2-252">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="8fea2-253">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-253">Int32</span></span>|<span data-ttu-id="8fea2-254">Укажите период для напоминания о автоматическую перезагрузку предупреждений.</span><span class="sxs-lookup"><span data-stu-id="8fea2-254">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="8fea2-255">Поддерживаемые значения: 2, 4, 8, 12 или 24 (в часах).</span><span class="sxs-lookup"><span data-stu-id="8fea2-255">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="8fea2-256">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="8fea2-256">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="8fea2-257">Int32</span><span class="sxs-lookup"><span data-stu-id="8fea2-257">Int32</span></span>|<span data-ttu-id="8fea2-258">Укажите период для автоматическую перезагрузку предстоящее предупреждений.</span><span class="sxs-lookup"><span data-stu-id="8fea2-258">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="8fea2-259">Поддерживаемые значения: 15, 30 или 60 (в минутах).</span><span class="sxs-lookup"><span data-stu-id="8fea2-259">Supported values: 15, 30 or 60 (minutes).</span></span>|



## <a name="response"></a><span data-ttu-id="8fea2-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fea2-260">Response</span></span>
<span data-ttu-id="8fea2-261">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8fea2-261">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fea2-262">Пример</span><span class="sxs-lookup"><span data-stu-id="8fea2-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fea2-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fea2-263">Request</span></span>
<span data-ttu-id="8fea2-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fea2-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7
}
```

### <a name="response"></a><span data-ttu-id="8fea2-265">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fea2-265">Response</span></span>
<span data-ttu-id="8fea2-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8fea2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1971

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
  "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7
}
```





