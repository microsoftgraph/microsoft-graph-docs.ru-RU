---
title: Обновление Андроиддевицеовнервификонфигуратион
description: Обновление свойств объекта Андроиддевицеовнервификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6de60af4f1bc0dbf2c221c3d2062fd88957cdd3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479738"
---
# <a name="update-androiddeviceownerwificonfiguration"></a><span data-ttu-id="67978-103">Обновление Андроиддевицеовнервификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="67978-103">Update androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="67978-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67978-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67978-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67978-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67978-106">Обновление свойств объекта [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="67978-106">Update the properties of a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67978-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67978-107">Prerequisites</span></span>
<span data-ttu-id="67978-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67978-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67978-110">Permission type</span></span>|<span data-ttu-id="67978-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67978-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67978-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67978-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67978-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67978-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67978-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67978-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67978-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67978-115">Not supported.</span></span>|
|<span data-ttu-id="67978-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67978-116">Application</span></span>|<span data-ttu-id="67978-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67978-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67978-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67978-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="67978-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67978-119">Request headers</span></span>
|<span data-ttu-id="67978-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67978-120">Header</span></span>|<span data-ttu-id="67978-121">Значение</span><span class="sxs-lookup"><span data-stu-id="67978-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67978-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67978-122">Authorization</span></span>|<span data-ttu-id="67978-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67978-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67978-124">Accept</span><span class="sxs-lookup"><span data-stu-id="67978-124">Accept</span></span>|<span data-ttu-id="67978-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67978-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67978-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67978-126">Request body</span></span>
<span data-ttu-id="67978-127">В тексте запроса добавьте представление объекта [Андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67978-127">In the request body, supply a JSON representation for the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

<span data-ttu-id="67978-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-128">The following table shows the properties that are required when you create the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span>

|<span data-ttu-id="67978-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="67978-129">Property</span></span>|<span data-ttu-id="67978-130">Тип</span><span class="sxs-lookup"><span data-stu-id="67978-130">Type</span></span>|<span data-ttu-id="67978-131">Описание</span><span class="sxs-lookup"><span data-stu-id="67978-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67978-132">id</span><span class="sxs-lookup"><span data-stu-id="67978-132">id</span></span>|<span data-ttu-id="67978-133">Строка</span><span class="sxs-lookup"><span data-stu-id="67978-133">String</span></span>|<span data-ttu-id="67978-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67978-134">Key of the entity.</span></span> <span data-ttu-id="67978-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67978-136">lastModifiedDateTime</span></span>|<span data-ttu-id="67978-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67978-137">DateTimeOffset</span></span>|<span data-ttu-id="67978-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="67978-138">DateTime the object was last modified.</span></span> <span data-ttu-id="67978-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67978-140">roleScopeTagIds</span></span>|<span data-ttu-id="67978-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67978-141">String collection</span></span>|<span data-ttu-id="67978-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="67978-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67978-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="67978-144">supportsScopeTags</span></span>|<span data-ttu-id="67978-145">Логический</span><span class="sxs-lookup"><span data-stu-id="67978-145">Boolean</span></span>|<span data-ttu-id="67978-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="67978-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="67978-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="67978-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="67978-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="67978-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="67978-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67978-149">This property is read-only.</span></span> <span data-ttu-id="67978-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67978-151">createdDateTime</span></span>|<span data-ttu-id="67978-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67978-152">DateTimeOffset</span></span>|<span data-ttu-id="67978-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="67978-153">DateTime the object was created.</span></span> <span data-ttu-id="67978-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-155">description</span><span class="sxs-lookup"><span data-stu-id="67978-155">description</span></span>|<span data-ttu-id="67978-156">String</span><span class="sxs-lookup"><span data-stu-id="67978-156">String</span></span>|<span data-ttu-id="67978-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67978-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67978-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-159">displayName</span><span class="sxs-lookup"><span data-stu-id="67978-159">displayName</span></span>|<span data-ttu-id="67978-160">String</span><span class="sxs-lookup"><span data-stu-id="67978-160">String</span></span>|<span data-ttu-id="67978-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67978-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67978-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-163">version</span><span class="sxs-lookup"><span data-stu-id="67978-163">version</span></span>|<span data-ttu-id="67978-164">Int32</span><span class="sxs-lookup"><span data-stu-id="67978-164">Int32</span></span>|<span data-ttu-id="67978-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67978-165">Version of the device configuration.</span></span> <span data-ttu-id="67978-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67978-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67978-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="67978-167">networkName</span></span>|<span data-ttu-id="67978-168">String</span><span class="sxs-lookup"><span data-stu-id="67978-168">String</span></span>|<span data-ttu-id="67978-169">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="67978-169">Network Name</span></span>|
|<span data-ttu-id="67978-170">SSID</span><span class="sxs-lookup"><span data-stu-id="67978-170">ssid</span></span>|<span data-ttu-id="67978-171">String</span><span class="sxs-lookup"><span data-stu-id="67978-171">String</span></span>|<span data-ttu-id="67978-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="67978-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="67978-173">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="67978-173">connectAutomatically</span></span>|<span data-ttu-id="67978-174">Логический</span><span class="sxs-lookup"><span data-stu-id="67978-174">Boolean</span></span>|<span data-ttu-id="67978-175">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="67978-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="67978-176">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="67978-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="67978-177">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="67978-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="67978-178">Логический</span><span class="sxs-lookup"><span data-stu-id="67978-178">Boolean</span></span>|<span data-ttu-id="67978-179">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="67978-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="67978-180">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="67978-180">wiFiSecurityType</span></span>|[<span data-ttu-id="67978-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="67978-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="67978-182">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="67978-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="67978-183">Возможные значения: `open`, `wep`, `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="67978-183">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="67978-184">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="67978-184">preSharedKey</span></span>|<span data-ttu-id="67978-185">String</span><span class="sxs-lookup"><span data-stu-id="67978-185">String</span></span>|<span data-ttu-id="67978-186">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="67978-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="67978-187">Прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="67978-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="67978-188">Логический</span><span class="sxs-lookup"><span data-stu-id="67978-188">Boolean</span></span>|<span data-ttu-id="67978-189">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="67978-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="67978-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="67978-190">Response</span></span>
<span data-ttu-id="67978-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67978-191">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67978-192">Пример</span><span class="sxs-lookup"><span data-stu-id="67978-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="67978-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="67978-193">Request</span></span>
<span data-ttu-id="67978-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67978-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="67978-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="67978-195">Response</span></span>
<span data-ttu-id="67978-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67978-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 681

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





