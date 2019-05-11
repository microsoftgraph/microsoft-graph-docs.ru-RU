---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 900043e6ff08a889ce1f34a8701d485fac506b9c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933188"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="8502b-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8502b-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8502b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8502b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8502b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8502b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8502b-106">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8502b-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8502b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8502b-107">Prerequisites</span></span>
<span data-ttu-id="8502b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8502b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8502b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8502b-110">Permission type</span></span>|<span data-ttu-id="8502b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8502b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8502b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8502b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8502b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8502b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8502b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8502b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8502b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8502b-115">Not supported.</span></span>|
|<span data-ttu-id="8502b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8502b-116">Application</span></span>|<span data-ttu-id="8502b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8502b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8502b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8502b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8502b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8502b-119">Request headers</span></span>
|<span data-ttu-id="8502b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8502b-120">Header</span></span>|<span data-ttu-id="8502b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8502b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8502b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8502b-122">Authorization</span></span>|<span data-ttu-id="8502b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8502b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8502b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8502b-124">Accept</span></span>|<span data-ttu-id="8502b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8502b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8502b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8502b-126">Request body</span></span>
<span data-ttu-id="8502b-127">В тексте запроса добавьте представление объекта [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8502b-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="8502b-128">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="8502b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8502b-129">Property</span></span>|<span data-ttu-id="8502b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8502b-130">Type</span></span>|<span data-ttu-id="8502b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8502b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8502b-132">id</span><span class="sxs-lookup"><span data-stu-id="8502b-132">id</span></span>|<span data-ttu-id="8502b-133">String</span><span class="sxs-lookup"><span data-stu-id="8502b-133">String</span></span>|<span data-ttu-id="8502b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8502b-134">Key of the entity.</span></span> <span data-ttu-id="8502b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8502b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8502b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8502b-137">DateTimeOffset</span></span>|<span data-ttu-id="8502b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8502b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8502b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8502b-140">roleScopeTagIds</span></span>|<span data-ttu-id="8502b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8502b-141">String collection</span></span>|<span data-ttu-id="8502b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8502b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8502b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8502b-144">supportsScopeTags</span></span>|<span data-ttu-id="8502b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-145">Boolean</span></span>|<span data-ttu-id="8502b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8502b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8502b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8502b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8502b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8502b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8502b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8502b-149">This property is read-only.</span></span> <span data-ttu-id="8502b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8502b-151">createdDateTime</span></span>|<span data-ttu-id="8502b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8502b-152">DateTimeOffset</span></span>|<span data-ttu-id="8502b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8502b-153">DateTime the object was created.</span></span> <span data-ttu-id="8502b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-155">description</span><span class="sxs-lookup"><span data-stu-id="8502b-155">description</span></span>|<span data-ttu-id="8502b-156">String</span><span class="sxs-lookup"><span data-stu-id="8502b-156">String</span></span>|<span data-ttu-id="8502b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8502b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8502b-159">displayName</span></span>|<span data-ttu-id="8502b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="8502b-160">String</span></span>|<span data-ttu-id="8502b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8502b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-163">version</span><span class="sxs-lookup"><span data-stu-id="8502b-163">version</span></span>|<span data-ttu-id="8502b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-164">Int32</span></span>|<span data-ttu-id="8502b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-165">Version of the device configuration.</span></span> <span data-ttu-id="8502b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8502b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8502b-167">Аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="8502b-167">accountsBlockModification</span></span>|<span data-ttu-id="8502b-168">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-168">Boolean</span></span>|<span data-ttu-id="8502b-169">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="8502b-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="8502b-170">Аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="8502b-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="8502b-171">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-171">Boolean</span></span>|<span data-ttu-id="8502b-172">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="8502b-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="8502b-173">Аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="8502b-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="8502b-174">Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="8502b-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="8502b-175">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="8502b-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="8502b-176">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="8502b-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="8502b-177">Аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="8502b-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="8502b-178">Андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="8502b-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="8502b-179">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="8502b-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="8502b-180">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="8502b-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="8502b-181">Аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="8502b-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="8502b-182">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-182">Boolean</span></span>|<span data-ttu-id="8502b-183">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="8502b-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="8502b-184">Блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8502b-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="8502b-185">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-185">Boolean</span></span>|<span data-ttu-id="8502b-186">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8502b-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="8502b-187">Блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="8502b-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="8502b-188">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-188">Boolean</span></span>|<span data-ttu-id="8502b-189">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8502b-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="8502b-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8502b-190">cameraBlocked</span></span>|<span data-ttu-id="8502b-191">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-191">Boolean</span></span>|<span data-ttu-id="8502b-192">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="8502b-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="8502b-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="8502b-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="8502b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8502b-194">Boolean</span></span>|<span data-ttu-id="8502b-195">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8502b-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="8502b-196">Датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="8502b-196">dataRoamingBlocked</span></span>|<span data-ttu-id="8502b-197">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-197">Boolean</span></span>|<span data-ttu-id="8502b-198">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="8502b-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="8502b-199">Датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="8502b-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="8502b-200">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-200">Boolean</span></span>|<span data-ttu-id="8502b-201">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8502b-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="8502b-202">Факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="8502b-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="8502b-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8502b-203">String collection</span></span>|<span data-ttu-id="8502b-204">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="8502b-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="8502b-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="8502b-205">factoryResetBlocked</span></span>|<span data-ttu-id="8502b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="8502b-206">Boolean</span></span>|<span data-ttu-id="8502b-207">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="8502b-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="8502b-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="8502b-208">kioskModeApps</span></span>|<span data-ttu-id="8502b-209">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8502b-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8502b-210">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8502b-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="8502b-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8502b-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8502b-212">Киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="8502b-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="8502b-213">Строка</span><span class="sxs-lookup"><span data-stu-id="8502b-213">String</span></span>|<span data-ttu-id="8502b-214">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8502b-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8502b-215">Киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="8502b-215">kioskModeExitCode</span></span>|<span data-ttu-id="8502b-216">Строка</span><span class="sxs-lookup"><span data-stu-id="8502b-216">String</span></span>|<span data-ttu-id="8502b-217">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8502b-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8502b-218">Киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="8502b-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="8502b-219">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-219">Boolean</span></span>|<span data-ttu-id="8502b-220">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8502b-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8502b-221">Киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8502b-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="8502b-222">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-222">Boolean</span></span>|<span data-ttu-id="8502b-223">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8502b-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8502b-224">Киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8502b-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="8502b-225">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-225">Boolean</span></span>|<span data-ttu-id="8502b-226">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8502b-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8502b-227">Микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="8502b-227">microphoneForceMute</span></span>|<span data-ttu-id="8502b-228">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-228">Boolean</span></span>|<span data-ttu-id="8502b-229">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="8502b-230">Нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="8502b-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="8502b-231">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-231">Boolean</span></span>|<span data-ttu-id="8502b-232">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="8502b-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="8502b-233">Нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="8502b-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="8502b-234">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-234">Boolean</span></span>|<span data-ttu-id="8502b-235">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="8502b-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="8502b-236">Пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="8502b-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="8502b-237">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-237">Boolean</span></span>|<span data-ttu-id="8502b-238">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="8502b-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="8502b-239">Пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="8502b-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="8502b-240">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="8502b-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="8502b-241">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="8502b-241">List of device keyguard features to block.</span></span> <span data-ttu-id="8502b-242">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="8502b-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8502b-243">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="8502b-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="8502b-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8502b-244">passwordExpirationDays</span></span>|<span data-ttu-id="8502b-245">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-245">Int32</span></span>|<span data-ttu-id="8502b-246">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="8502b-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="8502b-247">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="8502b-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8502b-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8502b-248">passwordMinimumLength</span></span>|<span data-ttu-id="8502b-249">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-249">Int32</span></span>|<span data-ttu-id="8502b-250">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="8502b-251">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8502b-252">Пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="8502b-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="8502b-253">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-253">Int32</span></span>|<span data-ttu-id="8502b-254">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="8502b-255">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8502b-256">Пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="8502b-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="8502b-257">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-257">Int32</span></span>|<span data-ttu-id="8502b-258">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="8502b-259">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8502b-260">Пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="8502b-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="8502b-261">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-261">Int32</span></span>|<span data-ttu-id="8502b-262">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="8502b-263">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8502b-264">Пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="8502b-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="8502b-265">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-265">Int32</span></span>|<span data-ttu-id="8502b-266">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="8502b-267">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8502b-268">Пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="8502b-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="8502b-269">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-269">Int32</span></span>|<span data-ttu-id="8502b-270">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="8502b-271">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8502b-272">Пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="8502b-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="8502b-273">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-273">Int32</span></span>|<span data-ttu-id="8502b-274">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="8502b-275">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8502b-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8502b-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8502b-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8502b-277">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-277">Int32</span></span>|<span data-ttu-id="8502b-278">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="8502b-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8502b-279">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="8502b-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="8502b-280">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-280">Int32</span></span>|<span data-ttu-id="8502b-281">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="8502b-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="8502b-282">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="8502b-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8502b-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8502b-283">passwordRequiredType</span></span>|[<span data-ttu-id="8502b-284">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="8502b-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="8502b-285">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="8502b-286">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="8502b-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="8502b-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8502b-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8502b-288">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-288">Int32</span></span>|<span data-ttu-id="8502b-289">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="8502b-290">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="8502b-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="8502b-291">Плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="8502b-291">playStoreMode</span></span>|[<span data-ttu-id="8502b-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="8502b-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="8502b-293">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="8502b-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="8502b-294">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="8502b-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="8502b-295">Сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="8502b-295">safeBootBlocked</span></span>|<span data-ttu-id="8502b-296">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-296">Boolean</span></span>|<span data-ttu-id="8502b-297">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="8502b-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="8502b-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8502b-298">screenCaptureBlocked</span></span>|<span data-ttu-id="8502b-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="8502b-299">Boolean</span></span>|<span data-ttu-id="8502b-300">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="8502b-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="8502b-301">Секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="8502b-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="8502b-302">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-302">Boolean</span></span>|<span data-ttu-id="8502b-303">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8502b-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="8502b-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8502b-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="8502b-305">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-305">Boolean</span></span>|<span data-ttu-id="8502b-306">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="8502b-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="8502b-307">Статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="8502b-307">statusBarBlocked</span></span>|<span data-ttu-id="8502b-308">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-308">Boolean</span></span>|<span data-ttu-id="8502b-309">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="8502b-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="8502b-310">Стайонмодес</span><span class="sxs-lookup"><span data-stu-id="8502b-310">stayOnModes</span></span>|<span data-ttu-id="8502b-311">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="8502b-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="8502b-312">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="8502b-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="8502b-313">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="8502b-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="8502b-314">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="8502b-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="8502b-315">Сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="8502b-315">storageAllowUsb</span></span>|<span data-ttu-id="8502b-316">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-316">Boolean</span></span>|<span data-ttu-id="8502b-317">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="8502b-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="8502b-318">Сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="8502b-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="8502b-319">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-319">Boolean</span></span>|<span data-ttu-id="8502b-320">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="8502b-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="8502b-321">Сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="8502b-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="8502b-322">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-322">Boolean</span></span>|<span data-ttu-id="8502b-323">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="8502b-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="8502b-324">Системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="8502b-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="8502b-325">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-325">Int32</span></span>|<span data-ttu-id="8502b-326">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="8502b-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="8502b-327">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8502b-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8502b-328">Системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="8502b-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="8502b-329">Int32</span><span class="sxs-lookup"><span data-stu-id="8502b-329">Int32</span></span>|<span data-ttu-id="8502b-330">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="8502b-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="8502b-331">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8502b-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8502b-332">Системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="8502b-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="8502b-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8502b-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="8502b-334">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="8502b-334">The type of system update configuration.</span></span> <span data-ttu-id="8502b-335">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="8502b-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="8502b-336">Системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="8502b-336">systemWindowsBlocked</span></span>|<span data-ttu-id="8502b-337">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-337">Boolean</span></span>|<span data-ttu-id="8502b-338">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="8502b-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="8502b-339">Усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="8502b-339">usersBlockAdd</span></span>|<span data-ttu-id="8502b-340">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-340">Boolean</span></span>|<span data-ttu-id="8502b-341">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="8502b-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="8502b-342">Усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="8502b-342">usersBlockRemove</span></span>|<span data-ttu-id="8502b-343">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-343">Boolean</span></span>|<span data-ttu-id="8502b-344">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="8502b-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="8502b-345">Волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="8502b-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="8502b-346">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-346">Boolean</span></span>|<span data-ttu-id="8502b-347">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="8502b-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="8502b-348">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="8502b-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="8502b-349">Строка</span><span class="sxs-lookup"><span data-stu-id="8502b-349">String</span></span>|<span data-ttu-id="8502b-350">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="8502b-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="8502b-351">Впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="8502b-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="8502b-352">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-352">Boolean</span></span>|<span data-ttu-id="8502b-353">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="8502b-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="8502b-354">Вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="8502b-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="8502b-355">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-355">Boolean</span></span>|<span data-ttu-id="8502b-356">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="8502b-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="8502b-357">Вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="8502b-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="8502b-358">Логический</span><span class="sxs-lookup"><span data-stu-id="8502b-358">Boolean</span></span>|<span data-ttu-id="8502b-359">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="8502b-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8502b-360">Отклик</span><span class="sxs-lookup"><span data-stu-id="8502b-360">Response</span></span>
<span data-ttu-id="8502b-361">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8502b-361">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8502b-362">Пример</span><span class="sxs-lookup"><span data-stu-id="8502b-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="8502b-363">Запрос</span><span class="sxs-lookup"><span data-stu-id="8502b-363">Request</span></span>
<span data-ttu-id="8502b-364">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8502b-364">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2905

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="8502b-365">Отклик</span><span class="sxs-lookup"><span data-stu-id="8502b-365">Response</span></span>
<span data-ttu-id="8502b-p130">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8502b-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3077

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




