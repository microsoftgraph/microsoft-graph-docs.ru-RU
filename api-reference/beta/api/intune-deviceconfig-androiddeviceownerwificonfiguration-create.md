---
title: Создание Андроиддевицеовнервификонфигуратион
description: Создание нового объекта Андроиддевицеовнервификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1a76c274546815fc6004871b77e08502c4e908e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933160"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="a4dea-103">Создание Андроиддевицеовнервификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="a4dea-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="a4dea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4dea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4dea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4dea-106">Создание нового объекта [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a4dea-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4dea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4dea-107">Prerequisites</span></span>
<span data-ttu-id="a4dea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4dea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4dea-110">Permission type</span></span>|<span data-ttu-id="a4dea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4dea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4dea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4dea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4dea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4dea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4dea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4dea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4dea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dea-115">Not supported.</span></span>|
|<span data-ttu-id="a4dea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4dea-116">Application</span></span>|<span data-ttu-id="a4dea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4dea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4dea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4dea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4dea-119">Request headers</span></span>
|<span data-ttu-id="a4dea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4dea-120">Header</span></span>|<span data-ttu-id="a4dea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a4dea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4dea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4dea-122">Authorization</span></span>|<span data-ttu-id="a4dea-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4dea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4dea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a4dea-124">Accept</span></span>|<span data-ttu-id="a4dea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4dea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4dea-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4dea-126">Request body</span></span>
<span data-ttu-id="a4dea-127">В тексте запроса добавьте представление объекта Андроиддевицеовнервификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4dea-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="a4dea-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнервификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="a4dea-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="a4dea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4dea-129">Property</span></span>|<span data-ttu-id="a4dea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4dea-130">Type</span></span>|<span data-ttu-id="a4dea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4dea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4dea-132">id</span><span class="sxs-lookup"><span data-stu-id="a4dea-132">id</span></span>|<span data-ttu-id="a4dea-133">String</span><span class="sxs-lookup"><span data-stu-id="a4dea-133">String</span></span>|<span data-ttu-id="a4dea-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4dea-134">Key of the entity.</span></span> <span data-ttu-id="a4dea-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4dea-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a4dea-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4dea-137">DateTimeOffset</span></span>|<span data-ttu-id="a4dea-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a4dea-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a4dea-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4dea-140">roleScopeTagIds</span></span>|<span data-ttu-id="a4dea-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a4dea-141">String collection</span></span>|<span data-ttu-id="a4dea-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a4dea-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4dea-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a4dea-144">supportsScopeTags</span></span>|<span data-ttu-id="a4dea-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a4dea-145">Boolean</span></span>|<span data-ttu-id="a4dea-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a4dea-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a4dea-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a4dea-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a4dea-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a4dea-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a4dea-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4dea-149">This property is read-only.</span></span> <span data-ttu-id="a4dea-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4dea-151">createdDateTime</span></span>|<span data-ttu-id="a4dea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4dea-152">DateTimeOffset</span></span>|<span data-ttu-id="a4dea-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a4dea-153">DateTime the object was created.</span></span> <span data-ttu-id="a4dea-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-155">description</span><span class="sxs-lookup"><span data-stu-id="a4dea-155">description</span></span>|<span data-ttu-id="a4dea-156">String</span><span class="sxs-lookup"><span data-stu-id="a4dea-156">String</span></span>|<span data-ttu-id="a4dea-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a4dea-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4dea-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a4dea-159">displayName</span></span>|<span data-ttu-id="a4dea-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dea-160">String</span></span>|<span data-ttu-id="a4dea-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a4dea-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4dea-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-163">version</span><span class="sxs-lookup"><span data-stu-id="a4dea-163">version</span></span>|<span data-ttu-id="a4dea-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a4dea-164">Int32</span></span>|<span data-ttu-id="a4dea-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a4dea-165">Version of the device configuration.</span></span> <span data-ttu-id="a4dea-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4dea-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4dea-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="a4dea-167">networkName</span></span>|<span data-ttu-id="a4dea-168">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dea-168">String</span></span>|<span data-ttu-id="a4dea-169">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="a4dea-169">Network Name</span></span>|
|<span data-ttu-id="a4dea-170">SSID</span><span class="sxs-lookup"><span data-stu-id="a4dea-170">ssid</span></span>|<span data-ttu-id="a4dea-171">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dea-171">String</span></span>|<span data-ttu-id="a4dea-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="a4dea-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="a4dea-173">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="a4dea-173">connectAutomatically</span></span>|<span data-ttu-id="a4dea-174">Логический</span><span class="sxs-lookup"><span data-stu-id="a4dea-174">Boolean</span></span>|<span data-ttu-id="a4dea-175">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="a4dea-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a4dea-176">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="a4dea-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="a4dea-177">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="a4dea-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a4dea-178">Логический</span><span class="sxs-lookup"><span data-stu-id="a4dea-178">Boolean</span></span>|<span data-ttu-id="a4dea-179">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="a4dea-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="a4dea-180">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="a4dea-180">wiFiSecurityType</span></span>|[<span data-ttu-id="a4dea-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a4dea-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="a4dea-182">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="a4dea-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a4dea-183">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="a4dea-183">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="a4dea-184">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a4dea-184">preSharedKey</span></span>|<span data-ttu-id="a4dea-185">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dea-185">String</span></span>|<span data-ttu-id="a4dea-186">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="a4dea-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="a4dea-187">Прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="a4dea-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="a4dea-188">Логический</span><span class="sxs-lookup"><span data-stu-id="a4dea-188">Boolean</span></span>|<span data-ttu-id="a4dea-189">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="a4dea-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="a4dea-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dea-190">Response</span></span>
<span data-ttu-id="a4dea-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4dea-191">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4dea-192">Пример</span><span class="sxs-lookup"><span data-stu-id="a4dea-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4dea-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4dea-193">Request</span></span>
<span data-ttu-id="a4dea-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4dea-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a4dea-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dea-195">Response</span></span>
<span data-ttu-id="a4dea-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4dea-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




