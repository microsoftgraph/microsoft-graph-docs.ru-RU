---
title: Создание macOSWiFiConfiguration
description: Создайте новый объект macOSWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9d552fbc6c4d1d5a96309817482f2fca98ae983
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129673"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="71e43-103">Создание macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="71e43-103">Create macOSWiFiConfiguration</span></span>

<span data-ttu-id="71e43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71e43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71e43-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71e43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71e43-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71e43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71e43-107">Создайте [новый объект macOSWiFiConfiguration.](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71e43-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71e43-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71e43-108">Prerequisites</span></span>
<span data-ttu-id="71e43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71e43-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71e43-111">Permission type</span></span>|<span data-ttu-id="71e43-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71e43-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71e43-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71e43-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71e43-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71e43-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71e43-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71e43-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71e43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71e43-116">Not supported.</span></span>|
|<span data-ttu-id="71e43-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="71e43-117">Application</span></span>|<span data-ttu-id="71e43-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71e43-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71e43-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71e43-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71e43-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71e43-120">Request headers</span></span>
|<span data-ttu-id="71e43-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71e43-121">Header</span></span>|<span data-ttu-id="71e43-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71e43-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71e43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71e43-123">Authorization</span></span>|<span data-ttu-id="71e43-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71e43-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71e43-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71e43-125">Accept</span></span>|<span data-ttu-id="71e43-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71e43-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71e43-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71e43-127">Request body</span></span>
<span data-ttu-id="71e43-128">В теле запроса поставляем представление JSON для объекта macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="71e43-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="71e43-129">В следующей таблице показаны свойства, необходимые при создании macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="71e43-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="71e43-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71e43-130">Property</span></span>|<span data-ttu-id="71e43-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71e43-131">Type</span></span>|<span data-ttu-id="71e43-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71e43-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71e43-133">id</span><span class="sxs-lookup"><span data-stu-id="71e43-133">id</span></span>|<span data-ttu-id="71e43-134">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-134">String</span></span>|<span data-ttu-id="71e43-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71e43-135">Key of the entity.</span></span> <span data-ttu-id="71e43-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71e43-137">lastModifiedDateTime</span></span>|<span data-ttu-id="71e43-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71e43-138">DateTimeOffset</span></span>|<span data-ttu-id="71e43-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="71e43-139">DateTime the object was last modified.</span></span> <span data-ttu-id="71e43-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71e43-141">roleScopeTagIds</span></span>|<span data-ttu-id="71e43-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71e43-142">String collection</span></span>|<span data-ttu-id="71e43-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="71e43-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71e43-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71e43-145">supportsScopeTags</span></span>|<span data-ttu-id="71e43-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="71e43-146">Boolean</span></span>|<span data-ttu-id="71e43-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="71e43-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71e43-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="71e43-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71e43-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="71e43-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71e43-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71e43-150">This property is read-only.</span></span> <span data-ttu-id="71e43-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71e43-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="71e43-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71e43-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="71e43-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="71e43-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="71e43-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71e43-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="71e43-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71e43-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="71e43-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="71e43-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="71e43-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71e43-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="71e43-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71e43-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="71e43-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="71e43-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="71e43-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71e43-164">createdDateTime</span></span>|<span data-ttu-id="71e43-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71e43-165">DateTimeOffset</span></span>|<span data-ttu-id="71e43-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="71e43-166">DateTime the object was created.</span></span> <span data-ttu-id="71e43-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-168">description</span><span class="sxs-lookup"><span data-stu-id="71e43-168">description</span></span>|<span data-ttu-id="71e43-169">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-169">String</span></span>|<span data-ttu-id="71e43-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71e43-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71e43-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-172">displayName</span><span class="sxs-lookup"><span data-stu-id="71e43-172">displayName</span></span>|<span data-ttu-id="71e43-173">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-173">String</span></span>|<span data-ttu-id="71e43-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71e43-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71e43-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-176">version</span><span class="sxs-lookup"><span data-stu-id="71e43-176">version</span></span>|<span data-ttu-id="71e43-177">Int32</span><span class="sxs-lookup"><span data-stu-id="71e43-177">Int32</span></span>|<span data-ttu-id="71e43-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71e43-178">Version of the device configuration.</span></span> <span data-ttu-id="71e43-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71e43-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71e43-180">networkName</span><span class="sxs-lookup"><span data-stu-id="71e43-180">networkName</span></span>|<span data-ttu-id="71e43-181">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-181">String</span></span>|<span data-ttu-id="71e43-182">Имя сети</span><span class="sxs-lookup"><span data-stu-id="71e43-182">Network Name</span></span>|
|<span data-ttu-id="71e43-183">ssid</span><span class="sxs-lookup"><span data-stu-id="71e43-183">ssid</span></span>|<span data-ttu-id="71e43-184">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-184">String</span></span>|<span data-ttu-id="71e43-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="71e43-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="71e43-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="71e43-186">connectAutomatically</span></span>|<span data-ttu-id="71e43-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="71e43-187">Boolean</span></span>|<span data-ttu-id="71e43-188">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="71e43-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="71e43-189">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="71e43-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="71e43-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="71e43-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="71e43-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="71e43-191">Boolean</span></span>|<span data-ttu-id="71e43-192">Подключение, если сеть не передает свое имя (SSID).</span><span class="sxs-lookup"><span data-stu-id="71e43-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="71e43-193">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="71e43-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="71e43-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="71e43-194">wiFiSecurityType</span></span>|[<span data-ttu-id="71e43-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="71e43-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="71e43-196">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="71e43-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="71e43-197">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="71e43-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="71e43-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="71e43-198">proxySettings</span></span>|[<span data-ttu-id="71e43-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="71e43-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="71e43-200">Тип прокси для Wi-Fi подключения.</span><span class="sxs-lookup"><span data-stu-id="71e43-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="71e43-201">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="71e43-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="71e43-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="71e43-202">proxyManualAddress</span></span>|<span data-ttu-id="71e43-203">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-203">String</span></span>|<span data-ttu-id="71e43-204">IP-адрес или DNS-имя прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="71e43-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="71e43-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="71e43-205">proxyManualPort</span></span>|<span data-ttu-id="71e43-206">Int32</span><span class="sxs-lookup"><span data-stu-id="71e43-206">Int32</span></span>|<span data-ttu-id="71e43-207">Порт прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="71e43-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="71e43-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="71e43-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="71e43-209">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-209">String</span></span>|<span data-ttu-id="71e43-210">URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации.</span><span class="sxs-lookup"><span data-stu-id="71e43-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="71e43-211">Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration).</span><span class="sxs-lookup"><span data-stu-id="71e43-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="71e43-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="71e43-212">preSharedKey</span></span>|<span data-ttu-id="71e43-213">Строка</span><span class="sxs-lookup"><span data-stu-id="71e43-213">String</span></span>|<span data-ttu-id="71e43-214">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="71e43-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="71e43-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e43-215">Response</span></span>
<span data-ttu-id="71e43-216">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71e43-216">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71e43-217">Пример</span><span class="sxs-lookup"><span data-stu-id="71e43-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="71e43-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="71e43-218">Request</span></span>
<span data-ttu-id="71e43-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71e43-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1450

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="71e43-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e43-220">Response</span></span>
<span data-ttu-id="71e43-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71e43-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1622

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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
  "preSharedKey": "Pre Shared Key value"
}
```




