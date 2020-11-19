---
title: Создание windows10DeviceFirmwareConfigurationInterface
description: Создание нового объекта windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0efe13dd839e45ad2cfeb390e3600eaa5b4d6dd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236220"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="a8323-103">Создание windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="a8323-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

<span data-ttu-id="a8323-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8323-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8323-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8323-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8323-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8323-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8323-107">Создание нового объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .</span><span class="sxs-lookup"><span data-stu-id="a8323-107">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8323-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a8323-108">Prerequisites</span></span>
<span data-ttu-id="a8323-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8323-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8323-111">Permission type</span></span>|<span data-ttu-id="a8323-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8323-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8323-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8323-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8323-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8323-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8323-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8323-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8323-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8323-116">Not supported.</span></span>|
|<span data-ttu-id="a8323-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a8323-117">Application</span></span>|<span data-ttu-id="a8323-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8323-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8323-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8323-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8323-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a8323-120">Request headers</span></span>
|<span data-ttu-id="a8323-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8323-121">Header</span></span>|<span data-ttu-id="a8323-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8323-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8323-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8323-123">Authorization</span></span>|<span data-ttu-id="a8323-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8323-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8323-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8323-125">Accept</span></span>|<span data-ttu-id="a8323-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8323-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8323-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8323-127">Request body</span></span>
<span data-ttu-id="a8323-128">В тексте запроса добавьте представление объекта windows10DeviceFirmwareConfigurationInterface в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8323-128">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="a8323-129">В следующей таблице приведены свойства, необходимые при создании windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="a8323-129">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="a8323-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8323-130">Property</span></span>|<span data-ttu-id="a8323-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a8323-131">Type</span></span>|<span data-ttu-id="a8323-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a8323-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8323-133">id</span><span class="sxs-lookup"><span data-stu-id="a8323-133">id</span></span>|<span data-ttu-id="a8323-134">String</span><span class="sxs-lookup"><span data-stu-id="a8323-134">String</span></span>|<span data-ttu-id="a8323-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8323-135">Key of the entity.</span></span> <span data-ttu-id="a8323-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8323-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a8323-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8323-138">DateTimeOffset</span></span>|<span data-ttu-id="a8323-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a8323-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a8323-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8323-141">roleScopeTagIds</span></span>|<span data-ttu-id="a8323-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a8323-142">String collection</span></span>|<span data-ttu-id="a8323-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a8323-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8323-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a8323-145">supportsScopeTags</span></span>|<span data-ttu-id="a8323-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8323-146">Boolean</span></span>|<span data-ttu-id="a8323-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a8323-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8323-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a8323-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8323-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a8323-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8323-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8323-150">This property is read-only.</span></span> <span data-ttu-id="a8323-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8323-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a8323-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8323-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a8323-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8323-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a8323-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8323-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a8323-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8323-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a8323-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8323-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a8323-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8323-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a8323-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8323-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a8323-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8323-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a8323-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8323-164">createdDateTime</span></span>|<span data-ttu-id="a8323-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8323-165">DateTimeOffset</span></span>|<span data-ttu-id="a8323-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a8323-166">DateTime the object was created.</span></span> <span data-ttu-id="a8323-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-168">description</span><span class="sxs-lookup"><span data-stu-id="a8323-168">description</span></span>|<span data-ttu-id="a8323-169">String</span><span class="sxs-lookup"><span data-stu-id="a8323-169">String</span></span>|<span data-ttu-id="a8323-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8323-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8323-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a8323-172">displayName</span></span>|<span data-ttu-id="a8323-173">String</span><span class="sxs-lookup"><span data-stu-id="a8323-173">String</span></span>|<span data-ttu-id="a8323-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8323-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8323-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-176">version</span><span class="sxs-lookup"><span data-stu-id="a8323-176">version</span></span>|<span data-ttu-id="a8323-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a8323-177">Int32</span></span>|<span data-ttu-id="a8323-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8323-178">Version of the device configuration.</span></span> <span data-ttu-id="a8323-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8323-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8323-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="a8323-180">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="a8323-181">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="a8323-181">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="a8323-182">Определяет уровень разрешений, который предоставляется пользователям для изменения параметров UEFI.</span><span class="sxs-lookup"><span data-stu-id="a8323-182">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="a8323-183">Возможные значения: `notConfiguredOnly`, `none`.</span><span class="sxs-lookup"><span data-stu-id="a8323-183">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="a8323-184">виртуализатионофкпуандио</span><span class="sxs-lookup"><span data-stu-id="a8323-184">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="a8323-185">Включение</span><span class="sxs-lookup"><span data-stu-id="a8323-185">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a8323-186">Определяет, включена ли виртуализация ЦП и ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="a8323-186">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="a8323-187">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a8323-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a8323-188">камер</span><span class="sxs-lookup"><span data-stu-id="a8323-188">cameras</span></span>|[<span data-ttu-id="a8323-189">Включение</span><span class="sxs-lookup"><span data-stu-id="a8323-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a8323-190">Определяет, включены ли встроенные камеры.</span><span class="sxs-lookup"><span data-stu-id="a8323-190">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="a8323-191">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a8323-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a8323-192">микрофонесандспеакерс</span><span class="sxs-lookup"><span data-stu-id="a8323-192">microphonesAndSpeakers</span></span>|[<span data-ttu-id="a8323-193">Включение</span><span class="sxs-lookup"><span data-stu-id="a8323-193">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a8323-194">Определяет, включены ли встроенные микрофоны или динамики.</span><span class="sxs-lookup"><span data-stu-id="a8323-194">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="a8323-195">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a8323-195">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a8323-196">Радио</span><span class="sxs-lookup"><span data-stu-id="a8323-196">radios</span></span>|[<span data-ttu-id="a8323-197">Включение</span><span class="sxs-lookup"><span data-stu-id="a8323-197">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a8323-198">Определяет, включены ли встроенные радиостанции, например Wi-Fi, NFC, Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="a8323-198">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="a8323-199">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a8323-199">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a8323-200">бутфромекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="a8323-200">bootFromExternalMedia</span></span>|[<span data-ttu-id="a8323-201">Включение</span><span class="sxs-lookup"><span data-stu-id="a8323-201">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a8323-202">Определяет, может ли пользователь загружаться с внешнего носителя.</span><span class="sxs-lookup"><span data-stu-id="a8323-202">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="a8323-203">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a8323-203">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a8323-204">бутфромбуилтиннетворкадаптерс</span><span class="sxs-lookup"><span data-stu-id="a8323-204">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="a8323-205">Включение</span><span class="sxs-lookup"><span data-stu-id="a8323-205">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a8323-206">Определяет, может ли пользователь загружаться со встроенных сетевых адаптеров.</span><span class="sxs-lookup"><span data-stu-id="a8323-206">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="a8323-207">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a8323-207">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a8323-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8323-208">Response</span></span>
<span data-ttu-id="a8323-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8323-209">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8323-210">Пример</span><span class="sxs-lookup"><span data-stu-id="a8323-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8323-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8323-211">Request</span></span>
<span data-ttu-id="a8323-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8323-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8323-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8323-213">Response</span></span>
<span data-ttu-id="a8323-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8323-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




