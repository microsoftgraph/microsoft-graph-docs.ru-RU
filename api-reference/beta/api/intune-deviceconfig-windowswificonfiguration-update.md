---
title: Обновление windowsWifiConfiguration
description: Обновление свойств объекта WindowsWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adae47a270925418333b2ad30700680fcbaf912e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127188"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="b3f33-103">Обновление windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3f33-103">Update windowsWifiConfiguration</span></span>

<span data-ttu-id="b3f33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3f33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3f33-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3f33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3f33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3f33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3f33-107">Обновление свойств объекта [WindowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3f33-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3f33-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b3f33-108">Prerequisites</span></span>
<span data-ttu-id="b3f33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3f33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3f33-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3f33-111">Permission type</span></span>|<span data-ttu-id="b3f33-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3f33-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3f33-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3f33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3f33-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3f33-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3f33-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3f33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3f33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3f33-116">Not supported.</span></span>|
|<span data-ttu-id="b3f33-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3f33-117">Application</span></span>|<span data-ttu-id="b3f33-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3f33-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3f33-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3f33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3f33-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b3f33-120">Request headers</span></span>
|<span data-ttu-id="b3f33-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3f33-121">Header</span></span>|<span data-ttu-id="b3f33-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3f33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3f33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3f33-123">Authorization</span></span>|<span data-ttu-id="b3f33-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3f33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3f33-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3f33-125">Accept</span></span>|<span data-ttu-id="b3f33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3f33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3f33-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3f33-127">Request body</span></span>
<span data-ttu-id="b3f33-128">В теле запроса устрой представление JSON для [объекта WindowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3f33-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="b3f33-129">В следующей таблице показаны свойства, необходимые при создании [windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3f33-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="b3f33-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3f33-130">Property</span></span>|<span data-ttu-id="b3f33-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3f33-131">Type</span></span>|<span data-ttu-id="b3f33-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3f33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3f33-133">id</span><span class="sxs-lookup"><span data-stu-id="b3f33-133">id</span></span>|<span data-ttu-id="b3f33-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-134">String</span></span>|<span data-ttu-id="b3f33-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3f33-135">Key of the entity.</span></span> <span data-ttu-id="b3f33-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3f33-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b3f33-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3f33-138">DateTimeOffset</span></span>|<span data-ttu-id="b3f33-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b3f33-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b3f33-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3f33-141">roleScopeTagIds</span></span>|<span data-ttu-id="b3f33-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3f33-142">String collection</span></span>|<span data-ttu-id="b3f33-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="b3f33-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3f33-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3f33-145">supportsScopeTags</span></span>|<span data-ttu-id="b3f33-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f33-146">Boolean</span></span>|<span data-ttu-id="b3f33-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b3f33-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3f33-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="b3f33-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3f33-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b3f33-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3f33-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b3f33-150">This property is read-only.</span></span> <span data-ttu-id="b3f33-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3f33-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b3f33-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3f33-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b3f33-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b3f33-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b3f33-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3f33-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b3f33-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3f33-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b3f33-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b3f33-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b3f33-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3f33-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b3f33-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3f33-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b3f33-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b3f33-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b3f33-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3f33-164">createdDateTime</span></span>|<span data-ttu-id="b3f33-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3f33-165">DateTimeOffset</span></span>|<span data-ttu-id="b3f33-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b3f33-166">DateTime the object was created.</span></span> <span data-ttu-id="b3f33-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-168">description</span><span class="sxs-lookup"><span data-stu-id="b3f33-168">description</span></span>|<span data-ttu-id="b3f33-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-169">String</span></span>|<span data-ttu-id="b3f33-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3f33-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3f33-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b3f33-172">displayName</span></span>|<span data-ttu-id="b3f33-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-173">String</span></span>|<span data-ttu-id="b3f33-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3f33-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3f33-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-176">version</span><span class="sxs-lookup"><span data-stu-id="b3f33-176">version</span></span>|<span data-ttu-id="b3f33-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b3f33-177">Int32</span></span>|<span data-ttu-id="b3f33-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3f33-178">Version of the device configuration.</span></span> <span data-ttu-id="b3f33-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3f33-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3f33-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b3f33-180">preSharedKey</span></span>|<span data-ttu-id="b3f33-181">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-181">String</span></span>|<span data-ttu-id="b3f33-182">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="b3f33-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="b3f33-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b3f33-183">wifiSecurityType</span></span>|[<span data-ttu-id="b3f33-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b3f33-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="b3f33-185">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b3f33-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="b3f33-186">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="b3f33-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="b3f33-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="b3f33-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="b3f33-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="b3f33-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="b3f33-189">Укажите тип ограничения дозы подключения для подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b3f33-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="b3f33-190">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="b3f33-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="b3f33-191">ssid</span><span class="sxs-lookup"><span data-stu-id="b3f33-191">ssid</span></span>|<span data-ttu-id="b3f33-192">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-192">String</span></span>|<span data-ttu-id="b3f33-193">Укажите SSID подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b3f33-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="b3f33-194">networkName</span><span class="sxs-lookup"><span data-stu-id="b3f33-194">networkName</span></span>|<span data-ttu-id="b3f33-195">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-195">String</span></span>|<span data-ttu-id="b3f33-196">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="b3f33-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="b3f33-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b3f33-197">connectAutomatically</span></span>|<span data-ttu-id="b3f33-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f33-198">Boolean</span></span>|<span data-ttu-id="b3f33-199">Укажите, должно ли подключение Wi-Fi подключаться автоматически при диапазоне.</span><span class="sxs-lookup"><span data-stu-id="b3f33-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="b3f33-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="b3f33-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="b3f33-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f33-201">Boolean</span></span>|<span data-ttu-id="b3f33-202">Укажите, должно ли подключение Wi-Fi подключаться к более предпочтительным сетям при уже подключении к этой.</span><span class="sxs-lookup"><span data-stu-id="b3f33-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="b3f33-203">Требуется, чтобы ConnectAutomatically был правдивым.</span><span class="sxs-lookup"><span data-stu-id="b3f33-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="b3f33-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b3f33-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b3f33-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f33-205">Boolean</span></span>|<span data-ttu-id="b3f33-206">Укажите, следует ли подключать подключение к Wi-Fi автоматически, даже если SSID не транслируется.</span><span class="sxs-lookup"><span data-stu-id="b3f33-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="b3f33-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="b3f33-207">proxySetting</span></span>|[<span data-ttu-id="b3f33-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="b3f33-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="b3f33-209">Укажите параметр прокси для Wi-Fi конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b3f33-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="b3f33-210">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="b3f33-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="b3f33-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="b3f33-211">proxyManualAddress</span></span>|<span data-ttu-id="b3f33-212">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-212">String</span></span>|<span data-ttu-id="b3f33-213">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="b3f33-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="b3f33-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="b3f33-214">proxyManualPort</span></span>|<span data-ttu-id="b3f33-215">Int32</span><span class="sxs-lookup"><span data-stu-id="b3f33-215">Int32</span></span>|<span data-ttu-id="b3f33-216">Укажите порт для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="b3f33-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="b3f33-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b3f33-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b3f33-218">Строка</span><span class="sxs-lookup"><span data-stu-id="b3f33-218">String</span></span>|<span data-ttu-id="b3f33-219">Укажите URL-адрес сценария конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="b3f33-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="b3f33-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="b3f33-220">forceFIPSCompliance</span></span>|<span data-ttu-id="b3f33-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f33-221">Boolean</span></span>|<span data-ttu-id="b3f33-222">Укажите, следует ли принудительно принудить к соблюдению FIPS.</span><span class="sxs-lookup"><span data-stu-id="b3f33-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="b3f33-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3f33-223">Response</span></span>
<span data-ttu-id="b3f33-224">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b3f33-224">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3f33-225">Пример</span><span class="sxs-lookup"><span data-stu-id="b3f33-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3f33-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3f33-226">Request</span></span>
<span data-ttu-id="b3f33-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3f33-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="b3f33-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3f33-228">Response</span></span>
<span data-ttu-id="b3f33-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3f33-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1731

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```




