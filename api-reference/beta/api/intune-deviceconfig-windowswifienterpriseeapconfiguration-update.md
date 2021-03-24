---
title: Обновление windowsWifiEnterpriseEAPConfiguration
description: Обновление свойств объекта WindowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a6c89823f9b66a793302fd6d787ec369b4732fd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136904"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="5b1b7-103">Обновление windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b1b7-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="5b1b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b1b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b1b7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b1b7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b1b7-107">Обновление свойств объекта [WindowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b1b7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b1b7-108">Prerequisites</span></span>
<span data-ttu-id="5b1b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b1b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b1b7-111">Permission type</span></span>|<span data-ttu-id="5b1b7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b1b7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b1b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b1b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b1b7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b1b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-116">Not supported.</span></span>|
|<span data-ttu-id="5b1b7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b1b7-117">Application</span></span>|<span data-ttu-id="5b1b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b1b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b1b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b1b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b1b7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b1b7-120">Request headers</span></span>
|<span data-ttu-id="5b1b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b1b7-121">Header</span></span>|<span data-ttu-id="5b1b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b1b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b1b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b1b7-123">Authorization</span></span>|<span data-ttu-id="5b1b7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b1b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b1b7-125">Accept</span></span>|<span data-ttu-id="5b1b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b1b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b1b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b1b7-127">Request body</span></span>
<span data-ttu-id="5b1b7-128">В теле запроса поставляем представление JSON для [объекта WindowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="5b1b7-129">В следующей таблице показаны свойства, необходимые при создании [windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="5b1b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b1b7-130">Property</span></span>|<span data-ttu-id="5b1b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b1b7-131">Type</span></span>|<span data-ttu-id="5b1b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b1b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b1b7-133">id</span><span class="sxs-lookup"><span data-stu-id="5b1b7-133">id</span></span>|<span data-ttu-id="5b1b7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-134">String</span></span>|<span data-ttu-id="5b1b7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-135">Key of the entity.</span></span> <span data-ttu-id="5b1b7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b1b7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5b1b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b1b7-138">DateTimeOffset</span></span>|<span data-ttu-id="5b1b7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5b1b7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b1b7-141">roleScopeTagIds</span></span>|<span data-ttu-id="5b1b7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5b1b7-142">String collection</span></span>|<span data-ttu-id="5b1b7-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b1b7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5b1b7-145">supportsScopeTags</span></span>|<span data-ttu-id="5b1b7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-146">Boolean</span></span>|<span data-ttu-id="5b1b7-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5b1b7-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5b1b7-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5b1b7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-150">This property is read-only.</span></span> <span data-ttu-id="5b1b7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5b1b7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5b1b7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5b1b7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5b1b7-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5b1b7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5b1b7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5b1b7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5b1b7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5b1b7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5b1b7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5b1b7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5b1b7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5b1b7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5b1b7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5b1b7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b1b7-164">createdDateTime</span></span>|<span data-ttu-id="5b1b7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b1b7-165">DateTimeOffset</span></span>|<span data-ttu-id="5b1b7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-166">DateTime the object was created.</span></span> <span data-ttu-id="5b1b7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-168">description</span><span class="sxs-lookup"><span data-stu-id="5b1b7-168">description</span></span>|<span data-ttu-id="5b1b7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-169">String</span></span>|<span data-ttu-id="5b1b7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b1b7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5b1b7-172">displayName</span></span>|<span data-ttu-id="5b1b7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-173">String</span></span>|<span data-ttu-id="5b1b7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b1b7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-176">version</span><span class="sxs-lookup"><span data-stu-id="5b1b7-176">version</span></span>|<span data-ttu-id="5b1b7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-177">Int32</span></span>|<span data-ttu-id="5b1b7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-178">Version of the device configuration.</span></span> <span data-ttu-id="5b1b7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="5b1b7-180">preSharedKey</span></span>|<span data-ttu-id="5b1b7-181">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-181">String</span></span>|<span data-ttu-id="5b1b7-182">Это предварительный общий ключ для сети персональных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="5b1b7-183">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-184">wifiSecurityType</span></span>|[<span data-ttu-id="5b1b7-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="5b1b7-186">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="5b1b7-187">Унаследовано от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="5b1b7-188">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="5b1b7-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="5b1b7-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="5b1b7-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="5b1b7-191">Укажите тип ограничения дозы подключения для подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="5b1b7-192">Унаследовано от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="5b1b7-193">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="5b1b7-194">ssid</span><span class="sxs-lookup"><span data-stu-id="5b1b7-194">ssid</span></span>|<span data-ttu-id="5b1b7-195">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-195">String</span></span>|<span data-ttu-id="5b1b7-196">Укажите SSID подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="5b1b7-197">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-198">networkName</span><span class="sxs-lookup"><span data-stu-id="5b1b7-198">networkName</span></span>|<span data-ttu-id="5b1b7-199">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-199">String</span></span>|<span data-ttu-id="5b1b7-200">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-200">Specify the network configuration name.</span></span> <span data-ttu-id="5b1b7-201">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="5b1b7-202">connectAutomatically</span></span>|<span data-ttu-id="5b1b7-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-203">Boolean</span></span>|<span data-ttu-id="5b1b7-204">Укажите, должно ли подключение Wi-Fi подключаться автоматически при диапазоне.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="5b1b7-205">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="5b1b7-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="5b1b7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-207">Boolean</span></span>|<span data-ttu-id="5b1b7-208">Укажите, должно ли подключение Wi-Fi подключаться к более предпочтительным сетям при уже подключении к этой.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="5b1b7-209">Требуется, чтобы ConnectAutomatically был правдивым.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="5b1b7-210">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="5b1b7-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="5b1b7-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-212">Boolean</span></span>|<span data-ttu-id="5b1b7-213">Укажите, следует ли подключать подключение к Wi-Fi автоматически, даже если SSID не транслируется.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="5b1b7-214">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="5b1b7-215">proxySetting</span></span>|[<span data-ttu-id="5b1b7-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="5b1b7-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="5b1b7-217">Укажите параметр прокси для Wi-Fi конфигурации, унаследованной от [windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="5b1b7-218">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="5b1b7-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="5b1b7-219">proxyManualAddress</span></span>|<span data-ttu-id="5b1b7-220">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-220">String</span></span>|<span data-ttu-id="5b1b7-221">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="5b1b7-222">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="5b1b7-223">proxyManualPort</span></span>|<span data-ttu-id="5b1b7-224">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-224">Int32</span></span>|<span data-ttu-id="5b1b7-225">Укажите порт для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="5b1b7-226">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="5b1b7-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="5b1b7-228">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-228">String</span></span>|<span data-ttu-id="5b1b7-229">Укажите URL-адрес сценария конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="5b1b7-230">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="5b1b7-231">forceFIPSCompliance</span></span>|<span data-ttu-id="5b1b7-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-232">Boolean</span></span>|<span data-ttu-id="5b1b7-233">Укажите, следует ли принудительно принудить к соблюдению FIPS.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="5b1b7-234">Унаследованный от [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b1b7-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="5b1b7-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="5b1b7-235">networkSingleSignOn</span></span>|[<span data-ttu-id="5b1b7-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="5b1b7-237">Укажите сетевой единый знак по типу.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-237">Specify the network single sign on type.</span></span> <span data-ttu-id="5b1b7-238">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="5b1b7-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b1b7-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="5b1b7-240">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-240">Int32</span></span>|<span data-ttu-id="5b1b7-241">Укажите максимальное время проверки подлинности (в секундах).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="5b1b7-242">Допустимый диапазон: 1-120</span><span class="sxs-lookup"><span data-stu-id="5b1b7-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="5b1b7-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="5b1b7-243">userBasedVirtualLan</span></span>|<span data-ttu-id="5b1b7-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-244">Boolean</span></span>|<span data-ttu-id="5b1b7-245">Указывает, следует ли изменять виртуальный LAN-интерфейс, используемый устройством на основе учетных данных пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="5b1b7-246">Нельзя использовать, если для NetworkSingleSignOnType установлено отключение.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="5b1b7-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="5b1b7-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="5b1b7-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-248">Boolean</span></span>|<span data-ttu-id="5b1b7-249">Укажите, должно ли подключение Wi-Fi подсказать дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="5b1b7-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="5b1b7-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="5b1b7-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-251">Boolean</span></span>|<span data-ttu-id="5b1b7-252">Укажите, должно ли подключение Wi-Fi включить кэшинг ключей в парной области.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="5b1b7-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="5b1b7-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="5b1b7-254">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-254">Int32</span></span>|<span data-ttu-id="5b1b7-255">Укажите максимальное время кэша мастер-ключа парной стрелки (в минутах).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="5b1b7-256">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="5b1b7-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="5b1b7-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="5b1b7-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="5b1b7-258">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-258">Int32</span></span>|<span data-ttu-id="5b1b7-259">Укажите максимальное количество ключей в кэше с парной стрелкой.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="5b1b7-260">Допустимый диапазон: 1-255</span><span class="sxs-lookup"><span data-stu-id="5b1b7-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="5b1b7-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="5b1b7-261">enablePreAuthentication</span></span>|<span data-ttu-id="5b1b7-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-262">Boolean</span></span>|<span data-ttu-id="5b1b7-263">Укажите, должна ли быть включена предварительная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="5b1b7-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="5b1b7-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="5b1b7-265">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-265">Int32</span></span>|<span data-ttu-id="5b1b7-266">Укажите максимальные попытки предварительной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="5b1b7-267">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="5b1b7-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="5b1b7-268">eapType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-268">eapType</span></span>|[<span data-ttu-id="5b1b7-269">eapType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="5b1b7-270">Extensible Authentication Protocol (EAP).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="5b1b7-271">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="5b1b7-272">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="5b1b7-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="5b1b7-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="5b1b7-274">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5b1b7-274">String collection</span></span>|<span data-ttu-id="5b1b7-275">Укажите имена доверенных сертификатов сервера.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="5b1b7-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5b1b7-276">authenticationMethod</span></span>|[<span data-ttu-id="5b1b7-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5b1b7-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="5b1b7-278">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-278">Specify the authentication method.</span></span> <span data-ttu-id="5b1b7-279">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="5b1b7-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="5b1b7-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="5b1b7-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="5b1b7-282">Укажите внутренний протокол проверки подлинности для TTLS EAP.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="5b1b7-283">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="5b1b7-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="5b1b7-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="5b1b7-285">Строка</span><span class="sxs-lookup"><span data-stu-id="5b1b7-285">String</span></span>|<span data-ttu-id="5b1b7-286">Укажите строку для замены имен пользователей для конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="5b1b7-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="5b1b7-287">requireCryptographicBinding</span></span>|<span data-ttu-id="5b1b7-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-288">Boolean</span></span>|<span data-ttu-id="5b1b7-289">Укажите, следует ли включить криптографическую привязку при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="5b1b7-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="5b1b7-290">performServerValidation</span></span>|<span data-ttu-id="5b1b7-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-291">Boolean</span></span>|<span data-ttu-id="5b1b7-292">Укажите, следует ли включить проверку удостоверения сервера путем проверки сертификата при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="5b1b7-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="5b1b7-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="5b1b7-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-294">Boolean</span></span>|<span data-ttu-id="5b1b7-295">Укажите, следует ли запретить пользователю авторизировать новые серверы для доверенных органов сертификации при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="5b1b7-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b1b7-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="5b1b7-297">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-297">Int32</span></span>|<span data-ttu-id="5b1b7-298">Укажите количество секунд, которые клиент должен ждать после попытки проверки подлинности перед сбоем.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="5b1b7-299">Допустимый диапазон 1-3600.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="5b1b7-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b1b7-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="5b1b7-301">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-301">Int32</span></span>|<span data-ttu-id="5b1b7-302">Укажите количество секунд между неудачной проверкой подлинности и следующей попыткой проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="5b1b7-303">Допустимый диапазон 1-3600.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="5b1b7-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="5b1b7-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="5b1b7-305">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-305">Int32</span></span>|<span data-ttu-id="5b1b7-306">Укажите количество секунд, которые необходимо подождать перед отправкой начните сообщение EAPOL (Extensible Authentication Protocol over LAN).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="5b1b7-307">Допустимый диапазон 1-3600.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="5b1b7-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="5b1b7-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="5b1b7-309">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-309">Int32</span></span>|<span data-ttu-id="5b1b7-310">Задано максимальное число протоколов проверки подлинности EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="5b1b7-311">Допустимый диапазон 1-100.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="5b1b7-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="5b1b7-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="5b1b7-313">Int32</span><span class="sxs-lookup"><span data-stu-id="5b1b7-313">Int32</span></span>|<span data-ttu-id="5b1b7-314">Укажите максимально допустимые сбои проверки подлинности для набора учетных данных.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="5b1b7-315">Допустимый диапазон 1-100.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="5b1b7-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="5b1b7-316">cacheCredentials</span></span>|<span data-ttu-id="5b1b7-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b1b7-317">Boolean</span></span>|<span data-ttu-id="5b1b7-318">Укажите, следует ли кэшизировать учетные данные пользователей на устройстве, чтобы пользователям не нужно было постоянно вводить их при каждом подключении.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="5b1b7-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-319">authenticationType</span></span>|[<span data-ttu-id="5b1b7-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="5b1b7-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="5b1b7-321">Укажите, следует ли проверить подлинность пользователя, устройства или использовать гостевую проверку подлинности (нет).</span><span class="sxs-lookup"><span data-stu-id="5b1b7-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="5b1b7-322">Если вы используете проверку подлинности сертификатов, убедитесь, что тип сертификата соответствует типу проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="5b1b7-323">Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="5b1b7-324">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b1b7-324">Response</span></span>
<span data-ttu-id="5b1b7-325">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b1b7-326">Пример</span><span class="sxs-lookup"><span data-stu-id="5b1b7-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b1b7-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b1b7-327">Request</span></span>
<span data-ttu-id="5b1b7-328">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2695

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```

### <a name="response"></a><span data-ttu-id="5b1b7-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b1b7-329">Response</span></span>
<span data-ttu-id="5b1b7-p141">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b1b7-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2867

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```




