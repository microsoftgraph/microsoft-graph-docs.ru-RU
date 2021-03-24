---
title: Обновление androidDeviceOwnerEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidDeviceOwnerEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3e31a85edf8a35b48ccf62cdcf7b9ef0bb8bb42
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133502"
---
# <a name="update-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="148eb-103">Обновление androidDeviceOwnerEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="148eb-103">Update androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="148eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="148eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="148eb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="148eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="148eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="148eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148eb-107">Обновление свойств объекта [androidDeviceOwnerEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-107">Update the properties of a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="148eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="148eb-108">Prerequisites</span></span>
<span data-ttu-id="148eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="148eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="148eb-111">Permission type</span></span>|<span data-ttu-id="148eb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="148eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="148eb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="148eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="148eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="148eb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="148eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="148eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="148eb-116">Not supported.</span></span>|
|<span data-ttu-id="148eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="148eb-117">Application</span></span>|<span data-ttu-id="148eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="148eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="148eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="148eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="148eb-120">Request headers</span></span>
|<span data-ttu-id="148eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="148eb-121">Header</span></span>|<span data-ttu-id="148eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="148eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="148eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="148eb-123">Authorization</span></span>|<span data-ttu-id="148eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="148eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="148eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="148eb-125">Accept</span></span>|<span data-ttu-id="148eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="148eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="148eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="148eb-127">Request body</span></span>
<span data-ttu-id="148eb-128">В теле запроса предоставляем представление JSON для [объекта AndroidDeviceOwnerEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="148eb-129">В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="148eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="148eb-130">Property</span></span>|<span data-ttu-id="148eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="148eb-131">Type</span></span>|<span data-ttu-id="148eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="148eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148eb-133">id</span><span class="sxs-lookup"><span data-stu-id="148eb-133">id</span></span>|<span data-ttu-id="148eb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-134">String</span></span>|<span data-ttu-id="148eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="148eb-135">Key of the entity.</span></span> <span data-ttu-id="148eb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="148eb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="148eb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148eb-138">DateTimeOffset</span></span>|<span data-ttu-id="148eb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="148eb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="148eb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="148eb-141">roleScopeTagIds</span></span>|<span data-ttu-id="148eb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="148eb-142">String collection</span></span>|<span data-ttu-id="148eb-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="148eb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="148eb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="148eb-145">supportsScopeTags</span></span>|<span data-ttu-id="148eb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="148eb-146">Boolean</span></span>|<span data-ttu-id="148eb-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="148eb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="148eb-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="148eb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="148eb-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="148eb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="148eb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="148eb-150">This property is read-only.</span></span> <span data-ttu-id="148eb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="148eb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="148eb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="148eb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="148eb-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="148eb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="148eb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="148eb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="148eb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="148eb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="148eb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="148eb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="148eb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="148eb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="148eb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="148eb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="148eb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="148eb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="148eb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="148eb-164">createdDateTime</span></span>|<span data-ttu-id="148eb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="148eb-165">DateTimeOffset</span></span>|<span data-ttu-id="148eb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="148eb-166">DateTime the object was created.</span></span> <span data-ttu-id="148eb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-168">description</span><span class="sxs-lookup"><span data-stu-id="148eb-168">description</span></span>|<span data-ttu-id="148eb-169">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-169">String</span></span>|<span data-ttu-id="148eb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="148eb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="148eb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="148eb-172">displayName</span></span>|<span data-ttu-id="148eb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-173">String</span></span>|<span data-ttu-id="148eb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="148eb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="148eb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-176">version</span><span class="sxs-lookup"><span data-stu-id="148eb-176">version</span></span>|<span data-ttu-id="148eb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="148eb-177">Int32</span></span>|<span data-ttu-id="148eb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="148eb-178">Version of the device configuration.</span></span> <span data-ttu-id="148eb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="148eb-180">networkName</span><span class="sxs-lookup"><span data-stu-id="148eb-180">networkName</span></span>|<span data-ttu-id="148eb-181">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-181">String</span></span>|<span data-ttu-id="148eb-182">Имя сети, унаследованные от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-182">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="148eb-183">ssid</span><span class="sxs-lookup"><span data-stu-id="148eb-183">ssid</span></span>|<span data-ttu-id="148eb-184">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-184">String</span></span>|<span data-ttu-id="148eb-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="148eb-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="148eb-186">Унаследованный от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-186">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="148eb-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="148eb-187">connectAutomatically</span></span>|<span data-ttu-id="148eb-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="148eb-188">Boolean</span></span>|<span data-ttu-id="148eb-189">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="148eb-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="148eb-190">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="148eb-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="148eb-191">Унаследованный от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-191">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="148eb-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="148eb-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="148eb-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="148eb-193">Boolean</span></span>|<span data-ttu-id="148eb-194">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="148eb-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="148eb-195">Унаследованный от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-195">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="148eb-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="148eb-196">wiFiSecurityType</span></span>|[<span data-ttu-id="148eb-197">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="148eb-197">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="148eb-198">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="148eb-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="148eb-199">Унаследовано от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="148eb-199">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="148eb-200">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="148eb-200">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="148eb-201">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="148eb-201">preSharedKey</span></span>|<span data-ttu-id="148eb-202">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-202">String</span></span>|<span data-ttu-id="148eb-203">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="148eb-203">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="148eb-204">Унаследованный от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-204">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="148eb-205">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="148eb-205">preSharedKeyIsSet</span></span>|<span data-ttu-id="148eb-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="148eb-206">Boolean</span></span>|<span data-ttu-id="148eb-207">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="148eb-207">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="148eb-208">Унаследованный от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="148eb-208">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="148eb-209">eapType</span><span class="sxs-lookup"><span data-stu-id="148eb-209">eapType</span></span>|[<span data-ttu-id="148eb-210">androidEapType</span><span class="sxs-lookup"><span data-stu-id="148eb-210">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="148eb-211">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="148eb-211">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="148eb-212">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="148eb-212">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="148eb-213">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="148eb-213">authenticationMethod</span></span>|[<span data-ttu-id="148eb-214">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="148eb-214">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="148eb-215">Указывает метод проверки подлинности, который клиент (устройство) должен использовать, когда тип EAP настроен на PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="148eb-215">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="148eb-216">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="148eb-216">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="148eb-217">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="148eb-217">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="148eb-218">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="148eb-218">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="148eb-219">Метод без EAP для проверки подлинности (внутренняя идентичность), когда тип EAP EAP-TTLS и authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="148eb-219">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="148eb-220">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="148eb-220">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="148eb-221">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="148eb-221">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="148eb-222">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="148eb-222">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="148eb-223">Метод без EAP для проверки подлинности (внутренняя идентичность), когда тип EAP — PEAP, а проверка подлинности — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="148eb-223">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="148eb-224">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="148eb-224">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="148eb-225">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="148eb-225">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="148eb-226">Строка</span><span class="sxs-lookup"><span data-stu-id="148eb-226">String</span></span>|<span data-ttu-id="148eb-227">Введите конфиденциальность удостоверений (внешний идентификатор), если тип EAP настроен на EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="148eb-227">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="148eb-228">Строка, представленная здесь, используется для маскировки имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="148eb-228">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="148eb-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="148eb-229">Response</span></span>
<span data-ttu-id="148eb-230">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="148eb-230">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="148eb-231">Пример</span><span class="sxs-lookup"><span data-stu-id="148eb-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="148eb-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="148eb-232">Request</span></span>
<span data-ttu-id="148eb-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="148eb-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1612

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="148eb-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="148eb-234">Response</span></span>
<span data-ttu-id="148eb-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="148eb-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1784

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
  "id": "7ef0d9c3-d9c3-7ef0-c3d9-f07ec3d9f07e",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




