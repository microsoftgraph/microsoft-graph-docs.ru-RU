---
title: Обновление iosWiFiConfiguration
description: Обновление свойств объекта iosWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 12b29ee1d8b3c8fc980ea8e4617daa3c20779493
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151237"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="4e51e-103">Обновление iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e51e-103">Update iosWiFiConfiguration</span></span>

<span data-ttu-id="4e51e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e51e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e51e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e51e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e51e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e51e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e51e-107">Обновление свойств объекта [iosWiFiConfiguration.](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e51e-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e51e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e51e-108">Prerequisites</span></span>
<span data-ttu-id="4e51e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e51e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e51e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e51e-111">Permission type</span></span>|<span data-ttu-id="4e51e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e51e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e51e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e51e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e51e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e51e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e51e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e51e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e51e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e51e-116">Not supported.</span></span>|
|<span data-ttu-id="4e51e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e51e-117">Application</span></span>|<span data-ttu-id="4e51e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e51e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e51e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e51e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4e51e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e51e-120">Request headers</span></span>
|<span data-ttu-id="4e51e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e51e-121">Header</span></span>|<span data-ttu-id="4e51e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e51e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e51e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e51e-123">Authorization</span></span>|<span data-ttu-id="4e51e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e51e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e51e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e51e-125">Accept</span></span>|<span data-ttu-id="4e51e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e51e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e51e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e51e-127">Request body</span></span>
<span data-ttu-id="4e51e-128">В теле запроса поставляем представление JSON для [объекта iosWiFiConfiguration.](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e51e-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="4e51e-129">В следующей таблице показаны свойства, необходимые при создании [iosWiFiConfiguration.](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e51e-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="4e51e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e51e-130">Property</span></span>|<span data-ttu-id="4e51e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e51e-131">Type</span></span>|<span data-ttu-id="4e51e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e51e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e51e-133">id</span><span class="sxs-lookup"><span data-stu-id="4e51e-133">id</span></span>|<span data-ttu-id="4e51e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-134">String</span></span>|<span data-ttu-id="4e51e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e51e-135">Key of the entity.</span></span> <span data-ttu-id="4e51e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e51e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4e51e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e51e-138">DateTimeOffset</span></span>|<span data-ttu-id="4e51e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4e51e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4e51e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e51e-141">roleScopeTagIds</span></span>|<span data-ttu-id="4e51e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4e51e-142">String collection</span></span>|<span data-ttu-id="4e51e-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4e51e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4e51e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4e51e-145">supportsScopeTags</span></span>|<span data-ttu-id="4e51e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e51e-146">Boolean</span></span>|<span data-ttu-id="4e51e-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4e51e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4e51e-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="4e51e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4e51e-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4e51e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4e51e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e51e-150">This property is read-only.</span></span> <span data-ttu-id="4e51e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4e51e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4e51e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4e51e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4e51e-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e51e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4e51e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4e51e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4e51e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4e51e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4e51e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e51e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4e51e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4e51e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4e51e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4e51e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4e51e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e51e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4e51e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e51e-164">createdDateTime</span></span>|<span data-ttu-id="4e51e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e51e-165">DateTimeOffset</span></span>|<span data-ttu-id="4e51e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4e51e-166">DateTime the object was created.</span></span> <span data-ttu-id="4e51e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-168">description</span><span class="sxs-lookup"><span data-stu-id="4e51e-168">description</span></span>|<span data-ttu-id="4e51e-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-169">String</span></span>|<span data-ttu-id="4e51e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e51e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4e51e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4e51e-172">displayName</span></span>|<span data-ttu-id="4e51e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-173">String</span></span>|<span data-ttu-id="4e51e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e51e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4e51e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-176">version</span><span class="sxs-lookup"><span data-stu-id="4e51e-176">version</span></span>|<span data-ttu-id="4e51e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4e51e-177">Int32</span></span>|<span data-ttu-id="4e51e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e51e-178">Version of the device configuration.</span></span> <span data-ttu-id="4e51e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e51e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e51e-180">networkName</span><span class="sxs-lookup"><span data-stu-id="4e51e-180">networkName</span></span>|<span data-ttu-id="4e51e-181">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-181">String</span></span>|<span data-ttu-id="4e51e-182">Имя сети</span><span class="sxs-lookup"><span data-stu-id="4e51e-182">Network Name</span></span>|
|<span data-ttu-id="4e51e-183">ssid</span><span class="sxs-lookup"><span data-stu-id="4e51e-183">ssid</span></span>|<span data-ttu-id="4e51e-184">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-184">String</span></span>|<span data-ttu-id="4e51e-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="4e51e-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="4e51e-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="4e51e-186">connectAutomatically</span></span>|<span data-ttu-id="4e51e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e51e-187">Boolean</span></span>|<span data-ttu-id="4e51e-188">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="4e51e-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="4e51e-189">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="4e51e-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="4e51e-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="4e51e-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="4e51e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e51e-191">Boolean</span></span>|<span data-ttu-id="4e51e-192">Подключение, если сеть не передает свое имя (SSID).</span><span class="sxs-lookup"><span data-stu-id="4e51e-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="4e51e-193">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="4e51e-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="4e51e-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="4e51e-194">wiFiSecurityType</span></span>|[<span data-ttu-id="4e51e-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="4e51e-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="4e51e-196">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="4e51e-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="4e51e-197">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="4e51e-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="4e51e-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="4e51e-198">proxySettings</span></span>|[<span data-ttu-id="4e51e-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="4e51e-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="4e51e-200">Тип прокси для Wi-Fi подключения.</span><span class="sxs-lookup"><span data-stu-id="4e51e-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="4e51e-201">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4e51e-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="4e51e-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="4e51e-202">proxyManualAddress</span></span>|<span data-ttu-id="4e51e-203">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-203">String</span></span>|<span data-ttu-id="4e51e-204">IP-адрес или DNS-имя прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4e51e-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="4e51e-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="4e51e-205">proxyManualPort</span></span>|<span data-ttu-id="4e51e-206">Int32</span><span class="sxs-lookup"><span data-stu-id="4e51e-206">Int32</span></span>|<span data-ttu-id="4e51e-207">Порт прокси-сервера при выборе ручной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4e51e-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="4e51e-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="4e51e-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="4e51e-209">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-209">String</span></span>|<span data-ttu-id="4e51e-210">URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4e51e-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="4e51e-211">Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration).</span><span class="sxs-lookup"><span data-stu-id="4e51e-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="4e51e-212">отключениеMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="4e51e-212">disableMacAddressRandomization</span></span>|<span data-ttu-id="4e51e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e51e-213">Boolean</span></span>|<span data-ttu-id="4e51e-214">Если установлено истинное, устройства, подключающиеся с помощью этого Wi-Fi профиля, должны представить Wi-Fi mac-адрес, а не случайный MAC-адрес.</span><span class="sxs-lookup"><span data-stu-id="4e51e-214">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="4e51e-215">Применяется к iOS 14 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="4e51e-215">Applies to iOS 14 and later.</span></span>|
|<span data-ttu-id="4e51e-216">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="4e51e-216">preSharedKey</span></span>|<span data-ttu-id="4e51e-217">Строка</span><span class="sxs-lookup"><span data-stu-id="4e51e-217">String</span></span>|<span data-ttu-id="4e51e-218">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="4e51e-218">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="4e51e-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e51e-219">Response</span></span>
<span data-ttu-id="4e51e-220">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4e51e-220">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e51e-221">Пример</span><span class="sxs-lookup"><span data-stu-id="4e51e-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e51e-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e51e-222">Request</span></span>
<span data-ttu-id="4e51e-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e51e-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="4e51e-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e51e-224">Response</span></span>
<span data-ttu-id="4e51e-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e51e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "preSharedKey": "Pre Shared Key value"
}
```




