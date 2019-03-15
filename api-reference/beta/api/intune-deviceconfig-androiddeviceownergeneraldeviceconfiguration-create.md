---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd38922bd7daa8f3e805208fe7c70d6d4abe777
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571944"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="abdc4-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="abdc4-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="abdc4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abdc4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abdc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abdc4-106">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="abdc4-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abdc4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="abdc4-107">Prerequisites</span></span>
<span data-ttu-id="abdc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="abdc4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abdc4-110">Permission type</span></span>|<span data-ttu-id="abdc4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abdc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abdc4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abdc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abdc4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abdc4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abdc4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abdc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abdc4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdc4-115">Not supported.</span></span>|
|<span data-ttu-id="abdc4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abdc4-116">Application</span></span>|<span data-ttu-id="abdc4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdc4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abdc4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abdc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="abdc4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abdc4-119">Request headers</span></span>
|<span data-ttu-id="abdc4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abdc4-120">Header</span></span>|<span data-ttu-id="abdc4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="abdc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abdc4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abdc4-122">Authorization</span></span>|<span data-ttu-id="abdc4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abdc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abdc4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="abdc4-124">Accept</span></span>|<span data-ttu-id="abdc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abdc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abdc4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abdc4-126">Request body</span></span>
<span data-ttu-id="abdc4-127">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abdc4-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="abdc4-128">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="abdc4-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="abdc4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="abdc4-129">Property</span></span>|<span data-ttu-id="abdc4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="abdc4-130">Type</span></span>|<span data-ttu-id="abdc4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="abdc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abdc4-132">id</span><span class="sxs-lookup"><span data-stu-id="abdc4-132">id</span></span>|<span data-ttu-id="abdc4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="abdc4-133">String</span></span>|<span data-ttu-id="abdc4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="abdc4-134">Key of the entity.</span></span> <span data-ttu-id="abdc4-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abdc4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="abdc4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abdc4-137">DateTimeOffset</span></span>|<span data-ttu-id="abdc4-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="abdc4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="abdc4-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="abdc4-140">roleScopeTagIds</span></span>|<span data-ttu-id="abdc4-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="abdc4-141">String collection</span></span>|<span data-ttu-id="abdc4-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="abdc4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="abdc4-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="abdc4-144">supportsScopeTags</span></span>|<span data-ttu-id="abdc4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-145">Boolean</span></span>|<span data-ttu-id="abdc4-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="abdc4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="abdc4-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="abdc4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="abdc4-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="abdc4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="abdc4-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="abdc4-149">This property is read-only.</span></span> <span data-ttu-id="abdc4-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abdc4-151">createdDateTime</span></span>|<span data-ttu-id="abdc4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abdc4-152">DateTimeOffset</span></span>|<span data-ttu-id="abdc4-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="abdc4-153">DateTime the object was created.</span></span> <span data-ttu-id="abdc4-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-155">description</span><span class="sxs-lookup"><span data-stu-id="abdc4-155">description</span></span>|<span data-ttu-id="abdc4-156">String</span><span class="sxs-lookup"><span data-stu-id="abdc4-156">String</span></span>|<span data-ttu-id="abdc4-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="abdc4-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="abdc4-159">displayName</span></span>|<span data-ttu-id="abdc4-160">String</span><span class="sxs-lookup"><span data-stu-id="abdc4-160">String</span></span>|<span data-ttu-id="abdc4-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="abdc4-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-163">version</span><span class="sxs-lookup"><span data-stu-id="abdc4-163">version</span></span>|<span data-ttu-id="abdc4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-164">Int32</span></span>|<span data-ttu-id="abdc4-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-165">Version of the device configuration.</span></span> <span data-ttu-id="abdc4-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abdc4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abdc4-167">Аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="abdc4-167">accountsBlockModification</span></span>|<span data-ttu-id="abdc4-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-168">Boolean</span></span>|<span data-ttu-id="abdc4-169">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="abdc4-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="abdc4-170">Аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="abdc4-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="abdc4-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-171">Boolean</span></span>|<span data-ttu-id="abdc4-172">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="abdc4-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="abdc4-173">Аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="abdc4-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="abdc4-174">Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="abdc4-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="abdc4-175">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="abdc4-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="abdc4-176">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="abdc4-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="abdc4-177">Аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="abdc4-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="abdc4-178">Андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="abdc4-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="abdc4-179">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="abdc4-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="abdc4-180">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="abdc4-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="abdc4-181">Аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="abdc4-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="abdc4-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-182">Boolean</span></span>|<span data-ttu-id="abdc4-183">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="abdc4-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="abdc4-184">Блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="abdc4-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="abdc4-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-185">Boolean</span></span>|<span data-ttu-id="abdc4-186">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="abdc4-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="abdc4-187">Блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="abdc4-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="abdc4-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-188">Boolean</span></span>|<span data-ttu-id="abdc4-189">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="abdc4-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="abdc4-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="abdc4-190">cameraBlocked</span></span>|<span data-ttu-id="abdc4-191">Логический</span><span class="sxs-lookup"><span data-stu-id="abdc4-191">Boolean</span></span>|<span data-ttu-id="abdc4-192">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="abdc4-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="abdc4-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="abdc4-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="abdc4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-194">Boolean</span></span>|<span data-ttu-id="abdc4-195">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="abdc4-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="abdc4-196">Датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="abdc4-196">dataRoamingBlocked</span></span>|<span data-ttu-id="abdc4-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-197">Boolean</span></span>|<span data-ttu-id="abdc4-198">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="abdc4-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="abdc4-199">Датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="abdc4-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="abdc4-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-200">Boolean</span></span>|<span data-ttu-id="abdc4-201">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="abdc4-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="abdc4-202">Факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="abdc4-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="abdc4-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="abdc4-203">String collection</span></span>|<span data-ttu-id="abdc4-204">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="abdc4-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="abdc4-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="abdc4-205">factoryResetBlocked</span></span>|<span data-ttu-id="abdc4-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-206">Boolean</span></span>|<span data-ttu-id="abdc4-207">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="abdc4-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="abdc4-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="abdc4-208">kioskModeApps</span></span>|<span data-ttu-id="abdc4-209">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="abdc4-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="abdc4-210">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="abdc4-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="abdc4-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="abdc4-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="abdc4-212">Киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="abdc4-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="abdc4-213">Строка</span><span class="sxs-lookup"><span data-stu-id="abdc4-213">String</span></span>|<span data-ttu-id="abdc4-214">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="abdc4-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="abdc4-215">Киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="abdc4-215">kioskModeExitCode</span></span>|<span data-ttu-id="abdc4-216">Строка</span><span class="sxs-lookup"><span data-stu-id="abdc4-216">String</span></span>|<span data-ttu-id="abdc4-217">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="abdc4-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="abdc4-218">Киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="abdc4-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="abdc4-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-219">Boolean</span></span>|<span data-ttu-id="abdc4-220">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="abdc4-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="abdc4-221">Микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="abdc4-221">microphoneForceMute</span></span>|<span data-ttu-id="abdc4-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-222">Boolean</span></span>|<span data-ttu-id="abdc4-223">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-223">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="abdc4-224">Нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="abdc4-224">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="abdc4-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-225">Boolean</span></span>|<span data-ttu-id="abdc4-226">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="abdc4-226">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="abdc4-227">Нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="abdc4-227">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="abdc4-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-228">Boolean</span></span>|<span data-ttu-id="abdc4-229">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="abdc4-229">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="abdc4-230">Пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="abdc4-230">passwordBlockKeyguard</span></span>|<span data-ttu-id="abdc4-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-231">Boolean</span></span>|<span data-ttu-id="abdc4-232">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="abdc4-232">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="abdc4-233">Пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="abdc4-233">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="abdc4-234">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="abdc4-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="abdc4-235">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="abdc4-235">List of device keyguard features to block.</span></span> <span data-ttu-id="abdc4-236">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="abdc4-236">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="abdc4-237">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="abdc4-237">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="abdc4-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="abdc4-238">passwordExpirationDays</span></span>|<span data-ttu-id="abdc4-239">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-239">Int32</span></span>|<span data-ttu-id="abdc4-240">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="abdc4-240">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="abdc4-241">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="abdc4-241">Valid values 1 to 365</span></span>|
|<span data-ttu-id="abdc4-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="abdc4-242">passwordMinimumLength</span></span>|<span data-ttu-id="abdc4-243">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-243">Int32</span></span>|<span data-ttu-id="abdc4-244">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-244">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="abdc4-245">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="abdc4-245">Valid values 4 to 16</span></span>|
|<span data-ttu-id="abdc4-246">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="abdc4-246">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="abdc4-247">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-247">Int32</span></span>|<span data-ttu-id="abdc4-248">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="abdc4-248">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="abdc4-249">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="abdc4-249">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="abdc4-250">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-250">Int32</span></span>|<span data-ttu-id="abdc4-251">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="abdc4-251">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="abdc4-252">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="abdc4-252">Valid values 0 to 24</span></span>|
|<span data-ttu-id="abdc4-253">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="abdc4-253">passwordRequiredType</span></span>|[<span data-ttu-id="abdc4-254">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="abdc4-254">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="abdc4-255">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-255">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="abdc4-256">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="abdc4-256">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="abdc4-257">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="abdc4-257">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="abdc4-258">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-258">Int32</span></span>|<span data-ttu-id="abdc4-259">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-259">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="abdc4-260">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="abdc4-260">Valid values 4 to 11</span></span>|
|<span data-ttu-id="abdc4-261">Сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="abdc4-261">safeBootBlocked</span></span>|<span data-ttu-id="abdc4-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-262">Boolean</span></span>|<span data-ttu-id="abdc4-263">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="abdc4-263">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="abdc4-264">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="abdc4-264">screenCaptureBlocked</span></span>|<span data-ttu-id="abdc4-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-265">Boolean</span></span>|<span data-ttu-id="abdc4-266">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="abdc4-266">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="abdc4-267">Секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="abdc4-267">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="abdc4-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-268">Boolean</span></span>|<span data-ttu-id="abdc4-269">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="abdc4-269">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="abdc4-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="abdc4-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="abdc4-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-271">Boolean</span></span>|<span data-ttu-id="abdc4-272">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="abdc4-272">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="abdc4-273">Статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="abdc4-273">statusBarBlocked</span></span>|<span data-ttu-id="abdc4-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-274">Boolean</span></span>|<span data-ttu-id="abdc4-275">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="abdc4-275">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="abdc4-276">Стайонмодес</span><span class="sxs-lookup"><span data-stu-id="abdc4-276">stayOnModes</span></span>|<span data-ttu-id="abdc4-277">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="abdc4-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="abdc4-278">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="abdc4-278">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="abdc4-279">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="abdc4-279">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="abdc4-280">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="abdc4-280">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="abdc4-281">Сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="abdc4-281">storageAllowUsb</span></span>|<span data-ttu-id="abdc4-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-282">Boolean</span></span>|<span data-ttu-id="abdc4-283">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="abdc4-283">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="abdc4-284">Сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="abdc4-284">storageBlockExternalMedia</span></span>|<span data-ttu-id="abdc4-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-285">Boolean</span></span>|<span data-ttu-id="abdc4-286">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="abdc4-286">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="abdc4-287">Сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="abdc4-287">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="abdc4-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-288">Boolean</span></span>|<span data-ttu-id="abdc4-289">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="abdc4-289">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="abdc4-290">Системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="abdc4-290">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="abdc4-291">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-291">Int32</span></span>|<span data-ttu-id="abdc4-292">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="abdc4-292">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="abdc4-293">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="abdc4-293">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="abdc4-294">Системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="abdc4-294">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="abdc4-295">Int32</span><span class="sxs-lookup"><span data-stu-id="abdc4-295">Int32</span></span>|<span data-ttu-id="abdc4-296">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="abdc4-296">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="abdc4-297">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="abdc4-297">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="abdc4-298">Системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="abdc4-298">systemUpdateInstallType</span></span>|[<span data-ttu-id="abdc4-299">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="abdc4-299">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="abdc4-300">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="abdc4-300">The type of system update configuration.</span></span> <span data-ttu-id="abdc4-301">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="abdc4-301">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="abdc4-302">Системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="abdc4-302">systemWindowsBlocked</span></span>|<span data-ttu-id="abdc4-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-303">Boolean</span></span>|<span data-ttu-id="abdc4-304">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="abdc4-304">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="abdc4-305">Усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="abdc4-305">usersBlockAdd</span></span>|<span data-ttu-id="abdc4-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-306">Boolean</span></span>|<span data-ttu-id="abdc4-307">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="abdc4-307">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="abdc4-308">Усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="abdc4-308">usersBlockRemove</span></span>|<span data-ttu-id="abdc4-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-309">Boolean</span></span>|<span data-ttu-id="abdc4-310">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-310">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="abdc4-311">Волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="abdc4-311">volumeBlockAdjustment</span></span>|<span data-ttu-id="abdc4-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-312">Boolean</span></span>|<span data-ttu-id="abdc4-313">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="abdc4-313">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="abdc4-314">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="abdc4-314">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="abdc4-315">Строка</span><span class="sxs-lookup"><span data-stu-id="abdc4-315">String</span></span>|<span data-ttu-id="abdc4-316">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="abdc4-316">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="abdc4-317">Впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="abdc4-317">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="abdc4-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-318">Boolean</span></span>|<span data-ttu-id="abdc4-319">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="abdc4-319">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="abdc4-320">Вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="abdc4-320">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="abdc4-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-321">Boolean</span></span>|<span data-ttu-id="abdc4-322">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="abdc4-322">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="abdc4-323">Вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="abdc4-323">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="abdc4-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="abdc4-324">Boolean</span></span>|<span data-ttu-id="abdc4-325">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="abdc4-325">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="abdc4-326">Ответ</span><span class="sxs-lookup"><span data-stu-id="abdc4-326">Response</span></span>
<span data-ttu-id="abdc4-327">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abdc4-327">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abdc4-328">Пример</span><span class="sxs-lookup"><span data-stu-id="abdc4-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="abdc4-329">Запрос</span><span class="sxs-lookup"><span data-stu-id="abdc4-329">Request</span></span>
<span data-ttu-id="abdc4-330">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abdc4-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="abdc4-331">Отклик</span><span class="sxs-lookup"><span data-stu-id="abdc4-331">Response</span></span>
<span data-ttu-id="abdc4-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abdc4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




