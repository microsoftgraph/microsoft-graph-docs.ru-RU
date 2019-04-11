---
title: Обновление Андроидвификонфигуратион
description: Обновление свойств объекта Андроидвификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aff17577144443f4274aed33a386a3f4be4583
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807632"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="36a34-103">Обновление Андроидвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="36a34-103">Update androidWiFiConfiguration</span></span>

> <span data-ttu-id="36a34-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a34-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36a34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a34-106">Обновление свойств объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="36a34-106">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36a34-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36a34-107">Prerequisites</span></span>
<span data-ttu-id="36a34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36a34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36a34-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36a34-110">Permission type</span></span>|<span data-ttu-id="36a34-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36a34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36a34-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36a34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36a34-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36a34-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36a34-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36a34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36a34-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a34-115">Not supported.</span></span>|
|<span data-ttu-id="36a34-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36a34-116">Application</span></span>|<span data-ttu-id="36a34-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36a34-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36a34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="36a34-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36a34-119">Request headers</span></span>
|<span data-ttu-id="36a34-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36a34-120">Header</span></span>|<span data-ttu-id="36a34-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36a34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36a34-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36a34-122">Authorization</span></span>|<span data-ttu-id="36a34-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36a34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36a34-124">Accept</span><span class="sxs-lookup"><span data-stu-id="36a34-124">Accept</span></span>|<span data-ttu-id="36a34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36a34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36a34-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36a34-126">Request body</span></span>
<span data-ttu-id="36a34-127">В тексте запроса добавьте представление объекта [Андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36a34-127">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="36a34-128">В следующей таблице приведены свойства, необходимые при создании [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-128">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="36a34-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="36a34-129">Property</span></span>|<span data-ttu-id="36a34-130">Тип</span><span class="sxs-lookup"><span data-stu-id="36a34-130">Type</span></span>|<span data-ttu-id="36a34-131">Описание</span><span class="sxs-lookup"><span data-stu-id="36a34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36a34-132">id</span><span class="sxs-lookup"><span data-stu-id="36a34-132">id</span></span>|<span data-ttu-id="36a34-133">Строка</span><span class="sxs-lookup"><span data-stu-id="36a34-133">String</span></span>|<span data-ttu-id="36a34-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="36a34-134">Key of the entity.</span></span> <span data-ttu-id="36a34-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36a34-136">lastModifiedDateTime</span></span>|<span data-ttu-id="36a34-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36a34-137">DateTimeOffset</span></span>|<span data-ttu-id="36a34-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="36a34-138">DateTime the object was last modified.</span></span> <span data-ttu-id="36a34-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36a34-140">roleScopeTagIds</span></span>|<span data-ttu-id="36a34-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="36a34-141">String collection</span></span>|<span data-ttu-id="36a34-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="36a34-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36a34-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="36a34-144">supportsScopeTags</span></span>|<span data-ttu-id="36a34-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="36a34-145">Boolean</span></span>|<span data-ttu-id="36a34-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="36a34-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36a34-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="36a34-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36a34-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="36a34-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36a34-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36a34-149">This property is read-only.</span></span> <span data-ttu-id="36a34-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36a34-151">createdDateTime</span></span>|<span data-ttu-id="36a34-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36a34-152">DateTimeOffset</span></span>|<span data-ttu-id="36a34-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="36a34-153">DateTime the object was created.</span></span> <span data-ttu-id="36a34-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-155">description</span><span class="sxs-lookup"><span data-stu-id="36a34-155">description</span></span>|<span data-ttu-id="36a34-156">String</span><span class="sxs-lookup"><span data-stu-id="36a34-156">String</span></span>|<span data-ttu-id="36a34-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36a34-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36a34-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-159">displayName</span><span class="sxs-lookup"><span data-stu-id="36a34-159">displayName</span></span>|<span data-ttu-id="36a34-160">String</span><span class="sxs-lookup"><span data-stu-id="36a34-160">String</span></span>|<span data-ttu-id="36a34-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36a34-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36a34-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-163">version</span><span class="sxs-lookup"><span data-stu-id="36a34-163">version</span></span>|<span data-ttu-id="36a34-164">Int32</span><span class="sxs-lookup"><span data-stu-id="36a34-164">Int32</span></span>|<span data-ttu-id="36a34-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36a34-165">Version of the device configuration.</span></span> <span data-ttu-id="36a34-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36a34-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36a34-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="36a34-167">networkName</span></span>|<span data-ttu-id="36a34-168">String</span><span class="sxs-lookup"><span data-stu-id="36a34-168">String</span></span>|<span data-ttu-id="36a34-169">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="36a34-169">Network Name</span></span>|
|<span data-ttu-id="36a34-170">SSID</span><span class="sxs-lookup"><span data-stu-id="36a34-170">ssid</span></span>|<span data-ttu-id="36a34-171">String</span><span class="sxs-lookup"><span data-stu-id="36a34-171">String</span></span>|<span data-ttu-id="36a34-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="36a34-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="36a34-173">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="36a34-173">connectAutomatically</span></span>|<span data-ttu-id="36a34-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="36a34-174">Boolean</span></span>|<span data-ttu-id="36a34-175">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="36a34-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="36a34-176">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="36a34-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="36a34-177">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="36a34-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="36a34-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="36a34-178">Boolean</span></span>|<span data-ttu-id="36a34-179">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="36a34-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="36a34-180">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="36a34-180">wiFiSecurityType</span></span>|[<span data-ttu-id="36a34-181">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="36a34-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="36a34-182">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="36a34-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="36a34-183">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="36a34-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="36a34-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a34-184">Response</span></span>
<span data-ttu-id="36a34-185">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36a34-185">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36a34-186">Пример</span><span class="sxs-lookup"><span data-stu-id="36a34-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="36a34-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="36a34-187">Request</span></span>
<span data-ttu-id="36a34-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36a34-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="36a34-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a34-189">Response</span></span>
<span data-ttu-id="36a34-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36a34-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```





