---
title: Создание aospDeviceOwnerDeviceConfiguration
description: Создайте новый объект aospDeviceOwnerDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efe34a28e77181ff941570db1606a95351c0ec0c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151776"
---
# <a name="create-aospdeviceownerdeviceconfiguration"></a><span data-ttu-id="9372b-103">Создание aospDeviceOwnerDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9372b-103">Create aospDeviceOwnerDeviceConfiguration</span></span>

<span data-ttu-id="9372b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9372b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9372b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9372b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9372b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9372b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9372b-107">Создайте новый [объект aospDeviceOwnerDeviceConfiguration.](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9372b-107">Create a new [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9372b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9372b-108">Prerequisites</span></span>
<span data-ttu-id="9372b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9372b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9372b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9372b-111">Permission type</span></span>|<span data-ttu-id="9372b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9372b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9372b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9372b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9372b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9372b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9372b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9372b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9372b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9372b-116">Not supported.</span></span>|
|<span data-ttu-id="9372b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9372b-117">Application</span></span>|<span data-ttu-id="9372b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9372b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9372b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9372b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9372b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9372b-120">Request headers</span></span>
|<span data-ttu-id="9372b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9372b-121">Header</span></span>|<span data-ttu-id="9372b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9372b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9372b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9372b-123">Authorization</span></span>|<span data-ttu-id="9372b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9372b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9372b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9372b-125">Accept</span></span>|<span data-ttu-id="9372b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9372b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9372b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9372b-127">Request body</span></span>
<span data-ttu-id="9372b-128">В теле запроса поставляем представление JSON для объекта aospDeviceOwnerDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9372b-128">In the request body, supply a JSON representation for the aospDeviceOwnerDeviceConfiguration object.</span></span>

<span data-ttu-id="9372b-129">В следующей таблице показаны свойства, необходимые при создании aospDeviceOwnerDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9372b-129">The following table shows the properties that are required when you create the aospDeviceOwnerDeviceConfiguration.</span></span>

|<span data-ttu-id="9372b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9372b-130">Property</span></span>|<span data-ttu-id="9372b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9372b-131">Type</span></span>|<span data-ttu-id="9372b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9372b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9372b-133">id</span><span class="sxs-lookup"><span data-stu-id="9372b-133">id</span></span>|<span data-ttu-id="9372b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9372b-134">String</span></span>|<span data-ttu-id="9372b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9372b-135">Key of the entity.</span></span> <span data-ttu-id="9372b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9372b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9372b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9372b-138">DateTimeOffset</span></span>|<span data-ttu-id="9372b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9372b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9372b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9372b-141">roleScopeTagIds</span></span>|<span data-ttu-id="9372b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9372b-142">String collection</span></span>|<span data-ttu-id="9372b-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="9372b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9372b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9372b-145">supportsScopeTags</span></span>|<span data-ttu-id="9372b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-146">Boolean</span></span>|<span data-ttu-id="9372b-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9372b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9372b-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="9372b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9372b-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9372b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9372b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9372b-150">This property is read-only.</span></span> <span data-ttu-id="9372b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9372b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9372b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9372b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9372b-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9372b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9372b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9372b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9372b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9372b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9372b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9372b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9372b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9372b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9372b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9372b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9372b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9372b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9372b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9372b-164">createdDateTime</span></span>|<span data-ttu-id="9372b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9372b-165">DateTimeOffset</span></span>|<span data-ttu-id="9372b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9372b-166">DateTime the object was created.</span></span> <span data-ttu-id="9372b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-168">description</span><span class="sxs-lookup"><span data-stu-id="9372b-168">description</span></span>|<span data-ttu-id="9372b-169">Строка</span><span class="sxs-lookup"><span data-stu-id="9372b-169">String</span></span>|<span data-ttu-id="9372b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9372b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9372b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9372b-172">displayName</span></span>|<span data-ttu-id="9372b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="9372b-173">String</span></span>|<span data-ttu-id="9372b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9372b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9372b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-176">version</span><span class="sxs-lookup"><span data-stu-id="9372b-176">version</span></span>|<span data-ttu-id="9372b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9372b-177">Int32</span></span>|<span data-ttu-id="9372b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9372b-178">Version of the device configuration.</span></span> <span data-ttu-id="9372b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9372b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9372b-180">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="9372b-180">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="9372b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-181">Boolean</span></span>|<span data-ttu-id="9372b-182">Указывает, разрешено ли пользователю включить параметр неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="9372b-182">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="9372b-183">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="9372b-183">bluetoothBlocked</span></span>|<span data-ttu-id="9372b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-184">Boolean</span></span>|<span data-ttu-id="9372b-185">Указывает, следует ли отключить использование Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9372b-185">Indicates whether or not to disable the use of bluetooth.</span></span> <span data-ttu-id="9372b-186">При наборе true bluetooth нельзя включить на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9372b-186">When set to true, bluetooth cannot be enabled on the device.</span></span>|
|<span data-ttu-id="9372b-187">BluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="9372b-187">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="9372b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-188">Boolean</span></span>|<span data-ttu-id="9372b-189">Указывает, следует ли блокировать пользователю настройку Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9372b-189">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="9372b-190">BluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="9372b-190">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="9372b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-191">Boolean</span></span>|<span data-ttu-id="9372b-192">Указывает, следует ли блокировать пользователю доступ к контактам по Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9372b-192">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="9372b-193">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9372b-193">cameraBlocked</span></span>|<span data-ttu-id="9372b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-194">Boolean</span></span>|<span data-ttu-id="9372b-195">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="9372b-195">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="9372b-196">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="9372b-196">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="9372b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-197">Boolean</span></span>|<span data-ttu-id="9372b-198">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9372b-198">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="9372b-199">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="9372b-199">factoryResetBlocked</span></span>|<span data-ttu-id="9372b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-200">Boolean</span></span>|<span data-ttu-id="9372b-201">Указывает, отключен ли параметр сброса фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="9372b-201">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="9372b-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9372b-202">passwordMinimumLength</span></span>|<span data-ttu-id="9372b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9372b-203">Int32</span></span>|<span data-ttu-id="9372b-204">Указывает минимальную длину пароля, необходимого на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9372b-204">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="9372b-205">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="9372b-205">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9372b-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9372b-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9372b-207">Int32</span><span class="sxs-lookup"><span data-stu-id="9372b-207">Int32</span></span>|<span data-ttu-id="9372b-208">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="9372b-208">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9372b-209">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9372b-209">passwordRequiredType</span></span>|[<span data-ttu-id="9372b-210">AndroidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9372b-210">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="9372b-211">Указывает минимальное качество пароля, необходимое на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9372b-211">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="9372b-212">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="9372b-212">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="9372b-213">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9372b-213">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9372b-214">Int32</span><span class="sxs-lookup"><span data-stu-id="9372b-214">Int32</span></span>|<span data-ttu-id="9372b-215">Указывает количество случаев, когда пользователь может ввести неправильный пароль до стирки устройства.</span><span class="sxs-lookup"><span data-stu-id="9372b-215">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="9372b-216">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="9372b-216">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9372b-217">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9372b-217">screenCaptureBlocked</span></span>|<span data-ttu-id="9372b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-218">Boolean</span></span>|<span data-ttu-id="9372b-219">Указывает, следует ли отключить возможность делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="9372b-219">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="9372b-220">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="9372b-220">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="9372b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-221">Boolean</span></span>|<span data-ttu-id="9372b-222">Указывает, следует ли блокировать пользователю включение функций отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9372b-222">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="9372b-223">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="9372b-223">storageAllowUsb</span></span>|<span data-ttu-id="9372b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-224">Boolean</span></span>|<span data-ttu-id="9372b-225">Указывает, следует ли блокировать USB-хранилище.</span><span class="sxs-lookup"><span data-stu-id="9372b-225">Indicates whether or not to block USB storage.</span></span>|
|<span data-ttu-id="9372b-226">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="9372b-226">storageBlockExternalMedia</span></span>|<span data-ttu-id="9372b-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-227">Boolean</span></span>|<span data-ttu-id="9372b-228">Указывает, следует ли блокировать внешние носитли.</span><span class="sxs-lookup"><span data-stu-id="9372b-228">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="9372b-229">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="9372b-229">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="9372b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-230">Boolean</span></span>|<span data-ttu-id="9372b-231">Указывает, следует ли блокировать передачу usb-файлов.</span><span class="sxs-lookup"><span data-stu-id="9372b-231">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="9372b-232">backupBlocked</span><span class="sxs-lookup"><span data-stu-id="9372b-232">backupBlocked</span></span>|<span data-ttu-id="9372b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-233">Boolean</span></span>|<span data-ttu-id="9372b-234">Указывает, следует ли блокировать службу резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="9372b-234">Indicates whether or not to block backup service.</span></span>|
|<span data-ttu-id="9372b-235">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="9372b-235">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="9372b-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="9372b-236">Boolean</span></span>|<span data-ttu-id="9372b-237">Указывает, следует ли блокировать пользователю редактирование параметров подключения к Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9372b-237">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|



## <a name="response"></a><span data-ttu-id="9372b-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="9372b-238">Response</span></span>
<span data-ttu-id="9372b-239">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9372b-239">If successful, this method returns a `201 Created` response code and a [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9372b-240">Пример</span><span class="sxs-lookup"><span data-stu-id="9372b-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="9372b-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="9372b-241">Request</span></span>
<span data-ttu-id="9372b-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9372b-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1721

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="9372b-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="9372b-243">Response</span></span>
<span data-ttu-id="9372b-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9372b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1893

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
  "id": "c9e83a69-3a69-c9e8-693a-e8c9693ae8c9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```




