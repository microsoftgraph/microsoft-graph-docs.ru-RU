---
title: Обновление windows10DeviceFirmwareConfigurationInterface
description: Обновление свойств объекта Windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfa3f6b91b55847771a610a5743c27ea7f7f7fbb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863768"
---
# <a name="update-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="51e2e-103">Обновление windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="51e2e-103">Update windows10DeviceFirmwareConfigurationInterface</span></span>

<span data-ttu-id="51e2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51e2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51e2e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51e2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51e2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e2e-107">Обновление свойств объекта [Windows10DeviceFirmwareConfigurationInterface.](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)</span><span class="sxs-lookup"><span data-stu-id="51e2e-107">Update the properties of a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51e2e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51e2e-108">Prerequisites</span></span>
<span data-ttu-id="51e2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51e2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51e2e-111">Permission type</span></span>|<span data-ttu-id="51e2e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51e2e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51e2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51e2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51e2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51e2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e2e-116">Not supported.</span></span>|
|<span data-ttu-id="51e2e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="51e2e-117">Application</span></span>|<span data-ttu-id="51e2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51e2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="51e2e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51e2e-120">Request headers</span></span>
|<span data-ttu-id="51e2e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51e2e-121">Header</span></span>|<span data-ttu-id="51e2e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51e2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51e2e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51e2e-123">Authorization</span></span>|<span data-ttu-id="51e2e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51e2e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51e2e-125">Accept</span></span>|<span data-ttu-id="51e2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51e2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51e2e-127">Request body</span></span>
<span data-ttu-id="51e2e-128">В корпусе запроса предоставляем представление JSON для [объекта Windows10DeviceFirmwareConfigurationInterface.](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)</span><span class="sxs-lookup"><span data-stu-id="51e2e-128">In the request body, supply a JSON representation for the [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

<span data-ttu-id="51e2e-129">В следующей таблице показаны свойства, необходимые при создании [windows10DeviceFirmwareConfigurationInterface.](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)</span><span class="sxs-lookup"><span data-stu-id="51e2e-129">The following table shows the properties that are required when you create the [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).</span></span>

|<span data-ttu-id="51e2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="51e2e-130">Property</span></span>|<span data-ttu-id="51e2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="51e2e-131">Type</span></span>|<span data-ttu-id="51e2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="51e2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e2e-133">id</span><span class="sxs-lookup"><span data-stu-id="51e2e-133">id</span></span>|<span data-ttu-id="51e2e-134">String</span><span class="sxs-lookup"><span data-stu-id="51e2e-134">String</span></span>|<span data-ttu-id="51e2e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51e2e-135">Key of the entity.</span></span> <span data-ttu-id="51e2e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51e2e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="51e2e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51e2e-138">DateTimeOffset</span></span>|<span data-ttu-id="51e2e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="51e2e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="51e2e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51e2e-141">roleScopeTagIds</span></span>|<span data-ttu-id="51e2e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="51e2e-142">String collection</span></span>|<span data-ttu-id="51e2e-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="51e2e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51e2e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51e2e-145">supportsScopeTags</span></span>|<span data-ttu-id="51e2e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="51e2e-146">Boolean</span></span>|<span data-ttu-id="51e2e-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="51e2e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51e2e-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="51e2e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51e2e-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="51e2e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51e2e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51e2e-150">This property is read-only.</span></span> <span data-ttu-id="51e2e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51e2e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="51e2e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51e2e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="51e2e-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51e2e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="51e2e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51e2e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="51e2e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51e2e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="51e2e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51e2e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="51e2e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51e2e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="51e2e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51e2e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="51e2e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51e2e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="51e2e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51e2e-164">createdDateTime</span></span>|<span data-ttu-id="51e2e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51e2e-165">DateTimeOffset</span></span>|<span data-ttu-id="51e2e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="51e2e-166">DateTime the object was created.</span></span> <span data-ttu-id="51e2e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-168">description</span><span class="sxs-lookup"><span data-stu-id="51e2e-168">description</span></span>|<span data-ttu-id="51e2e-169">String</span><span class="sxs-lookup"><span data-stu-id="51e2e-169">String</span></span>|<span data-ttu-id="51e2e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51e2e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51e2e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="51e2e-172">displayName</span></span>|<span data-ttu-id="51e2e-173">String</span><span class="sxs-lookup"><span data-stu-id="51e2e-173">String</span></span>|<span data-ttu-id="51e2e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51e2e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51e2e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-176">version</span><span class="sxs-lookup"><span data-stu-id="51e2e-176">version</span></span>|<span data-ttu-id="51e2e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="51e2e-177">Int32</span></span>|<span data-ttu-id="51e2e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51e2e-178">Version of the device configuration.</span></span> <span data-ttu-id="51e2e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e2e-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="51e2e-180">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="51e2e-181">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="51e2e-181">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="51e2e-182">Определяет уровень разрешений, предоставленный пользователям для изменения параметров UEFI.</span><span class="sxs-lookup"><span data-stu-id="51e2e-182">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="51e2e-183">Возможные значения: `notConfiguredOnly`, `none`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-183">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="51e2e-184">виртуализацияOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="51e2e-184">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="51e2e-185">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-185">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-186">Определяет, включена ли виртуализация ЦП и IO.</span><span class="sxs-lookup"><span data-stu-id="51e2e-186">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="51e2e-187">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-188">камеры</span><span class="sxs-lookup"><span data-stu-id="51e2e-188">cameras</span></span>|[<span data-ttu-id="51e2e-189">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-190">Определяет, включены ли встроенные камеры.</span><span class="sxs-lookup"><span data-stu-id="51e2e-190">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="51e2e-191">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-192">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="51e2e-192">microphonesAndSpeakers</span></span>|[<span data-ttu-id="51e2e-193">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-193">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-194">Определяет, включены ли встроенные микрофоны или динамики.</span><span class="sxs-lookup"><span data-stu-id="51e2e-194">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="51e2e-195">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-195">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-196">радио</span><span class="sxs-lookup"><span data-stu-id="51e2e-196">radios</span></span>|[<span data-ttu-id="51e2e-197">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-197">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-198">Определяет, включены ли встроенные радиостанции, например WIFI, NFC, Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="51e2e-198">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="51e2e-199">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-199">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-200">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="51e2e-200">bootFromExternalMedia</span></span>|[<span data-ttu-id="51e2e-201">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-201">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-202">Определяет, разрешено ли пользователю загрузиться из внешних мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="51e2e-202">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="51e2e-203">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-203">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-204">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="51e2e-204">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="51e2e-205">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-205">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-206">Определяет, разрешена ли пользователю загрузка из встроенных сетевых адаптеров.</span><span class="sxs-lookup"><span data-stu-id="51e2e-206">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="51e2e-207">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-207">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-208">WindowsPlatformBinaryTable</span><span class="sxs-lookup"><span data-stu-id="51e2e-208">windowsPlatformBinaryTable</span></span>|[<span data-ttu-id="51e2e-209">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-209">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-210">Определяет, разрешено ли пользователю включить двоичную таблицу Windows Platform.</span><span class="sxs-lookup"><span data-stu-id="51e2e-210">Defines whether a user is allowed to enable Windows Platform Binary Table.</span></span> <span data-ttu-id="51e2e-211">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-211">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="51e2e-212">simultaneousMultiThreading</span><span class="sxs-lookup"><span data-stu-id="51e2e-212">simultaneousMultiThreading</span></span>|[<span data-ttu-id="51e2e-213">включить</span><span class="sxs-lookup"><span data-stu-id="51e2e-213">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="51e2e-214">Определяет, разрешено ли пользователю включить одновременную многотекустойку.</span><span class="sxs-lookup"><span data-stu-id="51e2e-214">Defines whether a user is allowed to enable Simultaneous MultiThreading.</span></span> <span data-ttu-id="51e2e-215">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-215">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="51e2e-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e2e-216">Response</span></span>
<span data-ttu-id="51e2e-217">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект Windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51e2e-217">If successful, this method returns a `200 OK` response code and an updated [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e2e-218">Пример</span><span class="sxs-lookup"><span data-stu-id="51e2e-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="51e2e-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e2e-219">Request</span></span>
<span data-ttu-id="51e2e-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e2e-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1397

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="51e2e-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e2e-221">Response</span></span>
<span data-ttu-id="51e2e-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51e2e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1569

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled"
}
```




