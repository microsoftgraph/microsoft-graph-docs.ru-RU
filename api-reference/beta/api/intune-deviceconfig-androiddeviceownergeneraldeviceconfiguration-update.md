---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1991fbfcef9ce55b12536c0b78c4f1d58937c033
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571559"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="49b8a-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="49b8a-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="49b8a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49b8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49b8a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49b8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49b8a-106">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="49b8a-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49b8a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49b8a-107">Prerequisites</span></span>
<span data-ttu-id="49b8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49b8a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49b8a-110">Permission type</span></span>|<span data-ttu-id="49b8a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49b8a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49b8a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49b8a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49b8a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49b8a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49b8a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49b8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49b8a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49b8a-115">Not supported.</span></span>|
|<span data-ttu-id="49b8a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49b8a-116">Application</span></span>|<span data-ttu-id="49b8a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49b8a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49b8a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49b8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="49b8a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49b8a-119">Request headers</span></span>
|<span data-ttu-id="49b8a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49b8a-120">Header</span></span>|<span data-ttu-id="49b8a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="49b8a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49b8a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49b8a-122">Authorization</span></span>|<span data-ttu-id="49b8a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49b8a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49b8a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="49b8a-124">Accept</span></span>|<span data-ttu-id="49b8a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49b8a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49b8a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49b8a-126">Request body</span></span>
<span data-ttu-id="49b8a-127">В тексте запроса добавьте представление объекта [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49b8a-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="49b8a-128">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="49b8a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="49b8a-129">Property</span></span>|<span data-ttu-id="49b8a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="49b8a-130">Type</span></span>|<span data-ttu-id="49b8a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="49b8a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49b8a-132">id</span><span class="sxs-lookup"><span data-stu-id="49b8a-132">id</span></span>|<span data-ttu-id="49b8a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="49b8a-133">String</span></span>|<span data-ttu-id="49b8a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49b8a-134">Key of the entity.</span></span> <span data-ttu-id="49b8a-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49b8a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="49b8a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49b8a-137">DateTimeOffset</span></span>|<span data-ttu-id="49b8a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="49b8a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="49b8a-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49b8a-140">roleScopeTagIds</span></span>|<span data-ttu-id="49b8a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="49b8a-141">String collection</span></span>|<span data-ttu-id="49b8a-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="49b8a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49b8a-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="49b8a-144">supportsScopeTags</span></span>|<span data-ttu-id="49b8a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-145">Boolean</span></span>|<span data-ttu-id="49b8a-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="49b8a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49b8a-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="49b8a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49b8a-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="49b8a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49b8a-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49b8a-149">This property is read-only.</span></span> <span data-ttu-id="49b8a-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49b8a-151">createdDateTime</span></span>|<span data-ttu-id="49b8a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49b8a-152">DateTimeOffset</span></span>|<span data-ttu-id="49b8a-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="49b8a-153">DateTime the object was created.</span></span> <span data-ttu-id="49b8a-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-155">description</span><span class="sxs-lookup"><span data-stu-id="49b8a-155">description</span></span>|<span data-ttu-id="49b8a-156">String</span><span class="sxs-lookup"><span data-stu-id="49b8a-156">String</span></span>|<span data-ttu-id="49b8a-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49b8a-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="49b8a-159">displayName</span></span>|<span data-ttu-id="49b8a-160">String</span><span class="sxs-lookup"><span data-stu-id="49b8a-160">String</span></span>|<span data-ttu-id="49b8a-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49b8a-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-163">version</span><span class="sxs-lookup"><span data-stu-id="49b8a-163">version</span></span>|<span data-ttu-id="49b8a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-164">Int32</span></span>|<span data-ttu-id="49b8a-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-165">Version of the device configuration.</span></span> <span data-ttu-id="49b8a-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49b8a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49b8a-167">Аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="49b8a-167">accountsBlockModification</span></span>|<span data-ttu-id="49b8a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-168">Boolean</span></span>|<span data-ttu-id="49b8a-169">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="49b8a-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="49b8a-170">Аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="49b8a-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="49b8a-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-171">Boolean</span></span>|<span data-ttu-id="49b8a-172">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="49b8a-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="49b8a-173">Аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="49b8a-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="49b8a-174">Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="49b8a-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="49b8a-175">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="49b8a-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="49b8a-176">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="49b8a-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="49b8a-177">Аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="49b8a-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="49b8a-178">Андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="49b8a-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="49b8a-179">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="49b8a-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="49b8a-180">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="49b8a-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="49b8a-181">Аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="49b8a-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="49b8a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-182">Boolean</span></span>|<span data-ttu-id="49b8a-183">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="49b8a-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="49b8a-184">Блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="49b8a-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="49b8a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-185">Boolean</span></span>|<span data-ttu-id="49b8a-186">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="49b8a-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="49b8a-187">Блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="49b8a-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="49b8a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-188">Boolean</span></span>|<span data-ttu-id="49b8a-189">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="49b8a-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="49b8a-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="49b8a-190">cameraBlocked</span></span>|<span data-ttu-id="49b8a-191">Логический</span><span class="sxs-lookup"><span data-stu-id="49b8a-191">Boolean</span></span>|<span data-ttu-id="49b8a-192">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="49b8a-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="49b8a-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="49b8a-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="49b8a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-194">Boolean</span></span>|<span data-ttu-id="49b8a-195">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="49b8a-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="49b8a-196">Датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="49b8a-196">dataRoamingBlocked</span></span>|<span data-ttu-id="49b8a-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-197">Boolean</span></span>|<span data-ttu-id="49b8a-198">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="49b8a-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="49b8a-199">Датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="49b8a-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="49b8a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-200">Boolean</span></span>|<span data-ttu-id="49b8a-201">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="49b8a-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="49b8a-202">Факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="49b8a-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="49b8a-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="49b8a-203">String collection</span></span>|<span data-ttu-id="49b8a-204">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="49b8a-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="49b8a-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="49b8a-205">factoryResetBlocked</span></span>|<span data-ttu-id="49b8a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-206">Boolean</span></span>|<span data-ttu-id="49b8a-207">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="49b8a-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="49b8a-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="49b8a-208">kioskModeApps</span></span>|<span data-ttu-id="49b8a-209">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="49b8a-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="49b8a-210">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="49b8a-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="49b8a-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="49b8a-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="49b8a-212">Киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="49b8a-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="49b8a-213">Строка</span><span class="sxs-lookup"><span data-stu-id="49b8a-213">String</span></span>|<span data-ttu-id="49b8a-214">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="49b8a-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="49b8a-215">Киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="49b8a-215">kioskModeExitCode</span></span>|<span data-ttu-id="49b8a-216">Строка</span><span class="sxs-lookup"><span data-stu-id="49b8a-216">String</span></span>|<span data-ttu-id="49b8a-217">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="49b8a-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="49b8a-218">Киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="49b8a-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="49b8a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-219">Boolean</span></span>|<span data-ttu-id="49b8a-220">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="49b8a-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="49b8a-221">Микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="49b8a-221">microphoneForceMute</span></span>|<span data-ttu-id="49b8a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-222">Boolean</span></span>|<span data-ttu-id="49b8a-223">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-223">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="49b8a-224">Нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="49b8a-224">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="49b8a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-225">Boolean</span></span>|<span data-ttu-id="49b8a-226">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="49b8a-226">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="49b8a-227">Нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="49b8a-227">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="49b8a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-228">Boolean</span></span>|<span data-ttu-id="49b8a-229">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="49b8a-229">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="49b8a-230">Пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="49b8a-230">passwordBlockKeyguard</span></span>|<span data-ttu-id="49b8a-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-231">Boolean</span></span>|<span data-ttu-id="49b8a-232">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="49b8a-232">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="49b8a-233">Пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="49b8a-233">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="49b8a-234">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="49b8a-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="49b8a-235">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="49b8a-235">List of device keyguard features to block.</span></span> <span data-ttu-id="49b8a-236">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="49b8a-236">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="49b8a-237">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="49b8a-237">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="49b8a-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="49b8a-238">passwordExpirationDays</span></span>|<span data-ttu-id="49b8a-239">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-239">Int32</span></span>|<span data-ttu-id="49b8a-240">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="49b8a-240">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="49b8a-241">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="49b8a-241">Valid values 1 to 365</span></span>|
|<span data-ttu-id="49b8a-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="49b8a-242">passwordMinimumLength</span></span>|<span data-ttu-id="49b8a-243">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-243">Int32</span></span>|<span data-ttu-id="49b8a-244">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-244">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="49b8a-245">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="49b8a-245">Valid values 4 to 16</span></span>|
|<span data-ttu-id="49b8a-246">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="49b8a-246">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="49b8a-247">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-247">Int32</span></span>|<span data-ttu-id="49b8a-248">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="49b8a-248">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="49b8a-249">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="49b8a-249">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="49b8a-250">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-250">Int32</span></span>|<span data-ttu-id="49b8a-251">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="49b8a-251">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="49b8a-252">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="49b8a-252">Valid values 0 to 24</span></span>|
|<span data-ttu-id="49b8a-253">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="49b8a-253">passwordRequiredType</span></span>|[<span data-ttu-id="49b8a-254">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="49b8a-254">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="49b8a-255">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-255">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="49b8a-256">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="49b8a-256">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="49b8a-257">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="49b8a-257">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="49b8a-258">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-258">Int32</span></span>|<span data-ttu-id="49b8a-259">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-259">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="49b8a-260">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="49b8a-260">Valid values 4 to 11</span></span>|
|<span data-ttu-id="49b8a-261">Сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="49b8a-261">safeBootBlocked</span></span>|<span data-ttu-id="49b8a-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-262">Boolean</span></span>|<span data-ttu-id="49b8a-263">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="49b8a-263">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="49b8a-264">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="49b8a-264">screenCaptureBlocked</span></span>|<span data-ttu-id="49b8a-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-265">Boolean</span></span>|<span data-ttu-id="49b8a-266">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="49b8a-266">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="49b8a-267">Секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="49b8a-267">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="49b8a-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-268">Boolean</span></span>|<span data-ttu-id="49b8a-269">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="49b8a-269">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="49b8a-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="49b8a-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="49b8a-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-271">Boolean</span></span>|<span data-ttu-id="49b8a-272">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="49b8a-272">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="49b8a-273">Статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="49b8a-273">statusBarBlocked</span></span>|<span data-ttu-id="49b8a-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-274">Boolean</span></span>|<span data-ttu-id="49b8a-275">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="49b8a-275">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="49b8a-276">Стайонмодес</span><span class="sxs-lookup"><span data-stu-id="49b8a-276">stayOnModes</span></span>|<span data-ttu-id="49b8a-277">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="49b8a-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="49b8a-278">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="49b8a-278">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="49b8a-279">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="49b8a-279">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="49b8a-280">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="49b8a-280">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="49b8a-281">Сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="49b8a-281">storageAllowUsb</span></span>|<span data-ttu-id="49b8a-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-282">Boolean</span></span>|<span data-ttu-id="49b8a-283">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="49b8a-283">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="49b8a-284">Сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="49b8a-284">storageBlockExternalMedia</span></span>|<span data-ttu-id="49b8a-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-285">Boolean</span></span>|<span data-ttu-id="49b8a-286">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="49b8a-286">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="49b8a-287">Сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="49b8a-287">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="49b8a-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-288">Boolean</span></span>|<span data-ttu-id="49b8a-289">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="49b8a-289">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="49b8a-290">Системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="49b8a-290">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="49b8a-291">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-291">Int32</span></span>|<span data-ttu-id="49b8a-292">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="49b8a-292">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="49b8a-293">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="49b8a-293">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="49b8a-294">Системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="49b8a-294">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="49b8a-295">Int32</span><span class="sxs-lookup"><span data-stu-id="49b8a-295">Int32</span></span>|<span data-ttu-id="49b8a-296">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="49b8a-296">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="49b8a-297">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="49b8a-297">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="49b8a-298">Системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="49b8a-298">systemUpdateInstallType</span></span>|[<span data-ttu-id="49b8a-299">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="49b8a-299">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="49b8a-300">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="49b8a-300">The type of system update configuration.</span></span> <span data-ttu-id="49b8a-301">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="49b8a-301">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="49b8a-302">Системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="49b8a-302">systemWindowsBlocked</span></span>|<span data-ttu-id="49b8a-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-303">Boolean</span></span>|<span data-ttu-id="49b8a-304">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="49b8a-304">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="49b8a-305">Усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="49b8a-305">usersBlockAdd</span></span>|<span data-ttu-id="49b8a-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-306">Boolean</span></span>|<span data-ttu-id="49b8a-307">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="49b8a-307">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="49b8a-308">Усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="49b8a-308">usersBlockRemove</span></span>|<span data-ttu-id="49b8a-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-309">Boolean</span></span>|<span data-ttu-id="49b8a-310">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-310">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="49b8a-311">Волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="49b8a-311">volumeBlockAdjustment</span></span>|<span data-ttu-id="49b8a-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-312">Boolean</span></span>|<span data-ttu-id="49b8a-313">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="49b8a-313">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="49b8a-314">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="49b8a-314">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="49b8a-315">Строка</span><span class="sxs-lookup"><span data-stu-id="49b8a-315">String</span></span>|<span data-ttu-id="49b8a-316">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="49b8a-316">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="49b8a-317">Впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="49b8a-317">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="49b8a-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-318">Boolean</span></span>|<span data-ttu-id="49b8a-319">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="49b8a-319">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="49b8a-320">Вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="49b8a-320">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="49b8a-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-321">Boolean</span></span>|<span data-ttu-id="49b8a-322">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="49b8a-322">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="49b8a-323">Вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="49b8a-323">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="49b8a-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="49b8a-324">Boolean</span></span>|<span data-ttu-id="49b8a-325">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="49b8a-325">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="49b8a-326">Ответ</span><span class="sxs-lookup"><span data-stu-id="49b8a-326">Response</span></span>
<span data-ttu-id="49b8a-327">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49b8a-327">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49b8a-328">Пример</span><span class="sxs-lookup"><span data-stu-id="49b8a-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="49b8a-329">Запрос</span><span class="sxs-lookup"><span data-stu-id="49b8a-329">Request</span></span>
<span data-ttu-id="49b8a-330">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49b8a-330">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2517

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="49b8a-331">Отклик</span><span class="sxs-lookup"><span data-stu-id="49b8a-331">Response</span></span>
<span data-ttu-id="49b8a-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49b8a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2689

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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




