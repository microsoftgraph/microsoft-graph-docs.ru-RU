---
title: Создание androidDeviceOwnerWiFiConfiguration
description: Создание нового объекта androidDeviceOwnerWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7fc0fbc146b9b77c2415715cdbdb5aded5a079c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823046"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="35f0a-103">Создание androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="35f0a-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="35f0a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35f0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35f0a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35f0a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35f0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35f0a-107">Создание нового объекта [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="35f0a-107">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35f0a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35f0a-108">Prerequisites</span></span>
<span data-ttu-id="35f0a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35f0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f0a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35f0a-111">Permission type</span></span>|<span data-ttu-id="35f0a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35f0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f0a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35f0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35f0a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f0a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35f0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35f0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f0a-116">Not supported.</span></span>|
|<span data-ttu-id="35f0a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35f0a-117">Application</span></span>|<span data-ttu-id="35f0a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f0a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35f0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35f0a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35f0a-120">Request headers</span></span>
|<span data-ttu-id="35f0a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35f0a-121">Header</span></span>|<span data-ttu-id="35f0a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35f0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35f0a-123">Authorization</span></span>|<span data-ttu-id="35f0a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35f0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f0a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35f0a-125">Accept</span></span>|<span data-ttu-id="35f0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35f0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f0a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35f0a-127">Request body</span></span>
<span data-ttu-id="35f0a-128">В тексте запроса укажите представление JSON для объекта androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35f0a-128">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="35f0a-129">В следующей таблице показаны свойства, которые необходимы для создания androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="35f0a-129">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="35f0a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="35f0a-130">Property</span></span>|<span data-ttu-id="35f0a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="35f0a-131">Type</span></span>|<span data-ttu-id="35f0a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="35f0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f0a-133">id</span><span class="sxs-lookup"><span data-stu-id="35f0a-133">id</span></span>|<span data-ttu-id="35f0a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="35f0a-134">String</span></span>|<span data-ttu-id="35f0a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35f0a-135">Key of the entity.</span></span> <span data-ttu-id="35f0a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35f0a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="35f0a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f0a-138">DateTimeOffset</span></span>|<span data-ttu-id="35f0a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="35f0a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="35f0a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35f0a-141">roleScopeTagIds</span></span>|<span data-ttu-id="35f0a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="35f0a-142">String collection</span></span>|<span data-ttu-id="35f0a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="35f0a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35f0a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35f0a-145">supportsScopeTags</span></span>|<span data-ttu-id="35f0a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="35f0a-146">Boolean</span></span>|<span data-ttu-id="35f0a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="35f0a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35f0a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="35f0a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35f0a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="35f0a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35f0a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35f0a-150">This property is read-only.</span></span> <span data-ttu-id="35f0a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35f0a-152">createdDateTime</span></span>|<span data-ttu-id="35f0a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f0a-153">DateTimeOffset</span></span>|<span data-ttu-id="35f0a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="35f0a-154">DateTime the object was created.</span></span> <span data-ttu-id="35f0a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-156">описание</span><span class="sxs-lookup"><span data-stu-id="35f0a-156">description</span></span>|<span data-ttu-id="35f0a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="35f0a-157">String</span></span>|<span data-ttu-id="35f0a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35f0a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35f0a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="35f0a-160">displayName</span></span>|<span data-ttu-id="35f0a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="35f0a-161">String</span></span>|<span data-ttu-id="35f0a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35f0a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35f0a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-164">version</span><span class="sxs-lookup"><span data-stu-id="35f0a-164">version</span></span>|<span data-ttu-id="35f0a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="35f0a-165">Int32</span></span>|<span data-ttu-id="35f0a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="35f0a-166">Version of the device configuration.</span></span> <span data-ttu-id="35f0a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35f0a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0a-168">networkName</span><span class="sxs-lookup"><span data-stu-id="35f0a-168">networkName</span></span>|<span data-ttu-id="35f0a-169">Строка</span><span class="sxs-lookup"><span data-stu-id="35f0a-169">String</span></span>|<span data-ttu-id="35f0a-170">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="35f0a-170">Network Name</span></span>|
|<span data-ttu-id="35f0a-171">SSID</span><span class="sxs-lookup"><span data-stu-id="35f0a-171">ssid</span></span>|<span data-ttu-id="35f0a-172">Строка</span><span class="sxs-lookup"><span data-stu-id="35f0a-172">String</span></span>|<span data-ttu-id="35f0a-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="35f0a-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="35f0a-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="35f0a-174">connectAutomatically</span></span>|<span data-ttu-id="35f0a-175">Логический</span><span class="sxs-lookup"><span data-stu-id="35f0a-175">Boolean</span></span>|<span data-ttu-id="35f0a-176">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="35f0a-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="35f0a-177">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="35f0a-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="35f0a-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="35f0a-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="35f0a-179">Логический</span><span class="sxs-lookup"><span data-stu-id="35f0a-179">Boolean</span></span>|<span data-ttu-id="35f0a-180">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="35f0a-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="35f0a-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="35f0a-181">wiFiSecurityType</span></span>|[<span data-ttu-id="35f0a-182">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="35f0a-182">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="35f0a-183">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="35f0a-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="35f0a-184">Возможные значения: `open`, `wep`, `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="35f0a-184">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="35f0a-185">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="35f0a-185">preSharedKey</span></span>|<span data-ttu-id="35f0a-186">Строка</span><span class="sxs-lookup"><span data-stu-id="35f0a-186">String</span></span>|<span data-ttu-id="35f0a-187">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="35f0a-187">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="35f0a-188">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="35f0a-188">preSharedKeyIsSet</span></span>|<span data-ttu-id="35f0a-189">Логический</span><span class="sxs-lookup"><span data-stu-id="35f0a-189">Boolean</span></span>|<span data-ttu-id="35f0a-190">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="35f0a-190">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="35f0a-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="35f0a-191">Response</span></span>
<span data-ttu-id="35f0a-192">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="35f0a-192">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f0a-193">Пример</span><span class="sxs-lookup"><span data-stu-id="35f0a-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="35f0a-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="35f0a-194">Request</span></span>
<span data-ttu-id="35f0a-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35f0a-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="35f0a-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="35f0a-196">Response</span></span>
<span data-ttu-id="35f0a-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35f0a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





