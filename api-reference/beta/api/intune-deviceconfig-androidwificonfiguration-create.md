---
title: Создание androidWiFiConfiguration
description: Создание нового объекта androidWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69ba72acd57454ecd70e6ee0de4cc5a1f8f4f213
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413033"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="849a3-103">Создание androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="849a3-103">Create androidWiFiConfiguration</span></span>

> <span data-ttu-id="849a3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="849a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="849a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="849a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="849a3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="849a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="849a3-107">Создание нового объекта [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="849a3-107">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="849a3-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="849a3-108">Prerequisites</span></span>
<span data-ttu-id="849a3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="849a3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="849a3-111">Permission type</span></span>|<span data-ttu-id="849a3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="849a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="849a3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="849a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="849a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="849a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="849a3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="849a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="849a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="849a3-116">Not supported.</span></span>|
|<span data-ttu-id="849a3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="849a3-117">Application</span></span>|<span data-ttu-id="849a3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="849a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="849a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="849a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="849a3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="849a3-120">Request headers</span></span>
|<span data-ttu-id="849a3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="849a3-121">Header</span></span>|<span data-ttu-id="849a3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="849a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="849a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="849a3-123">Authorization</span></span>|<span data-ttu-id="849a3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="849a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="849a3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="849a3-125">Accept</span></span>|<span data-ttu-id="849a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="849a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="849a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="849a3-127">Request body</span></span>
<span data-ttu-id="849a3-128">В тексте запроса укажите представление JSON для объекта androidWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="849a3-128">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="849a3-129">В следующей таблице показаны свойства, которые необходимы для создания androidWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="849a3-129">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="849a3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="849a3-130">Property</span></span>|<span data-ttu-id="849a3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="849a3-131">Type</span></span>|<span data-ttu-id="849a3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="849a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="849a3-133">id</span><span class="sxs-lookup"><span data-stu-id="849a3-133">id</span></span>|<span data-ttu-id="849a3-134">String</span><span class="sxs-lookup"><span data-stu-id="849a3-134">String</span></span>|<span data-ttu-id="849a3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="849a3-135">Key of the entity.</span></span> <span data-ttu-id="849a3-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="849a3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="849a3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="849a3-138">DateTimeOffset</span></span>|<span data-ttu-id="849a3-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="849a3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="849a3-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="849a3-141">roleScopeTagIds</span></span>|<span data-ttu-id="849a3-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="849a3-142">String collection</span></span>|<span data-ttu-id="849a3-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="849a3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="849a3-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="849a3-145">supportsScopeTags</span></span>|<span data-ttu-id="849a3-146">Логический</span><span class="sxs-lookup"><span data-stu-id="849a3-146">Boolean</span></span>|<span data-ttu-id="849a3-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="849a3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="849a3-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="849a3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="849a3-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="849a3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="849a3-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="849a3-150">This property is read-only.</span></span> <span data-ttu-id="849a3-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="849a3-152">createdDateTime</span></span>|<span data-ttu-id="849a3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="849a3-153">DateTimeOffset</span></span>|<span data-ttu-id="849a3-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="849a3-154">DateTime the object was created.</span></span> <span data-ttu-id="849a3-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-156">description</span><span class="sxs-lookup"><span data-stu-id="849a3-156">description</span></span>|<span data-ttu-id="849a3-157">String</span><span class="sxs-lookup"><span data-stu-id="849a3-157">String</span></span>|<span data-ttu-id="849a3-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="849a3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="849a3-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="849a3-160">displayName</span></span>|<span data-ttu-id="849a3-161">String</span><span class="sxs-lookup"><span data-stu-id="849a3-161">String</span></span>|<span data-ttu-id="849a3-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="849a3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="849a3-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-164">version</span><span class="sxs-lookup"><span data-stu-id="849a3-164">version</span></span>|<span data-ttu-id="849a3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="849a3-165">Int32</span></span>|<span data-ttu-id="849a3-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="849a3-166">Version of the device configuration.</span></span> <span data-ttu-id="849a3-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="849a3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="849a3-168">networkName</span><span class="sxs-lookup"><span data-stu-id="849a3-168">networkName</span></span>|<span data-ttu-id="849a3-169">String</span><span class="sxs-lookup"><span data-stu-id="849a3-169">String</span></span>|<span data-ttu-id="849a3-170">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="849a3-170">Network Name</span></span>|
|<span data-ttu-id="849a3-171">SSID</span><span class="sxs-lookup"><span data-stu-id="849a3-171">ssid</span></span>|<span data-ttu-id="849a3-172">String</span><span class="sxs-lookup"><span data-stu-id="849a3-172">String</span></span>|<span data-ttu-id="849a3-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="849a3-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="849a3-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="849a3-174">connectAutomatically</span></span>|<span data-ttu-id="849a3-175">Логический</span><span class="sxs-lookup"><span data-stu-id="849a3-175">Boolean</span></span>|<span data-ttu-id="849a3-176">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="849a3-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="849a3-177">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="849a3-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="849a3-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="849a3-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="849a3-179">Логический</span><span class="sxs-lookup"><span data-stu-id="849a3-179">Boolean</span></span>|<span data-ttu-id="849a3-180">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="849a3-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="849a3-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="849a3-181">wiFiSecurityType</span></span>|[<span data-ttu-id="849a3-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="849a3-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="849a3-183">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="849a3-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="849a3-184">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="849a3-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="849a3-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="849a3-185">Response</span></span>
<span data-ttu-id="849a3-186">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="849a3-186">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="849a3-187">Пример</span><span class="sxs-lookup"><span data-stu-id="849a3-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="849a3-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="849a3-188">Request</span></span>
<span data-ttu-id="849a3-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="849a3-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="849a3-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="849a3-190">Response</span></span>
<span data-ttu-id="849a3-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="849a3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




