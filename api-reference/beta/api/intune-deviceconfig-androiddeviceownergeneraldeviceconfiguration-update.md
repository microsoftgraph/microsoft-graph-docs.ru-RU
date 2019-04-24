---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fad142a5ec0f069c40185a40865e29ddee894789
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32480473"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="1aa90-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1aa90-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1aa90-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aa90-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1aa90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aa90-106">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1aa90-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aa90-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1aa90-107">Prerequisites</span></span>
<span data-ttu-id="1aa90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aa90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aa90-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa90-110">Permission type</span></span>|<span data-ttu-id="1aa90-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aa90-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aa90-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aa90-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1aa90-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aa90-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1aa90-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aa90-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aa90-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa90-115">Not supported.</span></span>|
|<span data-ttu-id="1aa90-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aa90-116">Application</span></span>|<span data-ttu-id="1aa90-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa90-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aa90-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aa90-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1aa90-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aa90-119">Request headers</span></span>
|<span data-ttu-id="1aa90-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1aa90-120">Header</span></span>|<span data-ttu-id="1aa90-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1aa90-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aa90-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1aa90-122">Authorization</span></span>|<span data-ttu-id="1aa90-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1aa90-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aa90-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1aa90-124">Accept</span></span>|<span data-ttu-id="1aa90-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1aa90-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aa90-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1aa90-126">Request body</span></span>
<span data-ttu-id="1aa90-127">В тексте запроса добавьте представление объекта [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1aa90-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1aa90-128">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1aa90-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1aa90-129">Property</span></span>|<span data-ttu-id="1aa90-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1aa90-130">Type</span></span>|<span data-ttu-id="1aa90-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa90-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aa90-132">id</span><span class="sxs-lookup"><span data-stu-id="1aa90-132">id</span></span>|<span data-ttu-id="1aa90-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1aa90-133">String</span></span>|<span data-ttu-id="1aa90-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1aa90-134">Key of the entity.</span></span> <span data-ttu-id="1aa90-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa90-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1aa90-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa90-137">DateTimeOffset</span></span>|<span data-ttu-id="1aa90-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1aa90-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1aa90-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1aa90-140">roleScopeTagIds</span></span>|<span data-ttu-id="1aa90-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1aa90-141">String collection</span></span>|<span data-ttu-id="1aa90-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1aa90-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1aa90-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1aa90-144">supportsScopeTags</span></span>|<span data-ttu-id="1aa90-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-145">Boolean</span></span>|<span data-ttu-id="1aa90-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1aa90-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1aa90-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1aa90-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1aa90-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1aa90-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1aa90-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1aa90-149">This property is read-only.</span></span> <span data-ttu-id="1aa90-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa90-151">createdDateTime</span></span>|<span data-ttu-id="1aa90-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa90-152">DateTimeOffset</span></span>|<span data-ttu-id="1aa90-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1aa90-153">DateTime the object was created.</span></span> <span data-ttu-id="1aa90-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-155">description</span><span class="sxs-lookup"><span data-stu-id="1aa90-155">description</span></span>|<span data-ttu-id="1aa90-156">String</span><span class="sxs-lookup"><span data-stu-id="1aa90-156">String</span></span>|<span data-ttu-id="1aa90-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1aa90-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1aa90-159">displayName</span></span>|<span data-ttu-id="1aa90-160">String</span><span class="sxs-lookup"><span data-stu-id="1aa90-160">String</span></span>|<span data-ttu-id="1aa90-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1aa90-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-163">version</span><span class="sxs-lookup"><span data-stu-id="1aa90-163">version</span></span>|<span data-ttu-id="1aa90-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-164">Int32</span></span>|<span data-ttu-id="1aa90-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-165">Version of the device configuration.</span></span> <span data-ttu-id="1aa90-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1aa90-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1aa90-167">Аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="1aa90-167">accountsBlockModification</span></span>|<span data-ttu-id="1aa90-168">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-168">Boolean</span></span>|<span data-ttu-id="1aa90-169">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="1aa90-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="1aa90-170">Аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="1aa90-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="1aa90-171">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-171">Boolean</span></span>|<span data-ttu-id="1aa90-172">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="1aa90-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="1aa90-173">Аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="1aa90-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="1aa90-174">Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="1aa90-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="1aa90-175">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="1aa90-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="1aa90-176">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="1aa90-177">Аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="1aa90-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="1aa90-178">Андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="1aa90-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="1aa90-179">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="1aa90-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="1aa90-180">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1aa90-181">Аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="1aa90-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="1aa90-182">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-182">Boolean</span></span>|<span data-ttu-id="1aa90-183">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="1aa90-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="1aa90-184">Блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1aa90-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="1aa90-185">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-185">Boolean</span></span>|<span data-ttu-id="1aa90-186">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="1aa90-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="1aa90-187">Блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="1aa90-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="1aa90-188">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-188">Boolean</span></span>|<span data-ttu-id="1aa90-189">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="1aa90-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="1aa90-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1aa90-190">cameraBlocked</span></span>|<span data-ttu-id="1aa90-191">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-191">Boolean</span></span>|<span data-ttu-id="1aa90-192">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="1aa90-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="1aa90-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="1aa90-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="1aa90-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aa90-194">Boolean</span></span>|<span data-ttu-id="1aa90-195">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="1aa90-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="1aa90-196">Датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="1aa90-196">dataRoamingBlocked</span></span>|<span data-ttu-id="1aa90-197">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-197">Boolean</span></span>|<span data-ttu-id="1aa90-198">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="1aa90-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="1aa90-199">Датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="1aa90-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="1aa90-200">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-200">Boolean</span></span>|<span data-ttu-id="1aa90-201">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1aa90-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="1aa90-202">Факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="1aa90-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="1aa90-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1aa90-203">String collection</span></span>|<span data-ttu-id="1aa90-204">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="1aa90-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="1aa90-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="1aa90-205">factoryResetBlocked</span></span>|<span data-ttu-id="1aa90-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aa90-206">Boolean</span></span>|<span data-ttu-id="1aa90-207">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="1aa90-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="1aa90-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="1aa90-208">kioskModeApps</span></span>|<span data-ttu-id="1aa90-209">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1aa90-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1aa90-210">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1aa90-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="1aa90-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1aa90-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1aa90-212">Киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="1aa90-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="1aa90-213">String</span><span class="sxs-lookup"><span data-stu-id="1aa90-213">String</span></span>|<span data-ttu-id="1aa90-214">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1aa90-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1aa90-215">Киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="1aa90-215">kioskModeExitCode</span></span>|<span data-ttu-id="1aa90-216">String</span><span class="sxs-lookup"><span data-stu-id="1aa90-216">String</span></span>|<span data-ttu-id="1aa90-217">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1aa90-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1aa90-218">Киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="1aa90-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="1aa90-219">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-219">Boolean</span></span>|<span data-ttu-id="1aa90-220">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1aa90-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1aa90-221">Киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1aa90-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="1aa90-222">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-222">Boolean</span></span>|<span data-ttu-id="1aa90-223">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1aa90-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1aa90-224">Киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1aa90-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="1aa90-225">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-225">Boolean</span></span>|<span data-ttu-id="1aa90-226">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1aa90-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1aa90-227">Микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="1aa90-227">microphoneForceMute</span></span>|<span data-ttu-id="1aa90-228">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-228">Boolean</span></span>|<span data-ttu-id="1aa90-229">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="1aa90-230">Нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="1aa90-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="1aa90-231">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-231">Boolean</span></span>|<span data-ttu-id="1aa90-232">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="1aa90-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="1aa90-233">Нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="1aa90-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="1aa90-234">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-234">Boolean</span></span>|<span data-ttu-id="1aa90-235">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="1aa90-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="1aa90-236">Пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="1aa90-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="1aa90-237">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-237">Boolean</span></span>|<span data-ttu-id="1aa90-238">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="1aa90-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="1aa90-239">Пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="1aa90-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="1aa90-240">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="1aa90-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="1aa90-241">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="1aa90-241">List of device keyguard features to block.</span></span> <span data-ttu-id="1aa90-242">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="1aa90-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="1aa90-243">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="1aa90-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1aa90-244">passwordExpirationDays</span></span>|<span data-ttu-id="1aa90-245">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-245">Int32</span></span>|<span data-ttu-id="1aa90-246">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="1aa90-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="1aa90-247">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="1aa90-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1aa90-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1aa90-248">passwordMinimumLength</span></span>|<span data-ttu-id="1aa90-249">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-249">Int32</span></span>|<span data-ttu-id="1aa90-250">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="1aa90-251">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1aa90-252">Пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="1aa90-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="1aa90-253">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-253">Int32</span></span>|<span data-ttu-id="1aa90-254">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="1aa90-255">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1aa90-256">Пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="1aa90-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="1aa90-257">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-257">Int32</span></span>|<span data-ttu-id="1aa90-258">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="1aa90-259">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1aa90-260">Пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="1aa90-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="1aa90-261">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-261">Int32</span></span>|<span data-ttu-id="1aa90-262">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="1aa90-263">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1aa90-264">Пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="1aa90-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="1aa90-265">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-265">Int32</span></span>|<span data-ttu-id="1aa90-266">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="1aa90-267">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1aa90-268">Пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="1aa90-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="1aa90-269">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-269">Int32</span></span>|<span data-ttu-id="1aa90-270">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="1aa90-271">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1aa90-272">Пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="1aa90-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="1aa90-273">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-273">Int32</span></span>|<span data-ttu-id="1aa90-274">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="1aa90-275">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1aa90-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1aa90-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1aa90-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1aa90-277">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-277">Int32</span></span>|<span data-ttu-id="1aa90-278">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="1aa90-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1aa90-279">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="1aa90-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1aa90-280">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-280">Int32</span></span>|<span data-ttu-id="1aa90-281">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="1aa90-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="1aa90-282">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="1aa90-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1aa90-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1aa90-283">passwordRequiredType</span></span>|[<span data-ttu-id="1aa90-284">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1aa90-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1aa90-285">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="1aa90-286">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="1aa90-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1aa90-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1aa90-288">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-288">Int32</span></span>|<span data-ttu-id="1aa90-289">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="1aa90-290">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="1aa90-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1aa90-291">Плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="1aa90-291">playStoreMode</span></span>|[<span data-ttu-id="1aa90-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="1aa90-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="1aa90-293">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="1aa90-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="1aa90-294">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="1aa90-295">Сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="1aa90-295">safeBootBlocked</span></span>|<span data-ttu-id="1aa90-296">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-296">Boolean</span></span>|<span data-ttu-id="1aa90-297">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="1aa90-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="1aa90-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1aa90-298">screenCaptureBlocked</span></span>|<span data-ttu-id="1aa90-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aa90-299">Boolean</span></span>|<span data-ttu-id="1aa90-300">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="1aa90-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="1aa90-301">Секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="1aa90-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="1aa90-302">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-302">Boolean</span></span>|<span data-ttu-id="1aa90-303">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1aa90-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="1aa90-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1aa90-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="1aa90-305">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-305">Boolean</span></span>|<span data-ttu-id="1aa90-306">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="1aa90-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="1aa90-307">Статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="1aa90-307">statusBarBlocked</span></span>|<span data-ttu-id="1aa90-308">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-308">Boolean</span></span>|<span data-ttu-id="1aa90-309">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="1aa90-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="1aa90-310">Стайонмодес</span><span class="sxs-lookup"><span data-stu-id="1aa90-310">stayOnModes</span></span>|<span data-ttu-id="1aa90-311">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="1aa90-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="1aa90-312">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="1aa90-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="1aa90-313">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="1aa90-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="1aa90-314">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="1aa90-315">Сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="1aa90-315">storageAllowUsb</span></span>|<span data-ttu-id="1aa90-316">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-316">Boolean</span></span>|<span data-ttu-id="1aa90-317">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="1aa90-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="1aa90-318">Сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="1aa90-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="1aa90-319">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-319">Boolean</span></span>|<span data-ttu-id="1aa90-320">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="1aa90-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="1aa90-321">Сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="1aa90-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="1aa90-322">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-322">Boolean</span></span>|<span data-ttu-id="1aa90-323">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="1aa90-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="1aa90-324">Системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="1aa90-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="1aa90-325">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-325">Int32</span></span>|<span data-ttu-id="1aa90-326">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="1aa90-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="1aa90-327">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="1aa90-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1aa90-328">Системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="1aa90-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="1aa90-329">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa90-329">Int32</span></span>|<span data-ttu-id="1aa90-330">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="1aa90-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="1aa90-331">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="1aa90-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1aa90-332">Системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="1aa90-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="1aa90-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1aa90-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="1aa90-334">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="1aa90-334">The type of system update configuration.</span></span> <span data-ttu-id="1aa90-335">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="1aa90-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="1aa90-336">Системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="1aa90-336">systemWindowsBlocked</span></span>|<span data-ttu-id="1aa90-337">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-337">Boolean</span></span>|<span data-ttu-id="1aa90-338">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="1aa90-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="1aa90-339">Усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="1aa90-339">usersBlockAdd</span></span>|<span data-ttu-id="1aa90-340">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-340">Boolean</span></span>|<span data-ttu-id="1aa90-341">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="1aa90-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="1aa90-342">Усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="1aa90-342">usersBlockRemove</span></span>|<span data-ttu-id="1aa90-343">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-343">Boolean</span></span>|<span data-ttu-id="1aa90-344">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="1aa90-345">Волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="1aa90-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="1aa90-346">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-346">Boolean</span></span>|<span data-ttu-id="1aa90-347">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="1aa90-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="1aa90-348">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="1aa90-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="1aa90-349">String</span><span class="sxs-lookup"><span data-stu-id="1aa90-349">String</span></span>|<span data-ttu-id="1aa90-350">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="1aa90-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="1aa90-351">Впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="1aa90-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="1aa90-352">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-352">Boolean</span></span>|<span data-ttu-id="1aa90-353">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="1aa90-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="1aa90-354">Вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1aa90-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="1aa90-355">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-355">Boolean</span></span>|<span data-ttu-id="1aa90-356">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="1aa90-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="1aa90-357">Вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1aa90-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="1aa90-358">Логический</span><span class="sxs-lookup"><span data-stu-id="1aa90-358">Boolean</span></span>|<span data-ttu-id="1aa90-359">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="1aa90-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1aa90-360">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aa90-360">Response</span></span>
<span data-ttu-id="1aa90-361">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1aa90-361">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aa90-362">Пример</span><span class="sxs-lookup"><span data-stu-id="1aa90-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aa90-363">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aa90-363">Request</span></span>
<span data-ttu-id="1aa90-364">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1aa90-364">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1aa90-365">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aa90-365">Response</span></span>
<span data-ttu-id="1aa90-p130">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1aa90-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





