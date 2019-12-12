---
title: Создание Андроиддевицеовнервификонфигуратион
description: Создание нового объекта Андроиддевицеовнервификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2930163f530dffd2f7fcbdcf64d7b1e45b486ba1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39953371"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="3968f-103">Создание Андроиддевицеовнервификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="3968f-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="3968f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3968f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3968f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3968f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3968f-106">Создание нового объекта [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3968f-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3968f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3968f-107">Prerequisites</span></span>
<span data-ttu-id="3968f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3968f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3968f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3968f-110">Permission type</span></span>|<span data-ttu-id="3968f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3968f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3968f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3968f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3968f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3968f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3968f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3968f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3968f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3968f-115">Not supported.</span></span>|
|<span data-ttu-id="3968f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3968f-116">Application</span></span>|<span data-ttu-id="3968f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3968f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3968f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3968f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3968f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3968f-119">Request headers</span></span>
|<span data-ttu-id="3968f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3968f-120">Header</span></span>|<span data-ttu-id="3968f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3968f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3968f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3968f-122">Authorization</span></span>|<span data-ttu-id="3968f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3968f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3968f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3968f-124">Accept</span></span>|<span data-ttu-id="3968f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3968f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3968f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3968f-126">Request body</span></span>
<span data-ttu-id="3968f-127">В тексте запроса добавьте представление объекта Андроиддевицеовнервификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3968f-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="3968f-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнервификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="3968f-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="3968f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3968f-129">Property</span></span>|<span data-ttu-id="3968f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3968f-130">Type</span></span>|<span data-ttu-id="3968f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3968f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3968f-132">id</span><span class="sxs-lookup"><span data-stu-id="3968f-132">id</span></span>|<span data-ttu-id="3968f-133">String</span><span class="sxs-lookup"><span data-stu-id="3968f-133">String</span></span>|<span data-ttu-id="3968f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3968f-134">Key of the entity.</span></span> <span data-ttu-id="3968f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3968f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3968f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3968f-137">DateTimeOffset</span></span>|<span data-ttu-id="3968f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3968f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3968f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3968f-140">roleScopeTagIds</span></span>|<span data-ttu-id="3968f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3968f-141">String collection</span></span>|<span data-ttu-id="3968f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3968f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3968f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3968f-144">supportsScopeTags</span></span>|<span data-ttu-id="3968f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3968f-145">Boolean</span></span>|<span data-ttu-id="3968f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3968f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3968f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3968f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3968f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3968f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3968f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3968f-149">This property is read-only.</span></span> <span data-ttu-id="3968f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3968f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3968f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3968f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3968f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3968f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3968f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3968f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3968f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3968f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3968f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3968f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3968f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3968f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3968f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3968f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3968f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3968f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3968f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3968f-163">createdDateTime</span></span>|<span data-ttu-id="3968f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3968f-164">DateTimeOffset</span></span>|<span data-ttu-id="3968f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3968f-165">DateTime the object was created.</span></span> <span data-ttu-id="3968f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-167">description</span><span class="sxs-lookup"><span data-stu-id="3968f-167">description</span></span>|<span data-ttu-id="3968f-168">String</span><span class="sxs-lookup"><span data-stu-id="3968f-168">String</span></span>|<span data-ttu-id="3968f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3968f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3968f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="3968f-171">displayName</span></span>|<span data-ttu-id="3968f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="3968f-172">String</span></span>|<span data-ttu-id="3968f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3968f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3968f-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-175">version</span><span class="sxs-lookup"><span data-stu-id="3968f-175">version</span></span>|<span data-ttu-id="3968f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3968f-176">Int32</span></span>|<span data-ttu-id="3968f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3968f-177">Version of the device configuration.</span></span> <span data-ttu-id="3968f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3968f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3968f-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="3968f-179">networkName</span></span>|<span data-ttu-id="3968f-180">Строка</span><span class="sxs-lookup"><span data-stu-id="3968f-180">String</span></span>|<span data-ttu-id="3968f-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="3968f-181">Network Name</span></span>|
|<span data-ttu-id="3968f-182">SSID</span><span class="sxs-lookup"><span data-stu-id="3968f-182">ssid</span></span>|<span data-ttu-id="3968f-183">Строка</span><span class="sxs-lookup"><span data-stu-id="3968f-183">String</span></span>|<span data-ttu-id="3968f-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="3968f-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="3968f-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="3968f-185">connectAutomatically</span></span>|<span data-ttu-id="3968f-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="3968f-186">Boolean</span></span>|<span data-ttu-id="3968f-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="3968f-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="3968f-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="3968f-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="3968f-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="3968f-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3968f-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3968f-190">Boolean</span></span>|<span data-ttu-id="3968f-191">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="3968f-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="3968f-192">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="3968f-192">wiFiSecurityType</span></span>|[<span data-ttu-id="3968f-193">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3968f-193">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="3968f-194">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="3968f-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="3968f-195">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="3968f-195">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="3968f-196">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="3968f-196">preSharedKey</span></span>|<span data-ttu-id="3968f-197">Строка</span><span class="sxs-lookup"><span data-stu-id="3968f-197">String</span></span>|<span data-ttu-id="3968f-198">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="3968f-198">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="3968f-199">прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="3968f-199">preSharedKeyIsSet</span></span>|<span data-ttu-id="3968f-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="3968f-200">Boolean</span></span>|<span data-ttu-id="3968f-201">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="3968f-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="3968f-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="3968f-202">Response</span></span>
<span data-ttu-id="3968f-203">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3968f-203">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3968f-204">Пример</span><span class="sxs-lookup"><span data-stu-id="3968f-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="3968f-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="3968f-205">Request</span></span>
<span data-ttu-id="3968f-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3968f-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1282

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="3968f-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="3968f-207">Response</span></span>
<span data-ttu-id="3968f-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3968f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1454

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```





