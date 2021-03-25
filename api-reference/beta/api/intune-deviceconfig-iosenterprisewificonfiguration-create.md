---
title: Создание iosEnterpriseWiFiConfiguration
description: Создайте новый объект iosEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79df6dba6a4058b66f97bb95f74feb88a1a2e7b4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151335"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="77ca9-103">Создание iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="77ca9-103">Create iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="77ca9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77ca9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77ca9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77ca9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77ca9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77ca9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77ca9-107">Создайте новый [объект iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77ca9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77ca9-108">Prerequisites</span></span>
<span data-ttu-id="77ca9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77ca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77ca9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77ca9-111">Permission type</span></span>|<span data-ttu-id="77ca9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77ca9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77ca9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77ca9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77ca9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77ca9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77ca9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77ca9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77ca9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77ca9-116">Not supported.</span></span>|
|<span data-ttu-id="77ca9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77ca9-117">Application</span></span>|<span data-ttu-id="77ca9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77ca9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77ca9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77ca9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77ca9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77ca9-120">Request headers</span></span>
|<span data-ttu-id="77ca9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77ca9-121">Header</span></span>|<span data-ttu-id="77ca9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77ca9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77ca9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77ca9-123">Authorization</span></span>|<span data-ttu-id="77ca9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77ca9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77ca9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77ca9-125">Accept</span></span>|<span data-ttu-id="77ca9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77ca9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77ca9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77ca9-127">Request body</span></span>
<span data-ttu-id="77ca9-128">В теле запроса поставляем представление JSON для объекта iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="77ca9-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="77ca9-129">В следующей таблице показаны свойства, необходимые при создании iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="77ca9-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="77ca9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77ca9-130">Property</span></span>|<span data-ttu-id="77ca9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77ca9-131">Type</span></span>|<span data-ttu-id="77ca9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77ca9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77ca9-133">id</span><span class="sxs-lookup"><span data-stu-id="77ca9-133">id</span></span>|<span data-ttu-id="77ca9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-134">String</span></span>|<span data-ttu-id="77ca9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77ca9-135">Key of the entity.</span></span> <span data-ttu-id="77ca9-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77ca9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="77ca9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ca9-138">DateTimeOffset</span></span>|<span data-ttu-id="77ca9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="77ca9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="77ca9-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77ca9-141">roleScopeTagIds</span></span>|<span data-ttu-id="77ca9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77ca9-142">String collection</span></span>|<span data-ttu-id="77ca9-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="77ca9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77ca9-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77ca9-145">supportsScopeTags</span></span>|<span data-ttu-id="77ca9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="77ca9-146">Boolean</span></span>|<span data-ttu-id="77ca9-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="77ca9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77ca9-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="77ca9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77ca9-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="77ca9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77ca9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77ca9-150">This property is read-only.</span></span> <span data-ttu-id="77ca9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77ca9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="77ca9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77ca9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="77ca9-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77ca9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="77ca9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77ca9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="77ca9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77ca9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="77ca9-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77ca9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="77ca9-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="77ca9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="77ca9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="77ca9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="77ca9-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77ca9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="77ca9-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77ca9-164">createdDateTime</span></span>|<span data-ttu-id="77ca9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ca9-165">DateTimeOffset</span></span>|<span data-ttu-id="77ca9-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="77ca9-166">DateTime the object was created.</span></span> <span data-ttu-id="77ca9-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-168">description</span><span class="sxs-lookup"><span data-stu-id="77ca9-168">description</span></span>|<span data-ttu-id="77ca9-169">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-169">String</span></span>|<span data-ttu-id="77ca9-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77ca9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77ca9-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="77ca9-172">displayName</span></span>|<span data-ttu-id="77ca9-173">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-173">String</span></span>|<span data-ttu-id="77ca9-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77ca9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77ca9-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-176">version</span><span class="sxs-lookup"><span data-stu-id="77ca9-176">version</span></span>|<span data-ttu-id="77ca9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="77ca9-177">Int32</span></span>|<span data-ttu-id="77ca9-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77ca9-178">Version of the device configuration.</span></span> <span data-ttu-id="77ca9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-180">networkName</span><span class="sxs-lookup"><span data-stu-id="77ca9-180">networkName</span></span>|<span data-ttu-id="77ca9-181">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-181">String</span></span>|<span data-ttu-id="77ca9-182">Имя сети, унаследованные от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-183">ssid</span><span class="sxs-lookup"><span data-stu-id="77ca9-183">ssid</span></span>|<span data-ttu-id="77ca9-184">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-184">String</span></span>|<span data-ttu-id="77ca9-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="77ca9-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="77ca9-186">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="77ca9-187">connectAutomatically</span></span>|<span data-ttu-id="77ca9-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="77ca9-188">Boolean</span></span>|<span data-ttu-id="77ca9-189">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="77ca9-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="77ca9-190">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="77ca9-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="77ca9-191">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="77ca9-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="77ca9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="77ca9-193">Boolean</span></span>|<span data-ttu-id="77ca9-194">Подключение, если сеть не передает свое имя (SSID).</span><span class="sxs-lookup"><span data-stu-id="77ca9-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="77ca9-195">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="77ca9-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="77ca9-196">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="77ca9-197">wiFiSecurityType</span></span>|[<span data-ttu-id="77ca9-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="77ca9-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="77ca9-199">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="77ca9-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="77ca9-200">Наследуется [от iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77ca9-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="77ca9-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="77ca9-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="77ca9-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="77ca9-202">proxySettings</span></span>|[<span data-ttu-id="77ca9-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="77ca9-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="77ca9-204">Тип прокси для этого Wi-Fi, унаследованный от [iosWiFiConfiguration.](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="77ca9-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="77ca9-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="77ca9-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="77ca9-206">proxyManualAddress</span></span>|<span data-ttu-id="77ca9-207">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-207">String</span></span>|<span data-ttu-id="77ca9-208">IP-адрес или DNS-имя прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="77ca9-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="77ca9-209">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="77ca9-210">proxyManualPort</span></span>|<span data-ttu-id="77ca9-211">Int32</span><span class="sxs-lookup"><span data-stu-id="77ca9-211">Int32</span></span>|<span data-ttu-id="77ca9-212">Порт прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="77ca9-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="77ca9-213">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="77ca9-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="77ca9-215">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-215">String</span></span>|<span data-ttu-id="77ca9-216">URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации.</span><span class="sxs-lookup"><span data-stu-id="77ca9-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="77ca9-217">Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration).</span><span class="sxs-lookup"><span data-stu-id="77ca9-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="77ca9-218">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-219">отключениеMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="77ca9-219">disableMacAddressRandomization</span></span>|<span data-ttu-id="77ca9-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="77ca9-220">Boolean</span></span>|<span data-ttu-id="77ca9-221">Если установлено истинное, устройства, подключающиеся с помощью этого Wi-Fi профиля, должны представить Wi-Fi mac-адрес, а не случайный MAC-адрес.</span><span class="sxs-lookup"><span data-stu-id="77ca9-221">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="77ca9-222">Применяется к iOS 14 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="77ca9-222">Applies to iOS 14 and later.</span></span> <span data-ttu-id="77ca9-223">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-223">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-224">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="77ca9-224">preSharedKey</span></span>|<span data-ttu-id="77ca9-225">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-225">String</span></span>|<span data-ttu-id="77ca9-226">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="77ca9-226">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="77ca9-227">Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77ca9-227">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="77ca9-228">eapType</span><span class="sxs-lookup"><span data-stu-id="77ca9-228">eapType</span></span>|[<span data-ttu-id="77ca9-229">eapType</span><span class="sxs-lookup"><span data-stu-id="77ca9-229">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="77ca9-230">Extensible Authentication Protocol (EAP).</span><span class="sxs-lookup"><span data-stu-id="77ca9-230">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="77ca9-231">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="77ca9-231">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="77ca9-232">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="77ca9-232">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="77ca9-233">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="77ca9-233">eapFastConfiguration</span></span>|[<span data-ttu-id="77ca9-234">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="77ca9-234">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="77ca9-235">Параметр конфигурации EAP-FAST, когда EAP-FAST является выбранным типом EAP.</span><span class="sxs-lookup"><span data-stu-id="77ca9-235">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="77ca9-236">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="77ca9-236">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="77ca9-237">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="77ca9-237">trustedServerCertificateNames</span></span>|<span data-ttu-id="77ca9-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77ca9-238">String collection</span></span>|<span data-ttu-id="77ca9-239">Доверенные имена сертификатов сервера при настройке типа EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="77ca9-239">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="77ca9-240">Это общее имя, используемая в сертификатах, выдаванных доверенным органом сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="77ca9-240">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="77ca9-241">Если вы предоставите эту информацию, можно обойти динамический диалог доверия, отображаемый на устройствах конечных пользователей при подключении к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="77ca9-241">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="77ca9-242">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77ca9-242">authenticationMethod</span></span>|[<span data-ttu-id="77ca9-243">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77ca9-243">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="77ca9-244">Метод проверки подлинности при настройке типа EAP на PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="77ca9-244">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="77ca9-245">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="77ca9-245">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="77ca9-246">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="77ca9-246">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="77ca9-247">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="77ca9-247">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="77ca9-248">Метод без EAP для проверки подлинности, если тип EAP — EAP-TTLS, а проверка подлинности — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="77ca9-248">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="77ca9-249">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="77ca9-249">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="77ca9-250">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="77ca9-250">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="77ca9-251">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-251">String</span></span>|<span data-ttu-id="77ca9-252">Включить конфиденциальность удостоверений (внешний идентификатор), когда тип EAP настроен на EAP - TTLS, EAP - FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="77ca9-252">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="77ca9-253">Это свойство маскирует имена пользователей с вводимым текстом.</span><span class="sxs-lookup"><span data-stu-id="77ca9-253">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="77ca9-254">Например, если используется "анонимный", каждый пользователь, который Wi-Fi с этим подключением, используя свое реальное имя пользователя, отображается как "анонимный".</span><span class="sxs-lookup"><span data-stu-id="77ca9-254">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="77ca9-255">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="77ca9-255">usernameFormatString</span></span>|<span data-ttu-id="77ca9-256">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-256">String</span></span>|<span data-ttu-id="77ca9-257">Строка формата username, используемая для создания имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="77ca9-257">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="77ca9-258">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="77ca9-258">passwordFormatString</span></span>|<span data-ttu-id="77ca9-259">Строка</span><span class="sxs-lookup"><span data-stu-id="77ca9-259">String</span></span>|<span data-ttu-id="77ca9-260">Строка формата пароля, используемая для создания пароля для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="77ca9-260">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="77ca9-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="77ca9-261">Response</span></span>
<span data-ttu-id="77ca9-262">В случае успеха этот метод возвращает код отклика и `201 Created` [объект iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="77ca9-262">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77ca9-263">Пример</span><span class="sxs-lookup"><span data-stu-id="77ca9-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="77ca9-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="77ca9-264">Request</span></span>
<span data-ttu-id="77ca9-265">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77ca9-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="77ca9-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="77ca9-266">Response</span></span>
<span data-ttu-id="77ca9-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77ca9-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




