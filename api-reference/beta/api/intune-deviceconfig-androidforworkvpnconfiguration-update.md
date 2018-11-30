---
title: Обновление androidForWorkVpnConfiguration
description: Обновление свойства объекта androidForWorkVpnConfiguration.
ms.openlocfilehash: f63c315b0e291b84169c813a0b2ffbf0c7bebda2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078607"
---
# <a name="update-androidforworkvpnconfiguration"></a><span data-ttu-id="5839b-103">Обновление androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="5839b-103">Update androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="5839b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5839b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5839b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5839b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5839b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5839b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5839b-107">Обновление свойства объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5839b-107">Update the properties of a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5839b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5839b-108">Prerequisites</span></span>
<span data-ttu-id="5839b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5839b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5839b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5839b-111">Permission type</span></span>|<span data-ttu-id="5839b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5839b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5839b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5839b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5839b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5839b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5839b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5839b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5839b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5839b-116">Not supported.</span></span>|
|<span data-ttu-id="5839b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5839b-117">Application</span></span>|<span data-ttu-id="5839b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5839b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5839b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5839b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5839b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5839b-120">Request headers</span></span>
|<span data-ttu-id="5839b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5839b-121">Header</span></span>|<span data-ttu-id="5839b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5839b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5839b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5839b-123">Authorization</span></span>|<span data-ttu-id="5839b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5839b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5839b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5839b-125">Accept</span></span>|<span data-ttu-id="5839b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5839b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5839b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5839b-127">Request body</span></span>
<span data-ttu-id="5839b-128">В тексте запроса укажите представление JSON для объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5839b-128">In the request body, supply a JSON representation for the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

<span data-ttu-id="5839b-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-129">The following table shows the properties that are required when you create the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span></span>

|<span data-ttu-id="5839b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5839b-130">Property</span></span>|<span data-ttu-id="5839b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5839b-131">Type</span></span>|<span data-ttu-id="5839b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5839b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5839b-133">id</span><span class="sxs-lookup"><span data-stu-id="5839b-133">id</span></span>|<span data-ttu-id="5839b-134">String</span><span class="sxs-lookup"><span data-stu-id="5839b-134">String</span></span>|<span data-ttu-id="5839b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5839b-135">Key of the entity.</span></span> <span data-ttu-id="5839b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5839b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5839b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5839b-138">DateTimeOffset</span></span>|<span data-ttu-id="5839b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5839b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5839b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5839b-141">roleScopeTagIds</span></span>|<span data-ttu-id="5839b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5839b-142">String collection</span></span>|<span data-ttu-id="5839b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5839b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5839b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5839b-145">supportsScopeTags</span></span>|<span data-ttu-id="5839b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5839b-146">Boolean</span></span>|<span data-ttu-id="5839b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="5839b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5839b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="5839b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5839b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5839b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5839b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5839b-150">This property is read-only.</span></span> <span data-ttu-id="5839b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5839b-152">createdDateTime</span></span>|<span data-ttu-id="5839b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5839b-153">DateTimeOffset</span></span>|<span data-ttu-id="5839b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5839b-154">DateTime the object was created.</span></span> <span data-ttu-id="5839b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-156">описание</span><span class="sxs-lookup"><span data-stu-id="5839b-156">description</span></span>|<span data-ttu-id="5839b-157">String</span><span class="sxs-lookup"><span data-stu-id="5839b-157">String</span></span>|<span data-ttu-id="5839b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5839b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5839b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5839b-160">displayName</span></span>|<span data-ttu-id="5839b-161">String</span><span class="sxs-lookup"><span data-stu-id="5839b-161">String</span></span>|<span data-ttu-id="5839b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5839b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5839b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-164">version</span><span class="sxs-lookup"><span data-stu-id="5839b-164">version</span></span>|<span data-ttu-id="5839b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5839b-165">Int32</span></span>|<span data-ttu-id="5839b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5839b-166">Version of the device configuration.</span></span> <span data-ttu-id="5839b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5839b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5839b-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="5839b-168">connectionName</span></span>|<span data-ttu-id="5839b-169">String</span><span class="sxs-lookup"><span data-stu-id="5839b-169">String</span></span>|<span data-ttu-id="5839b-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="5839b-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="5839b-171">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="5839b-171">connectionType</span></span>|[<span data-ttu-id="5839b-172">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="5839b-172">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="5839b-173">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="5839b-173">Connection type.</span></span> <span data-ttu-id="5839b-174">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="5839b-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="5839b-175">role</span><span class="sxs-lookup"><span data-stu-id="5839b-175">role</span></span>|<span data-ttu-id="5839b-176">String</span><span class="sxs-lookup"><span data-stu-id="5839b-176">String</span></span>|<span data-ttu-id="5839b-177">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="5839b-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="5839b-178">область</span><span class="sxs-lookup"><span data-stu-id="5839b-178">realm</span></span>|<span data-ttu-id="5839b-179">String</span><span class="sxs-lookup"><span data-stu-id="5839b-179">String</span></span>|<span data-ttu-id="5839b-180">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="5839b-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="5839b-181">серверы</span><span class="sxs-lookup"><span data-stu-id="5839b-181">servers</span></span>|<span data-ttu-id="5839b-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5839b-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="5839b-183">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="5839b-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="5839b-184">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="5839b-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="5839b-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5839b-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5839b-186">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="5839b-186">fingerprint</span></span>|<span data-ttu-id="5839b-187">String</span><span class="sxs-lookup"><span data-stu-id="5839b-187">String</span></span>|<span data-ttu-id="5839b-188">Отпечаток является строку, которая будет использоваться для проверки VPN-сервер может быть доверенным, который применяется только для проверки VPN капсула точка — это тип подключения.</span><span class="sxs-lookup"><span data-stu-id="5839b-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="5839b-189">customData</span><span class="sxs-lookup"><span data-stu-id="5839b-189">customData</span></span>|<span data-ttu-id="5839b-190">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5839b-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="5839b-191">Пользовательские данные Citrix задается тип подключения.</span><span class="sxs-lookup"><span data-stu-id="5839b-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="5839b-192">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="5839b-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="5839b-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="5839b-193">customKeyValueData</span></span>|<span data-ttu-id="5839b-194">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5839b-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5839b-195">Пользовательские данные Citrix задается тип подключения.</span><span class="sxs-lookup"><span data-stu-id="5839b-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="5839b-196">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="5839b-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="5839b-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5839b-197">authenticationMethod</span></span>|[<span data-ttu-id="5839b-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5839b-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="5839b-199">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5839b-199">Authentication method.</span></span> <span data-ttu-id="5839b-200">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="5839b-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="5839b-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="5839b-201">Response</span></span>
<span data-ttu-id="5839b-202">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5839b-202">If successful, this method returns a `200 OK` response code and an updated [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5839b-203">Пример</span><span class="sxs-lookup"><span data-stu-id="5839b-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="5839b-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="5839b-204">Request</span></span>
<span data-ttu-id="5839b-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5839b-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 980

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="5839b-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="5839b-206">Response</span></span>
<span data-ttu-id="5839b-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5839b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1157

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```





