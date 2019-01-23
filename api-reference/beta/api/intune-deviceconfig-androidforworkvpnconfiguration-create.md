---
title: Создание androidForWorkVpnConfiguration
description: Создание нового объекта androidForWorkVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 88ed4fd8b9f7e0ad134318614b0d8bd160c4b4b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408917"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="c9c81-103">Создание androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9c81-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="c9c81-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9c81-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9c81-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9c81-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9c81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9c81-107">Создание нового объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c9c81-107">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9c81-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c9c81-108">Prerequisites</span></span>
<span data-ttu-id="c9c81-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9c81-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c81-111">Permission type</span></span>|<span data-ttu-id="c9c81-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9c81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9c81-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9c81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9c81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9c81-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9c81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9c81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c81-116">Not supported.</span></span>|
|<span data-ttu-id="c9c81-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9c81-117">Application</span></span>|<span data-ttu-id="c9c81-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9c81-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9c81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c9c81-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9c81-120">Request headers</span></span>
|<span data-ttu-id="c9c81-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9c81-121">Header</span></span>|<span data-ttu-id="c9c81-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9c81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9c81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9c81-123">Authorization</span></span>|<span data-ttu-id="c9c81-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c9c81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9c81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9c81-125">Accept</span></span>|<span data-ttu-id="c9c81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9c81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9c81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9c81-127">Request body</span></span>
<span data-ttu-id="c9c81-128">В тексте запроса укажите представление JSON для объекта androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c9c81-128">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="c9c81-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c9c81-129">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="c9c81-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9c81-130">Property</span></span>|<span data-ttu-id="c9c81-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9c81-131">Type</span></span>|<span data-ttu-id="c9c81-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9c81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9c81-133">id</span><span class="sxs-lookup"><span data-stu-id="c9c81-133">id</span></span>|<span data-ttu-id="c9c81-134">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-134">String</span></span>|<span data-ttu-id="c9c81-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9c81-135">Key of the entity.</span></span> <span data-ttu-id="c9c81-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c81-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c9c81-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c81-138">DateTimeOffset</span></span>|<span data-ttu-id="c9c81-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c9c81-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c9c81-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9c81-141">roleScopeTagIds</span></span>|<span data-ttu-id="c9c81-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c9c81-142">String collection</span></span>|<span data-ttu-id="c9c81-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c9c81-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9c81-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9c81-145">supportsScopeTags</span></span>|<span data-ttu-id="c9c81-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c9c81-146">Boolean</span></span>|<span data-ttu-id="c9c81-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c9c81-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9c81-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c9c81-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9c81-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c9c81-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9c81-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9c81-150">This property is read-only.</span></span> <span data-ttu-id="c9c81-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c81-152">createdDateTime</span></span>|<span data-ttu-id="c9c81-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c81-153">DateTimeOffset</span></span>|<span data-ttu-id="c9c81-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c9c81-154">DateTime the object was created.</span></span> <span data-ttu-id="c9c81-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-156">description</span><span class="sxs-lookup"><span data-stu-id="c9c81-156">description</span></span>|<span data-ttu-id="c9c81-157">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-157">String</span></span>|<span data-ttu-id="c9c81-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9c81-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9c81-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c9c81-160">displayName</span></span>|<span data-ttu-id="c9c81-161">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-161">String</span></span>|<span data-ttu-id="c9c81-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9c81-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9c81-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-164">version</span><span class="sxs-lookup"><span data-stu-id="c9c81-164">version</span></span>|<span data-ttu-id="c9c81-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c81-165">Int32</span></span>|<span data-ttu-id="c9c81-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9c81-166">Version of the device configuration.</span></span> <span data-ttu-id="c9c81-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9c81-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c81-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="c9c81-168">connectionName</span></span>|<span data-ttu-id="c9c81-169">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-169">String</span></span>|<span data-ttu-id="c9c81-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c9c81-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="c9c81-171">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="c9c81-171">connectionType</span></span>|[<span data-ttu-id="c9c81-172">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c9c81-172">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="c9c81-173">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c9c81-173">Connection type.</span></span> <span data-ttu-id="c9c81-174">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="c9c81-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="c9c81-175">role</span><span class="sxs-lookup"><span data-stu-id="c9c81-175">role</span></span>|<span data-ttu-id="c9c81-176">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-176">String</span></span>|<span data-ttu-id="c9c81-177">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="c9c81-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c9c81-178">область</span><span class="sxs-lookup"><span data-stu-id="c9c81-178">realm</span></span>|<span data-ttu-id="c9c81-179">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-179">String</span></span>|<span data-ttu-id="c9c81-180">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="c9c81-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c9c81-181">серверы</span><span class="sxs-lookup"><span data-stu-id="c9c81-181">servers</span></span>|<span data-ttu-id="c9c81-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c9c81-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c9c81-183">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="c9c81-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="c9c81-184">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="c9c81-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c9c81-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c9c81-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c9c81-186">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="c9c81-186">fingerprint</span></span>|<span data-ttu-id="c9c81-187">String</span><span class="sxs-lookup"><span data-stu-id="c9c81-187">String</span></span>|<span data-ttu-id="c9c81-188">Отпечаток является строку, которая будет использоваться для проверки VPN-сервер может быть доверенным, который применяется только для проверки VPN капсула точка — это тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c9c81-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="c9c81-189">customData</span><span class="sxs-lookup"><span data-stu-id="c9c81-189">customData</span></span>|<span data-ttu-id="c9c81-190">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c9c81-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c9c81-191">Пользовательские данные Citrix задается тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c9c81-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="c9c81-192">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="c9c81-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c9c81-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c9c81-193">customKeyValueData</span></span>|<span data-ttu-id="c9c81-194">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c9c81-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c9c81-195">Пользовательские данные Citrix задается тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c9c81-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="c9c81-196">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="c9c81-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c9c81-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c9c81-197">authenticationMethod</span></span>|[<span data-ttu-id="c9c81-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c9c81-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c9c81-199">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c9c81-199">Authentication method.</span></span> <span data-ttu-id="c9c81-200">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c9c81-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="c9c81-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c81-201">Response</span></span>
<span data-ttu-id="c9c81-202">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9c81-202">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9c81-203">Пример</span><span class="sxs-lookup"><span data-stu-id="c9c81-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9c81-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9c81-204">Request</span></span>
<span data-ttu-id="c9c81-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9c81-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 985

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="c9c81-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c81-206">Response</span></span>
<span data-ttu-id="c9c81-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c9c81-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




