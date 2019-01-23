---
title: Обновление androidWorkProfileWiFiConfiguration
description: Обновление свойства объекта androidWorkProfileWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6881b062897d8aa6432cf3b288084d8a3a97c7e4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409596"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="5991b-103">Обновление androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="5991b-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="5991b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5991b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5991b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5991b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5991b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5991b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5991b-107">Обновление свойства объекта [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5991b-107">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5991b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5991b-108">Prerequisites</span></span>
<span data-ttu-id="5991b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5991b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5991b-111">Permission type</span></span>|<span data-ttu-id="5991b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5991b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5991b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5991b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5991b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5991b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5991b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5991b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5991b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5991b-116">Not supported.</span></span>|
|<span data-ttu-id="5991b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5991b-117">Application</span></span>|<span data-ttu-id="5991b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5991b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5991b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5991b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5991b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5991b-120">Request headers</span></span>
|<span data-ttu-id="5991b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5991b-121">Header</span></span>|<span data-ttu-id="5991b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5991b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5991b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5991b-123">Authorization</span></span>|<span data-ttu-id="5991b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5991b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5991b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5991b-125">Accept</span></span>|<span data-ttu-id="5991b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5991b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5991b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5991b-127">Request body</span></span>
<span data-ttu-id="5991b-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5991b-128">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="5991b-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-129">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="5991b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5991b-130">Property</span></span>|<span data-ttu-id="5991b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5991b-131">Type</span></span>|<span data-ttu-id="5991b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5991b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5991b-133">id</span><span class="sxs-lookup"><span data-stu-id="5991b-133">id</span></span>|<span data-ttu-id="5991b-134">String</span><span class="sxs-lookup"><span data-stu-id="5991b-134">String</span></span>|<span data-ttu-id="5991b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5991b-135">Key of the entity.</span></span> <span data-ttu-id="5991b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5991b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5991b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5991b-138">DateTimeOffset</span></span>|<span data-ttu-id="5991b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5991b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5991b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5991b-141">roleScopeTagIds</span></span>|<span data-ttu-id="5991b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5991b-142">String collection</span></span>|<span data-ttu-id="5991b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5991b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5991b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5991b-145">supportsScopeTags</span></span>|<span data-ttu-id="5991b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5991b-146">Boolean</span></span>|<span data-ttu-id="5991b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="5991b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5991b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="5991b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5991b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5991b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5991b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5991b-150">This property is read-only.</span></span> <span data-ttu-id="5991b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5991b-152">createdDateTime</span></span>|<span data-ttu-id="5991b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5991b-153">DateTimeOffset</span></span>|<span data-ttu-id="5991b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5991b-154">DateTime the object was created.</span></span> <span data-ttu-id="5991b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-156">description</span><span class="sxs-lookup"><span data-stu-id="5991b-156">description</span></span>|<span data-ttu-id="5991b-157">String</span><span class="sxs-lookup"><span data-stu-id="5991b-157">String</span></span>|<span data-ttu-id="5991b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5991b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5991b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5991b-160">displayName</span></span>|<span data-ttu-id="5991b-161">String</span><span class="sxs-lookup"><span data-stu-id="5991b-161">String</span></span>|<span data-ttu-id="5991b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5991b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5991b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-164">version</span><span class="sxs-lookup"><span data-stu-id="5991b-164">version</span></span>|<span data-ttu-id="5991b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5991b-165">Int32</span></span>|<span data-ttu-id="5991b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5991b-166">Version of the device configuration.</span></span> <span data-ttu-id="5991b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5991b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5991b-168">networkName</span><span class="sxs-lookup"><span data-stu-id="5991b-168">networkName</span></span>|<span data-ttu-id="5991b-169">String</span><span class="sxs-lookup"><span data-stu-id="5991b-169">String</span></span>|<span data-ttu-id="5991b-170">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="5991b-170">Network Name</span></span>|
|<span data-ttu-id="5991b-171">SSID</span><span class="sxs-lookup"><span data-stu-id="5991b-171">ssid</span></span>|<span data-ttu-id="5991b-172">String</span><span class="sxs-lookup"><span data-stu-id="5991b-172">String</span></span>|<span data-ttu-id="5991b-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="5991b-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="5991b-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="5991b-174">connectAutomatically</span></span>|<span data-ttu-id="5991b-175">Логический</span><span class="sxs-lookup"><span data-stu-id="5991b-175">Boolean</span></span>|<span data-ttu-id="5991b-176">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="5991b-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="5991b-177">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="5991b-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="5991b-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="5991b-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="5991b-179">Логический</span><span class="sxs-lookup"><span data-stu-id="5991b-179">Boolean</span></span>|<span data-ttu-id="5991b-180">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="5991b-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="5991b-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="5991b-181">wiFiSecurityType</span></span>|[<span data-ttu-id="5991b-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="5991b-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="5991b-183">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="5991b-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="5991b-184">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="5991b-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="5991b-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="5991b-185">Response</span></span>
<span data-ttu-id="5991b-186">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5991b-186">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5991b-187">Пример</span><span class="sxs-lookup"><span data-stu-id="5991b-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="5991b-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="5991b-188">Request</span></span>
<span data-ttu-id="5991b-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5991b-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 446

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="5991b-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="5991b-190">Response</span></span>
<span data-ttu-id="5991b-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5991b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 618

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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




