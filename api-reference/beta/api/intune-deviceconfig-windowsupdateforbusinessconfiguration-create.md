---
title: Create windowsUpdateForBusinessConfiguration
description: Создание объекта windowsUpdateForBusinessConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dade72412a64b5703fa253eda0a40829f2475549
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406194"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="4e8b6-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e8b6-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="4e8b6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e8b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e8b6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e8b6-107">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-107">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e8b6-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4e8b6-108">Prerequisites</span></span>
<span data-ttu-id="4e8b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e8b6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e8b6-111">Permission type</span></span>|<span data-ttu-id="4e8b6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e8b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e8b6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e8b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e8b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e8b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e8b6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e8b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e8b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-116">Not supported.</span></span>|
|<span data-ttu-id="4e8b6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e8b6-117">Application</span></span>|<span data-ttu-id="4e8b6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e8b6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e8b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e8b6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e8b6-120">Request headers</span></span>
|<span data-ttu-id="4e8b6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e8b6-121">Header</span></span>|<span data-ttu-id="4e8b6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e8b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e8b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e8b6-123">Authorization</span></span>|<span data-ttu-id="4e8b6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e8b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e8b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e8b6-125">Accept</span></span>|<span data-ttu-id="4e8b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e8b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e8b6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e8b6-127">Request body</span></span>
<span data-ttu-id="4e8b6-128">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-128">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="4e8b6-129">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-129">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="4e8b6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e8b6-130">Property</span></span>|<span data-ttu-id="4e8b6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e8b6-131">Type</span></span>|<span data-ttu-id="4e8b6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e8b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e8b6-133">id</span><span class="sxs-lookup"><span data-stu-id="4e8b6-133">id</span></span>|<span data-ttu-id="4e8b6-134">String</span><span class="sxs-lookup"><span data-stu-id="4e8b6-134">String</span></span>|<span data-ttu-id="4e8b6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-135">Key of the entity.</span></span> <span data-ttu-id="4e8b6-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8b6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4e8b6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8b6-138">DateTimeOffset</span></span>|<span data-ttu-id="4e8b6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4e8b6-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e8b6-141">roleScopeTagIds</span></span>|<span data-ttu-id="4e8b6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4e8b6-142">String collection</span></span>|<span data-ttu-id="4e8b6-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4e8b6-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4e8b6-145">supportsScopeTags</span></span>|<span data-ttu-id="4e8b6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="4e8b6-146">Boolean</span></span>|<span data-ttu-id="4e8b6-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4e8b6-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4e8b6-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4e8b6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-150">This property is read-only.</span></span> <span data-ttu-id="4e8b6-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8b6-152">createdDateTime</span></span>|<span data-ttu-id="4e8b6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8b6-153">DateTimeOffset</span></span>|<span data-ttu-id="4e8b6-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-154">DateTime the object was created.</span></span> <span data-ttu-id="4e8b6-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-156">description</span><span class="sxs-lookup"><span data-stu-id="4e8b6-156">description</span></span>|<span data-ttu-id="4e8b6-157">String</span><span class="sxs-lookup"><span data-stu-id="4e8b6-157">String</span></span>|<span data-ttu-id="4e8b6-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4e8b6-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4e8b6-160">displayName</span></span>|<span data-ttu-id="4e8b6-161">String</span><span class="sxs-lookup"><span data-stu-id="4e8b6-161">String</span></span>|<span data-ttu-id="4e8b6-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4e8b6-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-164">version</span><span class="sxs-lookup"><span data-stu-id="4e8b6-164">version</span></span>|<span data-ttu-id="4e8b6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-165">Int32</span></span>|<span data-ttu-id="4e8b6-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-166">Version of the device configuration.</span></span> <span data-ttu-id="4e8b6-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e8b6-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4e8b6-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="4e8b6-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4e8b6-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="4e8b6-170">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-170">Delivery Optimization Mode.</span></span> <span data-ttu-id="4e8b6-171">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="4e8b6-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="4e8b6-172">prereleaseFeatures</span></span>|[<span data-ttu-id="4e8b6-173">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="4e8b6-173">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="4e8b6-174">Экспериментальные функции.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-174">The pre-release features.</span></span> <span data-ttu-id="4e8b6-175">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-175">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="4e8b6-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="4e8b6-176">automaticUpdateMode</span></span>|[<span data-ttu-id="4e8b6-177">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="4e8b6-177">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="4e8b6-178">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-178">Automatic update mode.</span></span> <span data-ttu-id="4e8b6-179">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-179">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="4e8b6-180">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="4e8b6-180">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="4e8b6-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e8b6-181">Boolean</span></span>|<span data-ttu-id="4e8b6-182">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-182">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="4e8b6-183">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="4e8b6-183">driversExcluded</span></span>|<span data-ttu-id="4e8b6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e8b6-184">Boolean</span></span>|<span data-ttu-id="4e8b6-185">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-185">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="4e8b6-186">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="4e8b6-186">installationSchedule</span></span>|[<span data-ttu-id="4e8b6-187">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="4e8b6-187">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="4e8b6-188">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-188">Installation schedule</span></span>|
|<span data-ttu-id="4e8b6-189">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="4e8b6-189">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="4e8b6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-190">Int32</span></span>|<span data-ttu-id="4e8b6-191">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-191">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="4e8b6-192">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="4e8b6-192">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="4e8b6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-193">Int32</span></span>|<span data-ttu-id="4e8b6-194">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-194">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="4e8b6-195">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="4e8b6-195">qualityUpdatesPaused</span></span>|<span data-ttu-id="4e8b6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e8b6-196">Boolean</span></span>|<span data-ttu-id="4e8b6-197">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-197">Pause Quality Updates</span></span>|
|<span data-ttu-id="4e8b6-198">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="4e8b6-198">featureUpdatesPaused</span></span>|<span data-ttu-id="4e8b6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e8b6-199">Boolean</span></span>|<span data-ttu-id="4e8b6-200">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-200">Pause Feature Updates</span></span>|
|<span data-ttu-id="4e8b6-201">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8b6-201">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="4e8b6-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8b6-202">DateTimeOffset</span></span>|<span data-ttu-id="4e8b6-203">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-203">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="4e8b6-204">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8b6-204">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="4e8b6-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8b6-205">DateTimeOffset</span></span>|<span data-ttu-id="4e8b6-206">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-206">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="4e8b6-207">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="4e8b6-207">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="4e8b6-208">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="4e8b6-208">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="4e8b6-209">Определяет, какие устройства филиала будет получать обновления из.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-209">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="4e8b6-210">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-210">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="4e8b6-211">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="4e8b6-211">skipChecksBeforeRestart</span></span>|<span data-ttu-id="4e8b6-212">Логический</span><span class="sxs-lookup"><span data-stu-id="4e8b6-212">Boolean</span></span>|<span data-ttu-id="4e8b6-213">Задайте для всех проверку перед перезагрузкой: уровень батарей = 40%, сведения о присутствии пользователя необходимости отображения, режиме презентации, полноэкранный режим, состояние телефонный звонок, режим игры и т.д.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-213">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="4e8b6-214">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="4e8b6-214">updateWeeks</span></span>|[<span data-ttu-id="4e8b6-215">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="4e8b6-215">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="4e8b6-216">Планирование установки обновления на недели, месяца.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-216">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="4e8b6-217">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-217">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="4e8b6-218">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="4e8b6-218">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="4e8b6-219">дата;</span><span class="sxs-lookup"><span data-stu-id="4e8b6-219">Date</span></span>|<span data-ttu-id="4e8b6-220">Дата начала обновления приостановить качества.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-220">Quality Updates Pause start date.</span></span> <span data-ttu-id="4e8b6-221">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-221">This property is read-only.</span></span>|
|<span data-ttu-id="4e8b6-222">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="4e8b6-222">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="4e8b6-223">дата;</span><span class="sxs-lookup"><span data-stu-id="4e8b6-223">Date</span></span>|<span data-ttu-id="4e8b6-224">Дата начала приостановить обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-224">Feature Updates Pause start date.</span></span> <span data-ttu-id="4e8b6-225">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-225">This property is read-only.</span></span>|
|<span data-ttu-id="4e8b6-226">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="4e8b6-226">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="4e8b6-227">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-227">Int32</span></span>|<span data-ttu-id="4e8b6-228">Число дней после обновления компонента, для которого отката является допустимым</span><span class="sxs-lookup"><span data-stu-id="4e8b6-228">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="4e8b6-229">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="4e8b6-229">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="4e8b6-230">Логический</span><span class="sxs-lookup"><span data-stu-id="4e8b6-230">Boolean</span></span>|<span data-ttu-id="4e8b6-231">Определяет, будет ли отката обновлений качества на следующего устройства проверку</span><span class="sxs-lookup"><span data-stu-id="4e8b6-231">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="4e8b6-232">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="4e8b6-232">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="4e8b6-233">Логический</span><span class="sxs-lookup"><span data-stu-id="4e8b6-233">Boolean</span></span>|<span data-ttu-id="4e8b6-234">Определяет, нужно ли выполнить откат обновления компонента на следующего устройства проверку</span><span class="sxs-lookup"><span data-stu-id="4e8b6-234">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="4e8b6-235">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8b6-235">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="4e8b6-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8b6-236">DateTimeOffset</span></span>|<span data-ttu-id="4e8b6-237">Качество запуск отката обновления даты и времени</span><span class="sxs-lookup"><span data-stu-id="4e8b6-237">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="4e8b6-238">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8b6-238">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="4e8b6-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8b6-239">DateTimeOffset</span></span>|<span data-ttu-id="4e8b6-240">Запуск отката обновления даты и времени в функциях</span><span class="sxs-lookup"><span data-stu-id="4e8b6-240">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="4e8b6-241">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="4e8b6-241">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="4e8b6-242">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-242">Int32</span></span>|<span data-ttu-id="4e8b6-243">Крайний срок в днях, прежде чем автоматически планирование и выполнение отложенная перезагрузка active часы с допустимый диапазон от 2 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="4e8b6-243">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="4e8b6-244">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="4e8b6-244">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="4e8b6-245">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-245">Int32</span></span>|<span data-ttu-id="4e8b6-246">Количество дней, пользователь может отложить выполняет перезапуск почте напоминания с допустимые значения от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="4e8b6-246">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="4e8b6-247">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="4e8b6-247">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="4e8b6-248">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-248">Int32</span></span>|<span data-ttu-id="4e8b6-249">Количество дней до переход от автоматически перезапустит вне active часов выполняет перезапуск, с помощью которого пользователь может планировать с допустимый диапазон: от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="4e8b6-249">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="4e8b6-250">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="4e8b6-250">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="4e8b6-251">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="4e8b6-251">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="4e8b6-252">Выбор метода, с помощью которого перезапуск обязательные закрытия уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-252">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="4e8b6-253">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-253">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="4e8b6-254">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="4e8b6-254">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="4e8b6-255">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-255">Int32</span></span>|<span data-ttu-id="4e8b6-256">Укажите период для напоминания о автоматическую перезагрузку предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-256">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="4e8b6-257">Поддерживаемые значения: 2, 4, 8, 12 или 24 (в часах).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-257">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="4e8b6-258">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="4e8b6-258">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="4e8b6-259">Int32</span><span class="sxs-lookup"><span data-stu-id="4e8b6-259">Int32</span></span>|<span data-ttu-id="4e8b6-260">Укажите период для автоматическую перезагрузку предстоящее предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-260">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="4e8b6-261">Поддерживаемые значения: 15, 30 или 60 (в минутах).</span><span class="sxs-lookup"><span data-stu-id="4e8b6-261">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="4e8b6-262">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="4e8b6-262">userPauseAccess</span></span>|<span data-ttu-id="4e8b6-263">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="4e8b6-263">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="4e8b6-264">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="4e8b6-264">.md)</span></span>|<span data-ttu-id="4e8b6-265">Указывает, следует ли включить доступа конечных пользователей для приостановки обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-265">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="4e8b6-266">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-266">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="4e8b6-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e8b6-267">Response</span></span>
<span data-ttu-id="4e8b6-268">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-268">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e8b6-269">Пример</span><span class="sxs-lookup"><span data-stu-id="4e8b6-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e8b6-270">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e8b6-270">Request</span></span>
<span data-ttu-id="4e8b6-271">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1804

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
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
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="4e8b6-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e8b6-272">Response</span></span>
<span data-ttu-id="4e8b6-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4e8b6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1976

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
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
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
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled"
}
```




