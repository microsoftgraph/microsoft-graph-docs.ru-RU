---
title: Обновление iosEnterpriseWiFiConfiguration
description: Обновление свойств объекта iosEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76022c7bf57a719c46d36afecf0989696574615e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131570"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="7686f-103">Обновление iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="7686f-103">Update iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="7686f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7686f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7686f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7686f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7686f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7686f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7686f-107">Обновление свойств объекта [iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-107">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7686f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7686f-108">Prerequisites</span></span>
<span data-ttu-id="7686f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7686f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7686f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7686f-111">Permission type</span></span>|<span data-ttu-id="7686f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7686f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7686f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7686f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7686f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7686f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7686f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7686f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7686f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7686f-116">Not supported.</span></span>|
|<span data-ttu-id="7686f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7686f-117">Application</span></span>|<span data-ttu-id="7686f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7686f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7686f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7686f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7686f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7686f-120">Request headers</span></span>
|<span data-ttu-id="7686f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7686f-121">Header</span></span>|<span data-ttu-id="7686f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7686f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7686f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7686f-123">Authorization</span></span>|<span data-ttu-id="7686f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7686f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7686f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7686f-125">Accept</span></span>|<span data-ttu-id="7686f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7686f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7686f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7686f-127">Request body</span></span>
<span data-ttu-id="7686f-128">В теле запроса поставляем представление JSON для [объекта iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-128">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="7686f-129">В следующей таблице показаны свойства, необходимые при создании [iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-129">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="7686f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7686f-130">Property</span></span>|<span data-ttu-id="7686f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7686f-131">Type</span></span>|<span data-ttu-id="7686f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7686f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7686f-133">id</span><span class="sxs-lookup"><span data-stu-id="7686f-133">id</span></span>|<span data-ttu-id="7686f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-134">String</span></span>|<span data-ttu-id="7686f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7686f-135">Key of the entity.</span></span> <span data-ttu-id="7686f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7686f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7686f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7686f-138">DateTimeOffset</span></span>|<span data-ttu-id="7686f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7686f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7686f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7686f-141">roleScopeTagIds</span></span>|<span data-ttu-id="7686f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7686f-142">String collection</span></span>|<span data-ttu-id="7686f-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="7686f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7686f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7686f-145">supportsScopeTags</span></span>|<span data-ttu-id="7686f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7686f-146">Boolean</span></span>|<span data-ttu-id="7686f-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7686f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7686f-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="7686f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7686f-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7686f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7686f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7686f-150">This property is read-only.</span></span> <span data-ttu-id="7686f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7686f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7686f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7686f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7686f-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7686f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7686f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7686f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7686f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7686f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7686f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7686f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7686f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7686f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7686f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7686f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7686f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7686f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7686f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7686f-164">createdDateTime</span></span>|<span data-ttu-id="7686f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7686f-165">DateTimeOffset</span></span>|<span data-ttu-id="7686f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7686f-166">DateTime the object was created.</span></span> <span data-ttu-id="7686f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-168">description</span><span class="sxs-lookup"><span data-stu-id="7686f-168">description</span></span>|<span data-ttu-id="7686f-169">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-169">String</span></span>|<span data-ttu-id="7686f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7686f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7686f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7686f-172">displayName</span></span>|<span data-ttu-id="7686f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-173">String</span></span>|<span data-ttu-id="7686f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7686f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7686f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-176">version</span><span class="sxs-lookup"><span data-stu-id="7686f-176">version</span></span>|<span data-ttu-id="7686f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7686f-177">Int32</span></span>|<span data-ttu-id="7686f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7686f-178">Version of the device configuration.</span></span> <span data-ttu-id="7686f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7686f-180">networkName</span><span class="sxs-lookup"><span data-stu-id="7686f-180">networkName</span></span>|<span data-ttu-id="7686f-181">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-181">String</span></span>|<span data-ttu-id="7686f-182">Имя сети, унаследованные от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-183">ssid</span><span class="sxs-lookup"><span data-stu-id="7686f-183">ssid</span></span>|<span data-ttu-id="7686f-184">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-184">String</span></span>|<span data-ttu-id="7686f-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="7686f-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="7686f-186">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="7686f-187">connectAutomatically</span></span>|<span data-ttu-id="7686f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="7686f-188">Boolean</span></span>|<span data-ttu-id="7686f-189">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="7686f-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="7686f-190">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="7686f-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="7686f-191">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="7686f-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="7686f-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7686f-193">Boolean</span></span>|<span data-ttu-id="7686f-194">Подключение, если сеть не передает свое имя (SSID).</span><span class="sxs-lookup"><span data-stu-id="7686f-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="7686f-195">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="7686f-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="7686f-196">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7686f-197">wiFiSecurityType</span></span>|[<span data-ttu-id="7686f-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7686f-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="7686f-199">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="7686f-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="7686f-200">Наследуется [от iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7686f-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="7686f-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="7686f-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="7686f-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="7686f-202">proxySettings</span></span>|[<span data-ttu-id="7686f-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="7686f-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="7686f-204">Тип прокси для этого Wi-Fi, унаследованный от [iosWiFiConfiguration.](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="7686f-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="7686f-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="7686f-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="7686f-206">proxyManualAddress</span></span>|<span data-ttu-id="7686f-207">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-207">String</span></span>|<span data-ttu-id="7686f-208">IP-адрес или DNS-имя прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="7686f-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="7686f-209">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="7686f-210">proxyManualPort</span></span>|<span data-ttu-id="7686f-211">Int32</span><span class="sxs-lookup"><span data-stu-id="7686f-211">Int32</span></span>|<span data-ttu-id="7686f-212">Порт прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="7686f-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="7686f-213">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="7686f-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="7686f-215">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-215">String</span></span>|<span data-ttu-id="7686f-216">URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации.</span><span class="sxs-lookup"><span data-stu-id="7686f-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="7686f-217">Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration).</span><span class="sxs-lookup"><span data-stu-id="7686f-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="7686f-218">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-219">отключениеMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="7686f-219">disableMacAddressRandomization</span></span>|<span data-ttu-id="7686f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7686f-220">Boolean</span></span>|<span data-ttu-id="7686f-221">Если установлено истинное, устройства, подключающиеся с помощью этого Wi-Fi профиля, должны представить Wi-Fi mac-адрес, а не случайный MAC-адрес.</span><span class="sxs-lookup"><span data-stu-id="7686f-221">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="7686f-222">Применяется к iOS 14 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="7686f-222">Applies to iOS 14 and later.</span></span> <span data-ttu-id="7686f-223">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-223">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-224">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="7686f-224">preSharedKey</span></span>|<span data-ttu-id="7686f-225">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-225">String</span></span>|<span data-ttu-id="7686f-226">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="7686f-226">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="7686f-227">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7686f-227">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="7686f-228">eapType</span><span class="sxs-lookup"><span data-stu-id="7686f-228">eapType</span></span>|[<span data-ttu-id="7686f-229">eapType</span><span class="sxs-lookup"><span data-stu-id="7686f-229">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="7686f-230">Extensible Authentication Protocol (EAP).</span><span class="sxs-lookup"><span data-stu-id="7686f-230">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="7686f-231">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="7686f-231">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="7686f-232">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="7686f-232">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="7686f-233">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="7686f-233">eapFastConfiguration</span></span>|[<span data-ttu-id="7686f-234">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="7686f-234">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="7686f-235">Параметр конфигурации EAP-FAST, когда EAP-FAST является выбранным типом EAP.</span><span class="sxs-lookup"><span data-stu-id="7686f-235">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="7686f-236">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="7686f-236">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="7686f-237">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="7686f-237">trustedServerCertificateNames</span></span>|<span data-ttu-id="7686f-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7686f-238">String collection</span></span>|<span data-ttu-id="7686f-239">Доверенные имена сертификатов сервера при настройке типа EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="7686f-239">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="7686f-240">Это общее имя, используемая в сертификатах, выдаванных доверенным органом сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="7686f-240">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="7686f-241">Если вы предоставите эту информацию, можно обойти динамический диалог доверия, отображаемый на устройствах конечных пользователей при подключении к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="7686f-241">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="7686f-242">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7686f-242">authenticationMethod</span></span>|[<span data-ttu-id="7686f-243">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7686f-243">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="7686f-244">Метод проверки подлинности при настройке типа EAP на PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="7686f-244">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="7686f-245">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7686f-245">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7686f-246">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="7686f-246">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="7686f-247">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="7686f-247">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="7686f-248">Метод без EAP для проверки подлинности, если тип EAP — EAP-TTLS, а проверка подлинности — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="7686f-248">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="7686f-249">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="7686f-249">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="7686f-250">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="7686f-250">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="7686f-251">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-251">String</span></span>|<span data-ttu-id="7686f-252">Включить конфиденциальность удостоверений (внешний идентификатор), когда тип EAP настроен на EAP - TTLS, EAP - FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="7686f-252">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="7686f-253">Это свойство маскирует имена пользователей с вводимым текстом.</span><span class="sxs-lookup"><span data-stu-id="7686f-253">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="7686f-254">Например, если используется "анонимный", каждый пользователь, который Wi-Fi с этим подключением, используя свое реальное имя пользователя, отображается как "анонимный".</span><span class="sxs-lookup"><span data-stu-id="7686f-254">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="7686f-255">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="7686f-255">usernameFormatString</span></span>|<span data-ttu-id="7686f-256">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-256">String</span></span>|<span data-ttu-id="7686f-257">Строка формата username, используемая для создания имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="7686f-257">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="7686f-258">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="7686f-258">passwordFormatString</span></span>|<span data-ttu-id="7686f-259">Строка</span><span class="sxs-lookup"><span data-stu-id="7686f-259">String</span></span>|<span data-ttu-id="7686f-260">Строка формата пароля, используемая для создания пароля для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="7686f-260">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="7686f-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="7686f-261">Response</span></span>
<span data-ttu-id="7686f-262">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7686f-262">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7686f-263">Пример</span><span class="sxs-lookup"><span data-stu-id="7686f-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="7686f-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="7686f-264">Request</span></span>
<span data-ttu-id="7686f-265">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7686f-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2017

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="7686f-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="7686f-266">Response</span></span>
<span data-ttu-id="7686f-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7686f-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2189

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```




