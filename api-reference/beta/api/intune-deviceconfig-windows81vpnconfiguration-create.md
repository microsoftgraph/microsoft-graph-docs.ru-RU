---
title: Создание windows81VpnConfiguration
description: Создание нового объекта windows81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e036ac960cf90d11987f88a19137b443dd4e178c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975913"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="49e64-103">Создание windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="49e64-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="49e64-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49e64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49e64-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49e64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49e64-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49e64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49e64-107">Создание нового объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="49e64-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49e64-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="49e64-108">Prerequisites</span></span>
<span data-ttu-id="49e64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49e64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49e64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49e64-111">Permission type</span></span>|<span data-ttu-id="49e64-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49e64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49e64-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49e64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49e64-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e64-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49e64-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49e64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49e64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49e64-116">Not supported.</span></span>|
|<span data-ttu-id="49e64-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49e64-117">Application</span></span>|<span data-ttu-id="49e64-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49e64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49e64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49e64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49e64-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49e64-120">Request headers</span></span>
|<span data-ttu-id="49e64-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49e64-121">Header</span></span>|<span data-ttu-id="49e64-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49e64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49e64-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49e64-123">Authorization</span></span>|<span data-ttu-id="49e64-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="49e64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49e64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49e64-125">Accept</span></span>|<span data-ttu-id="49e64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49e64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49e64-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49e64-127">Request body</span></span>
<span data-ttu-id="49e64-128">В тексте запроса укажите представление JSON для объекта windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49e64-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="49e64-129">В следующей таблице показаны свойства, которые необходимы для создания windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49e64-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="49e64-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49e64-130">Property</span></span>|<span data-ttu-id="49e64-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49e64-131">Type</span></span>|<span data-ttu-id="49e64-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49e64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e64-133">id</span><span class="sxs-lookup"><span data-stu-id="49e64-133">id</span></span>|<span data-ttu-id="49e64-134">Строка</span><span class="sxs-lookup"><span data-stu-id="49e64-134">String</span></span>|<span data-ttu-id="49e64-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49e64-135">Key of the entity.</span></span> <span data-ttu-id="49e64-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49e64-137">lastModifiedDateTime</span></span>|<span data-ttu-id="49e64-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e64-138">DateTimeOffset</span></span>|<span data-ttu-id="49e64-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="49e64-139">DateTime the object was last modified.</span></span> <span data-ttu-id="49e64-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49e64-141">roleScopeTagIds</span></span>|<span data-ttu-id="49e64-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49e64-142">String collection</span></span>|<span data-ttu-id="49e64-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="49e64-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49e64-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="49e64-145">supportsScopeTags</span></span>|<span data-ttu-id="49e64-146">Логический</span><span class="sxs-lookup"><span data-stu-id="49e64-146">Boolean</span></span>|<span data-ttu-id="49e64-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="49e64-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49e64-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="49e64-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49e64-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="49e64-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49e64-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e64-150">This property is read-only.</span></span> <span data-ttu-id="49e64-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49e64-152">createdDateTime</span></span>|<span data-ttu-id="49e64-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e64-153">DateTimeOffset</span></span>|<span data-ttu-id="49e64-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="49e64-154">DateTime the object was created.</span></span> <span data-ttu-id="49e64-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-156">описание</span><span class="sxs-lookup"><span data-stu-id="49e64-156">description</span></span>|<span data-ttu-id="49e64-157">Строка</span><span class="sxs-lookup"><span data-stu-id="49e64-157">String</span></span>|<span data-ttu-id="49e64-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49e64-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49e64-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-160">displayName</span><span class="sxs-lookup"><span data-stu-id="49e64-160">displayName</span></span>|<span data-ttu-id="49e64-161">Строка</span><span class="sxs-lookup"><span data-stu-id="49e64-161">String</span></span>|<span data-ttu-id="49e64-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49e64-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49e64-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-164">version</span><span class="sxs-lookup"><span data-stu-id="49e64-164">version</span></span>|<span data-ttu-id="49e64-165">Int32</span><span class="sxs-lookup"><span data-stu-id="49e64-165">Int32</span></span>|<span data-ttu-id="49e64-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49e64-166">Version of the device configuration.</span></span> <span data-ttu-id="49e64-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49e64-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="49e64-168">connectionName</span></span>|<span data-ttu-id="49e64-169">Строка</span><span class="sxs-lookup"><span data-stu-id="49e64-169">String</span></span>|<span data-ttu-id="49e64-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="49e64-170">Connection name displayed to the user.</span></span> <span data-ttu-id="49e64-171">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49e64-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-172">серверы</span><span class="sxs-lookup"><span data-stu-id="49e64-172">servers</span></span>|<span data-ttu-id="49e64-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="49e64-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="49e64-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="49e64-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="49e64-175">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="49e64-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="49e64-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="49e64-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="49e64-177">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49e64-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-178">customXml</span><span class="sxs-lookup"><span data-stu-id="49e64-178">customXml</span></span>|<span data-ttu-id="49e64-179">Binary</span><span class="sxs-lookup"><span data-stu-id="49e64-179">Binary</span></span>|<span data-ttu-id="49e64-180">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="49e64-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="49e64-181">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49e64-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="49e64-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="49e64-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="49e64-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e64-183">Boolean</span></span>|<span data-ttu-id="49e64-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="49e64-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="49e64-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49e64-185">This property is read-only.</span></span>|
|<span data-ttu-id="49e64-186">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="49e64-186">connectionType</span></span>|[<span data-ttu-id="49e64-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="49e64-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="49e64-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="49e64-188">Connection type.</span></span> <span data-ttu-id="49e64-189">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="49e64-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="49e64-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="49e64-190">loginGroupOrDomain</span></span>|<span data-ttu-id="49e64-191">Строка</span><span class="sxs-lookup"><span data-stu-id="49e64-191">String</span></span>|<span data-ttu-id="49e64-192">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="49e64-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="49e64-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="49e64-193">enableSplitTunneling</span></span>|<span data-ttu-id="49e64-194">Логический</span><span class="sxs-lookup"><span data-stu-id="49e64-194">Boolean</span></span>|<span data-ttu-id="49e64-195">Включение разделенное туннелирование сети VPN.</span><span class="sxs-lookup"><span data-stu-id="49e64-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="49e64-196">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="49e64-196">proxyServer</span></span>|[<span data-ttu-id="49e64-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="49e64-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="49e64-198">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="49e64-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="49e64-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="49e64-199">Response</span></span>
<span data-ttu-id="49e64-200">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="49e64-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49e64-201">Пример</span><span class="sxs-lookup"><span data-stu-id="49e64-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="49e64-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e64-202">Request</span></span>
<span data-ttu-id="49e64-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49e64-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="49e64-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="49e64-204">Response</span></span>
<span data-ttu-id="49e64-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="49e64-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1187

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```





