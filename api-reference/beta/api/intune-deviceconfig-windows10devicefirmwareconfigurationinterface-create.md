---
title: Создание windows10DeviceFirmwareConfigurationInterface
description: Создание нового объекта windows10DeviceFirmwareConfigurationInterface.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 998935ac319a0ecd1643e70ca7c4d5da0d0a9806
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314681"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="cb6d8-103">Создание windows10DeviceFirmwareConfigurationInterface</span><span class="sxs-lookup"><span data-stu-id="cb6d8-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

> <span data-ttu-id="cb6d8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb6d8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb6d8-106">Создание нового объекта [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .</span><span class="sxs-lookup"><span data-stu-id="cb6d8-106">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb6d8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb6d8-107">Prerequisites</span></span>
<span data-ttu-id="cb6d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb6d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb6d8-110">Permission type</span></span>|<span data-ttu-id="cb6d8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb6d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb6d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb6d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb6d8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6d8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb6d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb6d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb6d8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-115">Not supported.</span></span>|
|<span data-ttu-id="cb6d8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb6d8-116">Application</span></span>|<span data-ttu-id="cb6d8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6d8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb6d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb6d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cb6d8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb6d8-119">Request headers</span></span>
|<span data-ttu-id="cb6d8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb6d8-120">Header</span></span>|<span data-ttu-id="cb6d8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb6d8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb6d8-122">Authorization</span></span>|<span data-ttu-id="cb6d8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb6d8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cb6d8-124">Accept</span></span>|<span data-ttu-id="cb6d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb6d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb6d8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb6d8-126">Request body</span></span>
<span data-ttu-id="cb6d8-127">В тексте запроса добавьте представление объекта windows10DeviceFirmwareConfigurationInterface в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-127">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="cb6d8-128">В следующей таблице приведены свойства, необходимые при создании windows10DeviceFirmwareConfigurationInterface.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-128">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="cb6d8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb6d8-129">Property</span></span>|<span data-ttu-id="cb6d8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cb6d8-130">Type</span></span>|<span data-ttu-id="cb6d8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cb6d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6d8-132">id</span><span class="sxs-lookup"><span data-stu-id="cb6d8-132">id</span></span>|<span data-ttu-id="cb6d8-133">String</span><span class="sxs-lookup"><span data-stu-id="cb6d8-133">String</span></span>|<span data-ttu-id="cb6d8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-134">Key of the entity.</span></span> <span data-ttu-id="cb6d8-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb6d8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cb6d8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb6d8-137">DateTimeOffset</span></span>|<span data-ttu-id="cb6d8-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cb6d8-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb6d8-140">roleScopeTagIds</span></span>|<span data-ttu-id="cb6d8-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cb6d8-141">String collection</span></span>|<span data-ttu-id="cb6d8-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cb6d8-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cb6d8-144">supportsScopeTags</span></span>|<span data-ttu-id="cb6d8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb6d8-145">Boolean</span></span>|<span data-ttu-id="cb6d8-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cb6d8-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cb6d8-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cb6d8-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-149">This property is read-only.</span></span> <span data-ttu-id="cb6d8-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cb6d8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cb6d8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cb6d8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cb6d8-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cb6d8-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cb6d8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cb6d8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cb6d8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cb6d8-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cb6d8-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="cb6d8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cb6d8-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="cb6d8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cb6d8-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cb6d8-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb6d8-163">createdDateTime</span></span>|<span data-ttu-id="cb6d8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb6d8-164">DateTimeOffset</span></span>|<span data-ttu-id="cb6d8-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-165">DateTime the object was created.</span></span> <span data-ttu-id="cb6d8-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-167">description</span><span class="sxs-lookup"><span data-stu-id="cb6d8-167">description</span></span>|<span data-ttu-id="cb6d8-168">String</span><span class="sxs-lookup"><span data-stu-id="cb6d8-168">String</span></span>|<span data-ttu-id="cb6d8-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb6d8-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="cb6d8-171">displayName</span></span>|<span data-ttu-id="cb6d8-172">Строка</span><span class="sxs-lookup"><span data-stu-id="cb6d8-172">String</span></span>|<span data-ttu-id="cb6d8-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb6d8-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-175">version</span><span class="sxs-lookup"><span data-stu-id="cb6d8-175">version</span></span>|<span data-ttu-id="cb6d8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="cb6d8-176">Int32</span></span>|<span data-ttu-id="cb6d8-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-177">Version of the device configuration.</span></span> <span data-ttu-id="cb6d8-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb6d8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb6d8-179">чанжеуефисеттингспермиссион</span><span class="sxs-lookup"><span data-stu-id="cb6d8-179">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="cb6d8-180">чанжеуефисеттингспермиссион</span><span class="sxs-lookup"><span data-stu-id="cb6d8-180">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="cb6d8-181">Определяет уровень разрешений, который предоставляется пользователям для изменения параметров UEFI.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-181">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="cb6d8-182">Возможные значения: `notConfiguredOnly`, `none`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-182">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="cb6d8-183">виртуализатионофкпуандио</span><span class="sxs-lookup"><span data-stu-id="cb6d8-183">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="cb6d8-184">Включение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cb6d8-185">Определяет, включена ли виртуализация ЦП и ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-185">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="cb6d8-186">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cb6d8-187">камер</span><span class="sxs-lookup"><span data-stu-id="cb6d8-187">cameras</span></span>|[<span data-ttu-id="cb6d8-188">Включение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cb6d8-189">Определяет, включены ли встроенные камеры.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-189">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="cb6d8-190">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cb6d8-191">микрофонесандспеакерс</span><span class="sxs-lookup"><span data-stu-id="cb6d8-191">microphonesAndSpeakers</span></span>|[<span data-ttu-id="cb6d8-192">Включение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cb6d8-193">Определяет, включены ли встроенные микрофоны или динамики.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-193">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="cb6d8-194">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cb6d8-195">Радио</span><span class="sxs-lookup"><span data-stu-id="cb6d8-195">radios</span></span>|[<span data-ttu-id="cb6d8-196">Включение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cb6d8-197">Определяет, включены ли встроенные радиостанции, например Wi-Fi, NFC, Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-197">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="cb6d8-198">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cb6d8-199">бутфромекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="cb6d8-199">bootFromExternalMedia</span></span>|[<span data-ttu-id="cb6d8-200">Включение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cb6d8-201">Определяет, может ли пользователь загружаться с внешнего носителя.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-201">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="cb6d8-202">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cb6d8-203">бутфромбуилтиннетворкадаптерс</span><span class="sxs-lookup"><span data-stu-id="cb6d8-203">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="cb6d8-204">Включение</span><span class="sxs-lookup"><span data-stu-id="cb6d8-204">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="cb6d8-205">Определяет, может ли пользователь загружаться со встроенных сетевых адаптеров.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-205">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="cb6d8-206">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="cb6d8-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb6d8-207">Response</span></span>
<span data-ttu-id="cb6d8-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-208">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb6d8-209">Пример</span><span class="sxs-lookup"><span data-stu-id="cb6d8-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb6d8-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb6d8-210">Request</span></span>
<span data-ttu-id="cb6d8-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb6d8-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb6d8-212">Response</span></span>
<span data-ttu-id="cb6d8-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb6d8-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






