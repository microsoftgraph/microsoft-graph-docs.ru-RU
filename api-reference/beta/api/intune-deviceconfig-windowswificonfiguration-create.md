---
title: Создание windowsWifiConfiguration
description: Создайте новый объект WindowsWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82b784c82d66c684ac0afac32e9bf490fc26aaaf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131038"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="3dac7-103">Создание windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dac7-103">Create windowsWifiConfiguration</span></span>

<span data-ttu-id="3dac7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dac7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3dac7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dac7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dac7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3dac7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dac7-107">Создайте [новый объект WindowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dac7-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dac7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3dac7-108">Prerequisites</span></span>
<span data-ttu-id="3dac7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dac7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dac7-111">Permission type</span></span>|<span data-ttu-id="3dac7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dac7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dac7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dac7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3dac7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dac7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3dac7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dac7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dac7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dac7-116">Not supported.</span></span>|
|<span data-ttu-id="3dac7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3dac7-117">Application</span></span>|<span data-ttu-id="3dac7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dac7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dac7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dac7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3dac7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3dac7-120">Request headers</span></span>
|<span data-ttu-id="3dac7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3dac7-121">Header</span></span>|<span data-ttu-id="3dac7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3dac7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dac7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dac7-123">Authorization</span></span>|<span data-ttu-id="3dac7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dac7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dac7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3dac7-125">Accept</span></span>|<span data-ttu-id="3dac7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dac7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dac7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3dac7-127">Request body</span></span>
<span data-ttu-id="3dac7-128">В теле запроса устрой представление JSON для объекта WindowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3dac7-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="3dac7-129">В следующей таблице показаны свойства, необходимые при создании windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3dac7-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="3dac7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dac7-130">Property</span></span>|<span data-ttu-id="3dac7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3dac7-131">Type</span></span>|<span data-ttu-id="3dac7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3dac7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dac7-133">id</span><span class="sxs-lookup"><span data-stu-id="3dac7-133">id</span></span>|<span data-ttu-id="3dac7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-134">String</span></span>|<span data-ttu-id="3dac7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3dac7-135">Key of the entity.</span></span> <span data-ttu-id="3dac7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dac7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3dac7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dac7-138">DateTimeOffset</span></span>|<span data-ttu-id="3dac7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3dac7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3dac7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3dac7-141">roleScopeTagIds</span></span>|<span data-ttu-id="3dac7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3dac7-142">String collection</span></span>|<span data-ttu-id="3dac7-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3dac7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3dac7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3dac7-145">supportsScopeTags</span></span>|<span data-ttu-id="3dac7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dac7-146">Boolean</span></span>|<span data-ttu-id="3dac7-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3dac7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3dac7-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3dac7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3dac7-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3dac7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3dac7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3dac7-150">This property is read-only.</span></span> <span data-ttu-id="3dac7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3dac7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3dac7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3dac7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3dac7-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3dac7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3dac7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3dac7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3dac7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3dac7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3dac7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3dac7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3dac7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3dac7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3dac7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3dac7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3dac7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3dac7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3dac7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dac7-164">createdDateTime</span></span>|<span data-ttu-id="3dac7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dac7-165">DateTimeOffset</span></span>|<span data-ttu-id="3dac7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3dac7-166">DateTime the object was created.</span></span> <span data-ttu-id="3dac7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-168">description</span><span class="sxs-lookup"><span data-stu-id="3dac7-168">description</span></span>|<span data-ttu-id="3dac7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-169">String</span></span>|<span data-ttu-id="3dac7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3dac7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3dac7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3dac7-172">displayName</span></span>|<span data-ttu-id="3dac7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-173">String</span></span>|<span data-ttu-id="3dac7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3dac7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3dac7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-176">version</span><span class="sxs-lookup"><span data-stu-id="3dac7-176">version</span></span>|<span data-ttu-id="3dac7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3dac7-177">Int32</span></span>|<span data-ttu-id="3dac7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3dac7-178">Version of the device configuration.</span></span> <span data-ttu-id="3dac7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dac7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dac7-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="3dac7-180">preSharedKey</span></span>|<span data-ttu-id="3dac7-181">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-181">String</span></span>|<span data-ttu-id="3dac7-182">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="3dac7-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="3dac7-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3dac7-183">wifiSecurityType</span></span>|[<span data-ttu-id="3dac7-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3dac7-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="3dac7-185">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3dac7-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="3dac7-186">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="3dac7-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="3dac7-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="3dac7-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="3dac7-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="3dac7-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="3dac7-189">Укажите тип ограничения дозы подключения для подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3dac7-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="3dac7-190">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="3dac7-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="3dac7-191">ssid</span><span class="sxs-lookup"><span data-stu-id="3dac7-191">ssid</span></span>|<span data-ttu-id="3dac7-192">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-192">String</span></span>|<span data-ttu-id="3dac7-193">Укажите SSID подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3dac7-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="3dac7-194">networkName</span><span class="sxs-lookup"><span data-stu-id="3dac7-194">networkName</span></span>|<span data-ttu-id="3dac7-195">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-195">String</span></span>|<span data-ttu-id="3dac7-196">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="3dac7-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="3dac7-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3dac7-197">connectAutomatically</span></span>|<span data-ttu-id="3dac7-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dac7-198">Boolean</span></span>|<span data-ttu-id="3dac7-199">Укажите, должно ли подключение Wi-Fi подключаться автоматически при диапазоне.</span><span class="sxs-lookup"><span data-stu-id="3dac7-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="3dac7-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="3dac7-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="3dac7-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dac7-201">Boolean</span></span>|<span data-ttu-id="3dac7-202">Укажите, должно ли подключение Wi-Fi подключаться к более предпочтительным сетям при уже подключении к этой.</span><span class="sxs-lookup"><span data-stu-id="3dac7-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="3dac7-203">Требуется, чтобы ConnectAutomatically был правдивым.</span><span class="sxs-lookup"><span data-stu-id="3dac7-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="3dac7-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3dac7-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3dac7-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dac7-205">Boolean</span></span>|<span data-ttu-id="3dac7-206">Укажите, следует ли подключать подключение к Wi-Fi автоматически, даже если SSID не транслируется.</span><span class="sxs-lookup"><span data-stu-id="3dac7-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="3dac7-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="3dac7-207">proxySetting</span></span>|[<span data-ttu-id="3dac7-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="3dac7-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="3dac7-209">Укажите параметр прокси для Wi-Fi конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3dac7-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="3dac7-210">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="3dac7-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="3dac7-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="3dac7-211">proxyManualAddress</span></span>|<span data-ttu-id="3dac7-212">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-212">String</span></span>|<span data-ttu-id="3dac7-213">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="3dac7-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="3dac7-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="3dac7-214">proxyManualPort</span></span>|<span data-ttu-id="3dac7-215">Int32</span><span class="sxs-lookup"><span data-stu-id="3dac7-215">Int32</span></span>|<span data-ttu-id="3dac7-216">Укажите порт для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="3dac7-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="3dac7-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="3dac7-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="3dac7-218">Строка</span><span class="sxs-lookup"><span data-stu-id="3dac7-218">String</span></span>|<span data-ttu-id="3dac7-219">Укажите URL-адрес сценария конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="3dac7-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="3dac7-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="3dac7-220">forceFIPSCompliance</span></span>|<span data-ttu-id="3dac7-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dac7-221">Boolean</span></span>|<span data-ttu-id="3dac7-222">Укажите, следует ли принудительно принудить к соблюдению FIPS.</span><span class="sxs-lookup"><span data-stu-id="3dac7-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="3dac7-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dac7-223">Response</span></span>
<span data-ttu-id="3dac7-224">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3dac7-224">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dac7-225">Пример</span><span class="sxs-lookup"><span data-stu-id="3dac7-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dac7-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dac7-226">Request</span></span>
<span data-ttu-id="3dac7-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3dac7-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3dac7-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dac7-228">Response</span></span>
<span data-ttu-id="3dac7-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3dac7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




