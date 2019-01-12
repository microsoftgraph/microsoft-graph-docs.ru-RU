---
title: Создание androidWorkProfileWiFiConfiguration
description: Создание нового объекта androidWorkProfileWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e7949c7f583c8f36a959ffd2013b260b958e6af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957846"
---
# <a name="create-androidworkprofilewificonfiguration"></a><span data-ttu-id="84123-103">Создание androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="84123-103">Create androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="84123-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84123-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84123-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84123-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84123-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84123-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84123-107">Создание нового объекта [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="84123-107">Create a new [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84123-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84123-108">Prerequisites</span></span>
<span data-ttu-id="84123-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84123-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84123-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84123-111">Permission type</span></span>|<span data-ttu-id="84123-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84123-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84123-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84123-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84123-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84123-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84123-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84123-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84123-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84123-116">Not supported.</span></span>|
|<span data-ttu-id="84123-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84123-117">Application</span></span>|<span data-ttu-id="84123-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84123-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84123-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84123-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84123-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84123-120">Request headers</span></span>
|<span data-ttu-id="84123-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84123-121">Header</span></span>|<span data-ttu-id="84123-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84123-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84123-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84123-123">Authorization</span></span>|<span data-ttu-id="84123-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84123-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84123-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84123-125">Accept</span></span>|<span data-ttu-id="84123-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84123-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84123-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84123-127">Request body</span></span>
<span data-ttu-id="84123-128">В тексте запроса укажите представление JSON для объекта androidWorkProfileWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84123-128">In the request body, supply a JSON representation for the androidWorkProfileWiFiConfiguration object.</span></span>

<span data-ttu-id="84123-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84123-129">The following table shows the properties that are required when you create the androidWorkProfileWiFiConfiguration.</span></span>

|<span data-ttu-id="84123-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84123-130">Property</span></span>|<span data-ttu-id="84123-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84123-131">Type</span></span>|<span data-ttu-id="84123-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84123-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84123-133">id</span><span class="sxs-lookup"><span data-stu-id="84123-133">id</span></span>|<span data-ttu-id="84123-134">Строка</span><span class="sxs-lookup"><span data-stu-id="84123-134">String</span></span>|<span data-ttu-id="84123-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84123-135">Key of the entity.</span></span> <span data-ttu-id="84123-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84123-137">lastModifiedDateTime</span></span>|<span data-ttu-id="84123-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84123-138">DateTimeOffset</span></span>|<span data-ttu-id="84123-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="84123-139">DateTime the object was last modified.</span></span> <span data-ttu-id="84123-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84123-141">roleScopeTagIds</span></span>|<span data-ttu-id="84123-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84123-142">String collection</span></span>|<span data-ttu-id="84123-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="84123-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84123-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84123-145">supportsScopeTags</span></span>|<span data-ttu-id="84123-146">Логический</span><span class="sxs-lookup"><span data-stu-id="84123-146">Boolean</span></span>|<span data-ttu-id="84123-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="84123-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84123-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="84123-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84123-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="84123-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84123-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84123-150">This property is read-only.</span></span> <span data-ttu-id="84123-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84123-152">createdDateTime</span></span>|<span data-ttu-id="84123-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84123-153">DateTimeOffset</span></span>|<span data-ttu-id="84123-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="84123-154">DateTime the object was created.</span></span> <span data-ttu-id="84123-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-156">описание</span><span class="sxs-lookup"><span data-stu-id="84123-156">description</span></span>|<span data-ttu-id="84123-157">Строка</span><span class="sxs-lookup"><span data-stu-id="84123-157">String</span></span>|<span data-ttu-id="84123-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84123-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84123-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-160">displayName</span><span class="sxs-lookup"><span data-stu-id="84123-160">displayName</span></span>|<span data-ttu-id="84123-161">Строка</span><span class="sxs-lookup"><span data-stu-id="84123-161">String</span></span>|<span data-ttu-id="84123-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84123-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84123-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-164">version</span><span class="sxs-lookup"><span data-stu-id="84123-164">version</span></span>|<span data-ttu-id="84123-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84123-165">Int32</span></span>|<span data-ttu-id="84123-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84123-166">Version of the device configuration.</span></span> <span data-ttu-id="84123-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84123-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84123-168">networkName</span><span class="sxs-lookup"><span data-stu-id="84123-168">networkName</span></span>|<span data-ttu-id="84123-169">Строка</span><span class="sxs-lookup"><span data-stu-id="84123-169">String</span></span>|<span data-ttu-id="84123-170">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="84123-170">Network Name</span></span>|
|<span data-ttu-id="84123-171">SSID</span><span class="sxs-lookup"><span data-stu-id="84123-171">ssid</span></span>|<span data-ttu-id="84123-172">Строка</span><span class="sxs-lookup"><span data-stu-id="84123-172">String</span></span>|<span data-ttu-id="84123-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="84123-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="84123-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="84123-174">connectAutomatically</span></span>|<span data-ttu-id="84123-175">Логический</span><span class="sxs-lookup"><span data-stu-id="84123-175">Boolean</span></span>|<span data-ttu-id="84123-176">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="84123-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="84123-177">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="84123-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="84123-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="84123-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="84123-179">Логический</span><span class="sxs-lookup"><span data-stu-id="84123-179">Boolean</span></span>|<span data-ttu-id="84123-180">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="84123-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="84123-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="84123-181">wiFiSecurityType</span></span>|[<span data-ttu-id="84123-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="84123-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="84123-183">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="84123-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="84123-184">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="84123-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="84123-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="84123-185">Response</span></span>
<span data-ttu-id="84123-186">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="84123-186">If successful, this method returns a `201 Created` response code and a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84123-187">Пример</span><span class="sxs-lookup"><span data-stu-id="84123-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="84123-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="84123-188">Request</span></span>
<span data-ttu-id="84123-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84123-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 510

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="84123-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="84123-190">Response</span></span>
<span data-ttu-id="84123-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84123-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





