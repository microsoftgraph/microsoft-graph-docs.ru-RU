---
title: Обновление windowsWifiEnterpriseEAPConfiguration
description: Обновление свойств объекта windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d092d4fd5cec9edd1ac102a935c63d9a96501808
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790722"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="dba4c-103">Обновление windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="dba4c-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="dba4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dba4c-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dba4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dba4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba4c-107">Обновление свойств объекта [windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dba4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dba4c-108">Prerequisites</span></span>
<span data-ttu-id="dba4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dba4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dba4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dba4c-111">Permission type</span></span>|<span data-ttu-id="dba4c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dba4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dba4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dba4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dba4c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba4c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dba4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dba4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dba4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba4c-116">Not supported.</span></span>|
|<span data-ttu-id="dba4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dba4c-117">Application</span></span>|<span data-ttu-id="dba4c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba4c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dba4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dba4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dba4c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dba4c-120">Request headers</span></span>
|<span data-ttu-id="dba4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dba4c-121">Header</span></span>|<span data-ttu-id="dba4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dba4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dba4c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dba4c-123">Authorization</span></span>|<span data-ttu-id="dba4c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dba4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dba4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dba4c-125">Accept</span></span>|<span data-ttu-id="dba4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dba4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dba4c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dba4c-127">Request body</span></span>
<span data-ttu-id="dba4c-128">В теле запроса предоставляем представление объекта [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="dba4c-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="dba4c-129">В следующей таблице показаны свойства, необходимые при создании [объекта windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="dba4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dba4c-130">Property</span></span>|<span data-ttu-id="dba4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dba4c-131">Type</span></span>|<span data-ttu-id="dba4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dba4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba4c-133">id</span><span class="sxs-lookup"><span data-stu-id="dba4c-133">id</span></span>|<span data-ttu-id="dba4c-134">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-134">String</span></span>|<span data-ttu-id="dba4c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dba4c-135">Key of the entity.</span></span> <span data-ttu-id="dba4c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dba4c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dba4c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dba4c-138">DateTimeOffset</span></span>|<span data-ttu-id="dba4c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dba4c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dba4c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dba4c-141">roleScopeTagIds</span></span>|<span data-ttu-id="dba4c-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dba4c-142">String collection</span></span>|<span data-ttu-id="dba4c-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dba4c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dba4c-145">supportsScopeTags</span></span>|<span data-ttu-id="dba4c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-146">Boolean</span></span>|<span data-ttu-id="dba4c-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="dba4c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dba4c-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="dba4c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dba4c-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="dba4c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dba4c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dba4c-150">This property is read-only.</span></span> <span data-ttu-id="dba4c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dba4c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dba4c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dba4c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dba4c-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dba4c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dba4c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dba4c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dba4c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dba4c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dba4c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dba4c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dba4c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dba4c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dba4c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dba4c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dba4c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dba4c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dba4c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dba4c-164">createdDateTime</span></span>|<span data-ttu-id="dba4c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dba4c-165">DateTimeOffset</span></span>|<span data-ttu-id="dba4c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dba4c-166">DateTime the object was created.</span></span> <span data-ttu-id="dba4c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-168">description</span><span class="sxs-lookup"><span data-stu-id="dba4c-168">description</span></span>|<span data-ttu-id="dba4c-169">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-169">String</span></span>|<span data-ttu-id="dba4c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dba4c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dba4c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="dba4c-172">displayName</span></span>|<span data-ttu-id="dba4c-173">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-173">String</span></span>|<span data-ttu-id="dba4c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dba4c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dba4c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-176">version</span><span class="sxs-lookup"><span data-stu-id="dba4c-176">version</span></span>|<span data-ttu-id="dba4c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-177">Int32</span></span>|<span data-ttu-id="dba4c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dba4c-178">Version of the device configuration.</span></span> <span data-ttu-id="dba4c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dba4c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="dba4c-180">preSharedKey</span></span>|<span data-ttu-id="dba4c-181">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-181">String</span></span>|<span data-ttu-id="dba4c-182">Это предварительный ключ для личных Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="dba4c-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="dba4c-183">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="dba4c-184">wifiSecurityType</span></span>|[<span data-ttu-id="dba4c-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="dba4c-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="dba4c-186">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="dba4c-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="dba4c-187">Наследуется [от windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="dba4c-188">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="dba4c-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="dba4c-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="dba4c-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="dba4c-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="dba4c-191">Укажите тип лимитного подключения для подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="dba4c-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="dba4c-192">Наследуется [от windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="dba4c-193">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="dba4c-194">ssid</span><span class="sxs-lookup"><span data-stu-id="dba4c-194">ssid</span></span>|<span data-ttu-id="dba4c-195">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-195">String</span></span>|<span data-ttu-id="dba4c-196">Укажите SSID подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="dba4c-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="dba4c-197">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-198">networkName</span><span class="sxs-lookup"><span data-stu-id="dba4c-198">networkName</span></span>|<span data-ttu-id="dba4c-199">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-199">String</span></span>|<span data-ttu-id="dba4c-200">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="dba4c-200">Specify the network configuration name.</span></span> <span data-ttu-id="dba4c-201">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="dba4c-202">connectAutomatically</span></span>|<span data-ttu-id="dba4c-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-203">Boolean</span></span>|<span data-ttu-id="dba4c-204">Укажите, должно ли подключение Wi-Fi подключаться автоматически в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="dba4c-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="dba4c-205">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="dba4c-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="dba4c-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-207">Boolean</span></span>|<span data-ttu-id="dba4c-208">Укажите, должно ли подключение Wi-Fi подключаться к более предпочтительным сетям, уже подключенным к этой сети.</span><span class="sxs-lookup"><span data-stu-id="dba4c-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="dba4c-209">Требуется, чтобы connectAutomatically было true.</span><span class="sxs-lookup"><span data-stu-id="dba4c-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="dba4c-210">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="dba4c-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="dba4c-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-212">Boolean</span></span>|<span data-ttu-id="dba4c-213">Укажите, должно ли подключение Wi-Fi подключаться автоматически, даже если SSID не транслируется.</span><span class="sxs-lookup"><span data-stu-id="dba4c-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="dba4c-214">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="dba4c-215">proxySetting</span></span>|[<span data-ttu-id="dba4c-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="dba4c-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="dba4c-217">Укажите параметр прокси-сервера для Wi-Fi наследуется от [windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="dba4c-218">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="dba4c-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="dba4c-219">proxyManualAddress</span></span>|<span data-ttu-id="dba4c-220">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-220">String</span></span>|<span data-ttu-id="dba4c-221">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="dba4c-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="dba4c-222">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="dba4c-223">proxyManualPort</span></span>|<span data-ttu-id="dba4c-224">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-224">Int32</span></span>|<span data-ttu-id="dba4c-225">Укажите порт для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="dba4c-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="dba4c-226">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="dba4c-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="dba4c-228">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-228">String</span></span>|<span data-ttu-id="dba4c-229">Укажите URL-адрес сценария конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="dba4c-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="dba4c-230">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="dba4c-231">forceFIPSCompliance</span></span>|<span data-ttu-id="dba4c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-232">Boolean</span></span>|<span data-ttu-id="dba4c-233">Укажите, следует ли принудительно обеспечить соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="dba4c-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="dba4c-234">Наследуется [от windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dba4c-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="dba4c-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="dba4c-235">networkSingleSignOn</span></span>|[<span data-ttu-id="dba4c-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="dba4c-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="dba4c-237">Укажите тип единого сетевого знака.</span><span class="sxs-lookup"><span data-stu-id="dba4c-237">Specify the network single sign on type.</span></span> <span data-ttu-id="dba4c-238">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="dba4c-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="dba4c-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="dba4c-240">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-240">Int32</span></span>|<span data-ttu-id="dba4c-241">Укажите максимальное время аутентификации (в секундах).</span><span class="sxs-lookup"><span data-stu-id="dba4c-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="dba4c-242">Допустимый диапазон: 1–120</span><span class="sxs-lookup"><span data-stu-id="dba4c-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="dba4c-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="dba4c-243">userBasedVirtualLan</span></span>|<span data-ttu-id="dba4c-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-244">Boolean</span></span>|<span data-ttu-id="dba4c-245">Указывает, следует ли изменить виртуальную локальной сети, используемую устройством, на основе учетных данных пользователя.</span><span class="sxs-lookup"><span data-stu-id="dba4c-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="dba4c-246">Не может использоваться, если для NetworkSingleSignOnType установлено отключение.</span><span class="sxs-lookup"><span data-stu-id="dba4c-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="dba4c-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="dba4c-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="dba4c-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-248">Boolean</span></span>|<span data-ttu-id="dba4c-249">Укажите, должно ли подключение Wi-Fi запросить дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="dba4c-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="dba4c-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="dba4c-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-251">Boolean</span></span>|<span data-ttu-id="dba4c-252">Укажите, должно ли подключение Wi-Fi включить кэш по парной основной клавише.</span><span class="sxs-lookup"><span data-stu-id="dba4c-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="dba4c-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="dba4c-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="dba4c-254">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-254">Int32</span></span>|<span data-ttu-id="dba4c-255">Укажите максимальное время кэша парных основных ключей (в минутах).</span><span class="sxs-lookup"><span data-stu-id="dba4c-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="dba4c-256">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="dba4c-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="dba4c-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="dba4c-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="dba4c-258">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-258">Int32</span></span>|<span data-ttu-id="dba4c-259">Укажите максимальное количество парных master-ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="dba4c-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="dba4c-260">Допустимый диапазон: 1–255</span><span class="sxs-lookup"><span data-stu-id="dba4c-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="dba4c-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="dba4c-261">enablePreAuthentication</span></span>|<span data-ttu-id="dba4c-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-262">Boolean</span></span>|<span data-ttu-id="dba4c-263">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="dba4c-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="dba4c-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="dba4c-265">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-265">Int32</span></span>|<span data-ttu-id="dba4c-266">Укажите максимальное количество попыток предварительной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="dba4c-267">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="dba4c-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="dba4c-268">eapType</span><span class="sxs-lookup"><span data-stu-id="dba4c-268">eapType</span></span>|[<span data-ttu-id="dba4c-269">eapType</span><span class="sxs-lookup"><span data-stu-id="dba4c-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="dba4c-270">Протокол EAP.</span><span class="sxs-lookup"><span data-stu-id="dba4c-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="dba4c-271">Указывает тип протокола EAP, установленного в конечной точке Wi-Fi (маршрутизаторе).</span><span class="sxs-lookup"><span data-stu-id="dba4c-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="dba4c-272">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="dba4c-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="dba4c-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="dba4c-274">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dba4c-274">String collection</span></span>|<span data-ttu-id="dba4c-275">Укажите имена сертификатов доверенных серверов.</span><span class="sxs-lookup"><span data-stu-id="dba4c-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="dba4c-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dba4c-276">authenticationMethod</span></span>|[<span data-ttu-id="dba4c-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dba4c-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="dba4c-278">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-278">Specify the authentication method.</span></span> <span data-ttu-id="dba4c-279">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="dba4c-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="dba4c-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="dba4c-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="dba4c-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="dba4c-282">Укажите внутренний протокол проверки подлинности для протокола TTLS EAP.</span><span class="sxs-lookup"><span data-stu-id="dba4c-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="dba4c-283">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="dba4c-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="dba4c-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="dba4c-285">String</span><span class="sxs-lookup"><span data-stu-id="dba4c-285">String</span></span>|<span data-ttu-id="dba4c-286">Укажите строку для замены имен пользователей для конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="dba4c-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="dba4c-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="dba4c-287">requireCryptographicBinding</span></span>|<span data-ttu-id="dba4c-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-288">Boolean</span></span>|<span data-ttu-id="dba4c-289">Укажите, следует ли включить криптографическую привязку при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="dba4c-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="dba4c-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="dba4c-290">performServerValidation</span></span>|<span data-ttu-id="dba4c-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-291">Boolean</span></span>|<span data-ttu-id="dba4c-292">Укажите, следует ли включить проверку удостоверения сервера путем проверки сертификата при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="dba4c-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="dba4c-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="dba4c-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="dba4c-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-294">Boolean</span></span>|<span data-ttu-id="dba4c-295">Укажите, следует ли запретить пользователю запрос на авторизации новых серверов для доверенных органов сертификации при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="dba4c-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="dba4c-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="dba4c-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="dba4c-297">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-297">Int32</span></span>|<span data-ttu-id="dba4c-298">Укажите время ожидания клиента в секундах после попытки проверки подлинности перед сбоем.</span><span class="sxs-lookup"><span data-stu-id="dba4c-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="dba4c-299">Допустимый диапазон от 1 до 3600.</span><span class="sxs-lookup"><span data-stu-id="dba4c-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="dba4c-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="dba4c-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="dba4c-301">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-301">Int32</span></span>|<span data-ttu-id="dba4c-302">Укажите количество секунд между неудачной проверкой подлинности и следующей попыткой проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="dba4c-303">Допустимый диапазон от 1 до 3600.</span><span class="sxs-lookup"><span data-stu-id="dba4c-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="dba4c-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="dba4c-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="dba4c-305">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-305">Int32</span></span>|<span data-ttu-id="dba4c-306">Укажите время в секундах до отправки начните сообщения EAPOL (Extensible Authentication Protocol over LAN).</span><span class="sxs-lookup"><span data-stu-id="dba4c-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="dba4c-307">Допустимый диапазон от 1 до 3600.</span><span class="sxs-lookup"><span data-stu-id="dba4c-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="dba4c-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="dba4c-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="dba4c-309">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-309">Int32</span></span>|<span data-ttu-id="dba4c-310">Указывает максимальное количество начните сообщений EAPOL (Extensible Authentication Protocol over LAN), отсылающихся перед возвратом сбоя.</span><span class="sxs-lookup"><span data-stu-id="dba4c-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="dba4c-311">Допустимый диапазон от 1 до 100.</span><span class="sxs-lookup"><span data-stu-id="dba4c-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="dba4c-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="dba4c-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="dba4c-313">Int32</span><span class="sxs-lookup"><span data-stu-id="dba4c-313">Int32</span></span>|<span data-ttu-id="dba4c-314">Укажите максимально допустимые сбои проверки подлинности для набора учетных данных.</span><span class="sxs-lookup"><span data-stu-id="dba4c-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="dba4c-315">Допустимый диапазон от 1 до 100.</span><span class="sxs-lookup"><span data-stu-id="dba4c-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="dba4c-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="dba4c-316">cacheCredentials</span></span>|<span data-ttu-id="dba4c-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4c-317">Boolean</span></span>|<span data-ttu-id="dba4c-318">Укажите, следует ли кэшизировать учетные данные пользователя на устройстве, чтобы пользователям не нужно было вводить их при каждом подключении.</span><span class="sxs-lookup"><span data-stu-id="dba4c-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="dba4c-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="dba4c-319">authenticationType</span></span>|[<span data-ttu-id="dba4c-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="dba4c-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="dba4c-321">Укажите, следует ли проверить подлинность пользователя, устройства или использовать гостевую проверку подлинности (нет).</span><span class="sxs-lookup"><span data-stu-id="dba4c-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="dba4c-322">При использовании проверки подлинности на сертификате убедитесь, что тип сертификата соответствует типу проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="dba4c-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="dba4c-323">Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="dba4c-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="dba4c-324">Отклик</span><span class="sxs-lookup"><span data-stu-id="dba4c-324">Response</span></span>
<span data-ttu-id="dba4c-325">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dba4c-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dba4c-326">Пример</span><span class="sxs-lookup"><span data-stu-id="dba4c-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="dba4c-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="dba4c-327">Request</span></span>
<span data-ttu-id="dba4c-328">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dba4c-328">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dba4c-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="dba4c-329">Response</span></span>
<span data-ttu-id="dba4c-p141">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dba4c-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




