---
title: Создание macOSEnterpriseWiFiConfiguration
description: Создайте новый объект macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e02ac502f22ad8bcc649d77383827739c1a5aed4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131311"
---
# <a name="create-macosenterprisewificonfiguration"></a><span data-ttu-id="d4a99-103">Создание macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4a99-103">Create macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="d4a99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4a99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4a99-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4a99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4a99-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4a99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4a99-107">Создайте [новый объект macOSEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-107">Create a new [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4a99-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4a99-108">Prerequisites</span></span>
<span data-ttu-id="d4a99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4a99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4a99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4a99-111">Permission type</span></span>|<span data-ttu-id="d4a99-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4a99-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4a99-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4a99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4a99-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a99-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4a99-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4a99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4a99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4a99-116">Not supported.</span></span>|
|<span data-ttu-id="d4a99-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4a99-117">Application</span></span>|<span data-ttu-id="d4a99-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a99-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4a99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4a99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d4a99-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4a99-120">Request headers</span></span>
|<span data-ttu-id="d4a99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4a99-121">Header</span></span>|<span data-ttu-id="d4a99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4a99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4a99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4a99-123">Authorization</span></span>|<span data-ttu-id="d4a99-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4a99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4a99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4a99-125">Accept</span></span>|<span data-ttu-id="d4a99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4a99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4a99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4a99-127">Request body</span></span>
<span data-ttu-id="d4a99-128">В теле запроса поставляем представление JSON для объекта macOSEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4a99-128">In the request body, supply a JSON representation for the macOSEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="d4a99-129">В следующей таблице показаны свойства, необходимые при создании macOSEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4a99-129">The following table shows the properties that are required when you create the macOSEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="d4a99-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4a99-130">Property</span></span>|<span data-ttu-id="d4a99-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4a99-131">Type</span></span>|<span data-ttu-id="d4a99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4a99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4a99-133">id</span><span class="sxs-lookup"><span data-stu-id="d4a99-133">id</span></span>|<span data-ttu-id="d4a99-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-134">String</span></span>|<span data-ttu-id="d4a99-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4a99-135">Key of the entity.</span></span> <span data-ttu-id="d4a99-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4a99-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d4a99-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4a99-138">DateTimeOffset</span></span>|<span data-ttu-id="d4a99-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d4a99-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d4a99-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4a99-141">roleScopeTagIds</span></span>|<span data-ttu-id="d4a99-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d4a99-142">String collection</span></span>|<span data-ttu-id="d4a99-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="d4a99-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4a99-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4a99-145">supportsScopeTags</span></span>|<span data-ttu-id="d4a99-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4a99-146">Boolean</span></span>|<span data-ttu-id="d4a99-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d4a99-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4a99-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="d4a99-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4a99-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d4a99-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4a99-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4a99-150">This property is read-only.</span></span> <span data-ttu-id="d4a99-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4a99-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d4a99-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4a99-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d4a99-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d4a99-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d4a99-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4a99-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d4a99-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4a99-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d4a99-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d4a99-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d4a99-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d4a99-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d4a99-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d4a99-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d4a99-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d4a99-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d4a99-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4a99-164">createdDateTime</span></span>|<span data-ttu-id="d4a99-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4a99-165">DateTimeOffset</span></span>|<span data-ttu-id="d4a99-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d4a99-166">DateTime the object was created.</span></span> <span data-ttu-id="d4a99-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-168">description</span><span class="sxs-lookup"><span data-stu-id="d4a99-168">description</span></span>|<span data-ttu-id="d4a99-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-169">String</span></span>|<span data-ttu-id="d4a99-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4a99-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4a99-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d4a99-172">displayName</span></span>|<span data-ttu-id="d4a99-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-173">String</span></span>|<span data-ttu-id="d4a99-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4a99-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4a99-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-176">version</span><span class="sxs-lookup"><span data-stu-id="d4a99-176">version</span></span>|<span data-ttu-id="d4a99-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d4a99-177">Int32</span></span>|<span data-ttu-id="d4a99-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4a99-178">Version of the device configuration.</span></span> <span data-ttu-id="d4a99-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-180">networkName</span><span class="sxs-lookup"><span data-stu-id="d4a99-180">networkName</span></span>|<span data-ttu-id="d4a99-181">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-181">String</span></span>|<span data-ttu-id="d4a99-182">Имя сети, унаследованные от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-182">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-183">ssid</span><span class="sxs-lookup"><span data-stu-id="d4a99-183">ssid</span></span>|<span data-ttu-id="d4a99-184">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-184">String</span></span>|<span data-ttu-id="d4a99-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="d4a99-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="d4a99-186">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-186">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="d4a99-187">connectAutomatically</span></span>|<span data-ttu-id="d4a99-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4a99-188">Boolean</span></span>|<span data-ttu-id="d4a99-189">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="d4a99-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="d4a99-190">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="d4a99-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="d4a99-191">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-191">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d4a99-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d4a99-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4a99-193">Boolean</span></span>|<span data-ttu-id="d4a99-194">Подключение, если сеть не передает свое имя (SSID).</span><span class="sxs-lookup"><span data-stu-id="d4a99-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="d4a99-195">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="d4a99-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="d4a99-196">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-196">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d4a99-197">wiFiSecurityType</span></span>|[<span data-ttu-id="d4a99-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d4a99-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="d4a99-199">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="d4a99-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="d4a99-200">Унаследовано от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4a99-200">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="d4a99-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="d4a99-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="d4a99-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="d4a99-202">proxySettings</span></span>|[<span data-ttu-id="d4a99-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="d4a99-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="d4a99-204">Тип прокси для этого Wi-Fi, унаследованный от [macOSWiFiConfiguration.](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-204">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="d4a99-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="d4a99-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="d4a99-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="d4a99-206">proxyManualAddress</span></span>|<span data-ttu-id="d4a99-207">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-207">String</span></span>|<span data-ttu-id="d4a99-208">IP-адрес или DNS-имя прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="d4a99-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="d4a99-209">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-209">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="d4a99-210">proxyManualPort</span></span>|<span data-ttu-id="d4a99-211">Int32</span><span class="sxs-lookup"><span data-stu-id="d4a99-211">Int32</span></span>|<span data-ttu-id="d4a99-212">Порт прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="d4a99-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="d4a99-213">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-213">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="d4a99-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="d4a99-215">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-215">String</span></span>|<span data-ttu-id="d4a99-216">URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации.</span><span class="sxs-lookup"><span data-stu-id="d4a99-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="d4a99-217">Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration).</span><span class="sxs-lookup"><span data-stu-id="d4a99-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="d4a99-218">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-218">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="d4a99-219">preSharedKey</span></span>|<span data-ttu-id="d4a99-220">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-220">String</span></span>|<span data-ttu-id="d4a99-221">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="d4a99-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="d4a99-222">Унаследованный от [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4a99-222">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="d4a99-223">eapType</span><span class="sxs-lookup"><span data-stu-id="d4a99-223">eapType</span></span>|[<span data-ttu-id="d4a99-224">eapType</span><span class="sxs-lookup"><span data-stu-id="d4a99-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="d4a99-225">Extensible Authentication Protocol (EAP).</span><span class="sxs-lookup"><span data-stu-id="d4a99-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="d4a99-226">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="d4a99-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="d4a99-227">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="d4a99-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="d4a99-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4a99-228">eapFastConfiguration</span></span>|[<span data-ttu-id="d4a99-229">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4a99-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="d4a99-230">Параметр конфигурации EAP-FAST, когда EAP-FAST является выбранным типом EAP.</span><span class="sxs-lookup"><span data-stu-id="d4a99-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="d4a99-231">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="d4a99-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="d4a99-232">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="d4a99-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="d4a99-233">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d4a99-233">String collection</span></span>|<span data-ttu-id="d4a99-234">Доверенные имена сертификатов сервера при настройке типа EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="d4a99-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="d4a99-235">Это общее имя, используемая в сертификатах, выдаванных доверенным органом сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="d4a99-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="d4a99-236">При предоставлении этих сведений можно обойти динамический диалог доверия, отображаемый на устройствах конечных пользователей при подключении к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="d4a99-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="d4a99-237">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d4a99-237">authenticationMethod</span></span>|[<span data-ttu-id="d4a99-238">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d4a99-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="d4a99-239">Метод проверки подлинности при настройке типа EAP на PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="d4a99-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="d4a99-240">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d4a99-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d4a99-241">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="d4a99-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="d4a99-242">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="d4a99-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="d4a99-243">Метод без EAP для проверки подлинности (внутренняя идентичность), когда тип EAP EAP-TTLS и authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="d4a99-243">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="d4a99-244">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="d4a99-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="d4a99-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="d4a99-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="d4a99-246">Строка</span><span class="sxs-lookup"><span data-stu-id="d4a99-246">String</span></span>|<span data-ttu-id="d4a99-247">Введите конфиденциальность удостоверений (внешний идентификатор), если тип EAP настроен на EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="d4a99-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="d4a99-248">Это свойство маскирует имена пользователей с вводимым текстом.</span><span class="sxs-lookup"><span data-stu-id="d4a99-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="d4a99-249">Например, если используется "анонимный", каждый пользователь, который Wi-Fi с этим подключением, используя свое реальное имя пользователя, отображается как "анонимный".</span><span class="sxs-lookup"><span data-stu-id="d4a99-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="d4a99-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4a99-250">Response</span></span>
<span data-ttu-id="d4a99-251">В случае успеха этот метод возвращает код отклика и `201 Created` [объект macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d4a99-251">If successful, this method returns a `201 Created` response code and a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4a99-252">Пример</span><span class="sxs-lookup"><span data-stu-id="d4a99-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4a99-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4a99-253">Request</span></span>
<span data-ttu-id="d4a99-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4a99-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1858

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="d4a99-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4a99-255">Response</span></span>
<span data-ttu-id="d4a99-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4a99-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2030

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




