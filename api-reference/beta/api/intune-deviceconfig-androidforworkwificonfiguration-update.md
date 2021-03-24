---
title: Обновление androidForWorkWiFiConfiguration
description: Обновление свойств объекта AndroidForWorkWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a8f45dd609964ae1800d0a1d952a584ee2e5e154
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130233"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="3c2f7-103">Обновление androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c2f7-103">Update androidForWorkWiFiConfiguration</span></span>

<span data-ttu-id="3c2f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c2f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c2f7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c2f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c2f7-107">Обновление свойств объекта [AndroidForWorkWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c2f7-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c2f7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c2f7-108">Prerequisites</span></span>
<span data-ttu-id="3c2f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c2f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c2f7-111">Permission type</span></span>|<span data-ttu-id="3c2f7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c2f7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c2f7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c2f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c2f7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c2f7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c2f7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c2f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c2f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-116">Not supported.</span></span>|
|<span data-ttu-id="3c2f7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3c2f7-117">Application</span></span>|<span data-ttu-id="3c2f7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c2f7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c2f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c2f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3c2f7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3c2f7-120">Request headers</span></span>
|<span data-ttu-id="3c2f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c2f7-121">Header</span></span>|<span data-ttu-id="3c2f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c2f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c2f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c2f7-123">Authorization</span></span>|<span data-ttu-id="3c2f7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c2f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c2f7-125">Accept</span></span>|<span data-ttu-id="3c2f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c2f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c2f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c2f7-127">Request body</span></span>
<span data-ttu-id="3c2f7-128">В теле запроса предоставляем представление JSON для [объекта AndroidForWorkWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c2f7-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="3c2f7-129">В следующей таблице показаны свойства, необходимые при создании [androidForWorkWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3c2f7-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="3c2f7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c2f7-130">Property</span></span>|<span data-ttu-id="3c2f7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c2f7-131">Type</span></span>|<span data-ttu-id="3c2f7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c2f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c2f7-133">id</span><span class="sxs-lookup"><span data-stu-id="3c2f7-133">id</span></span>|<span data-ttu-id="3c2f7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2f7-134">String</span></span>|<span data-ttu-id="3c2f7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-135">Key of the entity.</span></span> <span data-ttu-id="3c2f7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2f7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3c2f7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c2f7-138">DateTimeOffset</span></span>|<span data-ttu-id="3c2f7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3c2f7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3c2f7-141">roleScopeTagIds</span></span>|<span data-ttu-id="3c2f7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c2f7-142">String collection</span></span>|<span data-ttu-id="3c2f7-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3c2f7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3c2f7-145">supportsScopeTags</span></span>|<span data-ttu-id="3c2f7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c2f7-146">Boolean</span></span>|<span data-ttu-id="3c2f7-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3c2f7-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3c2f7-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3c2f7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-150">This property is read-only.</span></span> <span data-ttu-id="3c2f7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3c2f7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3c2f7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3c2f7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3c2f7-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3c2f7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3c2f7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3c2f7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3c2f7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3c2f7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3c2f7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3c2f7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3c2f7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3c2f7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3c2f7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3c2f7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c2f7-164">createdDateTime</span></span>|<span data-ttu-id="3c2f7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c2f7-165">DateTimeOffset</span></span>|<span data-ttu-id="3c2f7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-166">DateTime the object was created.</span></span> <span data-ttu-id="3c2f7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-168">description</span><span class="sxs-lookup"><span data-stu-id="3c2f7-168">description</span></span>|<span data-ttu-id="3c2f7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2f7-169">String</span></span>|<span data-ttu-id="3c2f7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3c2f7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3c2f7-172">displayName</span></span>|<span data-ttu-id="3c2f7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2f7-173">String</span></span>|<span data-ttu-id="3c2f7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3c2f7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-176">version</span><span class="sxs-lookup"><span data-stu-id="3c2f7-176">version</span></span>|<span data-ttu-id="3c2f7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3c2f7-177">Int32</span></span>|<span data-ttu-id="3c2f7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-178">Version of the device configuration.</span></span> <span data-ttu-id="3c2f7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c2f7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3c2f7-180">networkName</span><span class="sxs-lookup"><span data-stu-id="3c2f7-180">networkName</span></span>|<span data-ttu-id="3c2f7-181">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2f7-181">String</span></span>|<span data-ttu-id="3c2f7-182">Имя сети</span><span class="sxs-lookup"><span data-stu-id="3c2f7-182">Network Name</span></span>|
|<span data-ttu-id="3c2f7-183">ssid</span><span class="sxs-lookup"><span data-stu-id="3c2f7-183">ssid</span></span>|<span data-ttu-id="3c2f7-184">Строка</span><span class="sxs-lookup"><span data-stu-id="3c2f7-184">String</span></span>|<span data-ttu-id="3c2f7-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="3c2f7-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3c2f7-186">connectAutomatically</span></span>|<span data-ttu-id="3c2f7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c2f7-187">Boolean</span></span>|<span data-ttu-id="3c2f7-188">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="3c2f7-189">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="3c2f7-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3c2f7-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3c2f7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c2f7-191">Boolean</span></span>|<span data-ttu-id="3c2f7-192">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="3c2f7-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3c2f7-193">wiFiSecurityType</span></span>|[<span data-ttu-id="3c2f7-194">AndroidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3c2f7-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="3c2f7-195">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="3c2f7-196">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="3c2f7-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c2f7-197">Response</span></span>
<span data-ttu-id="3c2f7-198">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-198">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c2f7-199">Пример</span><span class="sxs-lookup"><span data-stu-id="3c2f7-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c2f7-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c2f7-200">Request</span></span>
<span data-ttu-id="3c2f7-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1215

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="3c2f7-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c2f7-202">Response</span></span>
<span data-ttu-id="3c2f7-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c2f7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1387

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```




