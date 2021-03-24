---
title: Создание windows10DeviceFirmwareConfigurationInterface
description: Создайте новый объект Windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea749cf9499031a8b0746ce06b4f9070c2b4f444
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147506"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="31159-103">Создание windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="31159-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

<span data-ttu-id="31159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31159-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31159-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31159-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31159-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31159-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31159-107">Создайте [новый объект Windows10DeviceFirmwareConfigurationInterface.](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)</span><span class="sxs-lookup"><span data-stu-id="31159-107">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31159-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31159-108">Prerequisites</span></span>
<span data-ttu-id="31159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31159-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31159-111">Permission type</span></span>|<span data-ttu-id="31159-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31159-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31159-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31159-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31159-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31159-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31159-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31159-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31159-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31159-116">Not supported.</span></span>|
|<span data-ttu-id="31159-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="31159-117">Application</span></span>|<span data-ttu-id="31159-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31159-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31159-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31159-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31159-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31159-120">Request headers</span></span>
|<span data-ttu-id="31159-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31159-121">Header</span></span>|<span data-ttu-id="31159-122">Значение</span><span class="sxs-lookup"><span data-stu-id="31159-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31159-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31159-123">Authorization</span></span>|<span data-ttu-id="31159-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31159-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31159-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31159-125">Accept</span></span>|<span data-ttu-id="31159-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31159-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31159-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31159-127">Request body</span></span>
<span data-ttu-id="31159-128">В корпусе запроса предоставляем представление JSON для объекта Windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="31159-128">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="31159-129">В следующей таблице показаны свойства, необходимые при создании windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="31159-129">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="31159-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="31159-130">Property</span></span>|<span data-ttu-id="31159-131">Тип</span><span class="sxs-lookup"><span data-stu-id="31159-131">Type</span></span>|<span data-ttu-id="31159-132">Описание</span><span class="sxs-lookup"><span data-stu-id="31159-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31159-133">id</span><span class="sxs-lookup"><span data-stu-id="31159-133">id</span></span>|<span data-ttu-id="31159-134">Строка</span><span class="sxs-lookup"><span data-stu-id="31159-134">String</span></span>|<span data-ttu-id="31159-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31159-135">Key of the entity.</span></span> <span data-ttu-id="31159-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31159-137">lastModifiedDateTime</span></span>|<span data-ttu-id="31159-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31159-138">DateTimeOffset</span></span>|<span data-ttu-id="31159-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="31159-139">DateTime the object was last modified.</span></span> <span data-ttu-id="31159-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31159-141">roleScopeTagIds</span></span>|<span data-ttu-id="31159-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31159-142">String collection</span></span>|<span data-ttu-id="31159-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="31159-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31159-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="31159-145">supportsScopeTags</span></span>|<span data-ttu-id="31159-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="31159-146">Boolean</span></span>|<span data-ttu-id="31159-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="31159-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31159-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="31159-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31159-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="31159-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31159-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31159-150">This property is read-only.</span></span> <span data-ttu-id="31159-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31159-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="31159-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="31159-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="31159-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="31159-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="31159-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="31159-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="31159-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="31159-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="31159-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="31159-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="31159-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="31159-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="31159-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="31159-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="31159-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="31159-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="31159-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31159-164">createdDateTime</span></span>|<span data-ttu-id="31159-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31159-165">DateTimeOffset</span></span>|<span data-ttu-id="31159-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="31159-166">DateTime the object was created.</span></span> <span data-ttu-id="31159-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-168">description</span><span class="sxs-lookup"><span data-stu-id="31159-168">description</span></span>|<span data-ttu-id="31159-169">Строка</span><span class="sxs-lookup"><span data-stu-id="31159-169">String</span></span>|<span data-ttu-id="31159-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31159-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31159-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-172">displayName</span><span class="sxs-lookup"><span data-stu-id="31159-172">displayName</span></span>|<span data-ttu-id="31159-173">Строка</span><span class="sxs-lookup"><span data-stu-id="31159-173">String</span></span>|<span data-ttu-id="31159-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31159-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31159-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-176">version</span><span class="sxs-lookup"><span data-stu-id="31159-176">version</span></span>|<span data-ttu-id="31159-177">Int32</span><span class="sxs-lookup"><span data-stu-id="31159-177">Int32</span></span>|<span data-ttu-id="31159-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31159-178">Version of the device configuration.</span></span> <span data-ttu-id="31159-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31159-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31159-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="31159-180">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="31159-181">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="31159-181">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="31159-182">Определяет уровень разрешений, предоставленный пользователям для изменения параметров UEFI.</span><span class="sxs-lookup"><span data-stu-id="31159-182">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="31159-183">Возможные значения: `notConfiguredOnly`, `none`.</span><span class="sxs-lookup"><span data-stu-id="31159-183">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="31159-184">виртуализацияOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="31159-184">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="31159-185">включить</span><span class="sxs-lookup"><span data-stu-id="31159-185">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="31159-186">Определяет, включена ли виртуализация ЦП и IO.</span><span class="sxs-lookup"><span data-stu-id="31159-186">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="31159-187">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="31159-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="31159-188">камеры</span><span class="sxs-lookup"><span data-stu-id="31159-188">cameras</span></span>|[<span data-ttu-id="31159-189">включить</span><span class="sxs-lookup"><span data-stu-id="31159-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="31159-190">Определяет, включены ли встроенные камеры.</span><span class="sxs-lookup"><span data-stu-id="31159-190">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="31159-191">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="31159-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="31159-192">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="31159-192">microphonesAndSpeakers</span></span>|[<span data-ttu-id="31159-193">включить</span><span class="sxs-lookup"><span data-stu-id="31159-193">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="31159-194">Определяет, включены ли встроенные микрофоны или динамики.</span><span class="sxs-lookup"><span data-stu-id="31159-194">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="31159-195">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="31159-195">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="31159-196">радио</span><span class="sxs-lookup"><span data-stu-id="31159-196">radios</span></span>|[<span data-ttu-id="31159-197">включить</span><span class="sxs-lookup"><span data-stu-id="31159-197">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="31159-198">Определяет, включены ли встроенные радиостанции, например WIFI, NFC, Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="31159-198">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="31159-199">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="31159-199">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="31159-200">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="31159-200">bootFromExternalMedia</span></span>|[<span data-ttu-id="31159-201">включить</span><span class="sxs-lookup"><span data-stu-id="31159-201">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="31159-202">Определяет, разрешено ли пользователю загрузиться из внешних мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="31159-202">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="31159-203">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="31159-203">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="31159-204">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="31159-204">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="31159-205">включить</span><span class="sxs-lookup"><span data-stu-id="31159-205">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="31159-206">Определяет, разрешена ли пользователю загрузка из встроенных сетевых адаптеров.</span><span class="sxs-lookup"><span data-stu-id="31159-206">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="31159-207">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="31159-207">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="31159-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="31159-208">Response</span></span>
<span data-ttu-id="31159-209">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект Windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="31159-209">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31159-210">Пример</span><span class="sxs-lookup"><span data-stu-id="31159-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="31159-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="31159-211">Request</span></span>
<span data-ttu-id="31159-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31159-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1309

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
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="31159-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="31159-213">Response</span></span>
<span data-ttu-id="31159-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31159-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1481

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
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```




