---
title: Обновление androidWorkProfileVpnConfiguration
description: Обновление свойства объекта androidWorkProfileVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96b40f2fc9b95bef1c76296adff38c7dd54b6284
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958196"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="ee7f2-103">Обновление androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee7f2-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="ee7f2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee7f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee7f2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee7f2-107">Обновление свойства объекта [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee7f2-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee7f2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee7f2-108">Prerequisites</span></span>
<span data-ttu-id="ee7f2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee7f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee7f2-111">Permission type</span></span>|<span data-ttu-id="ee7f2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee7f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee7f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee7f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee7f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-116">Not supported.</span></span>|
|<span data-ttu-id="ee7f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee7f2-117">Application</span></span>|<span data-ttu-id="ee7f2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee7f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee7f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee7f2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee7f2-120">Request headers</span></span>
|<span data-ttu-id="ee7f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee7f2-121">Header</span></span>|<span data-ttu-id="ee7f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee7f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee7f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee7f2-123">Authorization</span></span>|<span data-ttu-id="ee7f2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ee7f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee7f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee7f2-125">Accept</span></span>|<span data-ttu-id="ee7f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee7f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee7f2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee7f2-127">Request body</span></span>
<span data-ttu-id="ee7f2-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee7f2-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="ee7f2-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="ee7f2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee7f2-130">Property</span></span>|<span data-ttu-id="ee7f2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7f2-131">Type</span></span>|<span data-ttu-id="ee7f2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee7f2-133">id</span><span class="sxs-lookup"><span data-stu-id="ee7f2-133">id</span></span>|<span data-ttu-id="ee7f2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-134">String</span></span>|<span data-ttu-id="ee7f2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-135">Key of the entity.</span></span> <span data-ttu-id="ee7f2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ee7f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7f2-138">DateTimeOffset</span></span>|<span data-ttu-id="ee7f2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ee7f2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee7f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="ee7f2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee7f2-142">String collection</span></span>|<span data-ttu-id="ee7f2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee7f2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ee7f2-145">supportsScopeTags</span></span>|<span data-ttu-id="ee7f2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ee7f2-146">Boolean</span></span>|<span data-ttu-id="ee7f2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee7f2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee7f2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee7f2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-150">This property is read-only.</span></span> <span data-ttu-id="ee7f2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7f2-152">createdDateTime</span></span>|<span data-ttu-id="ee7f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7f2-153">DateTimeOffset</span></span>|<span data-ttu-id="ee7f2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-154">DateTime the object was created.</span></span> <span data-ttu-id="ee7f2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-156">описание</span><span class="sxs-lookup"><span data-stu-id="ee7f2-156">description</span></span>|<span data-ttu-id="ee7f2-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-157">String</span></span>|<span data-ttu-id="ee7f2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee7f2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7f2-160">displayName</span></span>|<span data-ttu-id="ee7f2-161">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-161">String</span></span>|<span data-ttu-id="ee7f2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee7f2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-164">version</span><span class="sxs-lookup"><span data-stu-id="ee7f2-164">version</span></span>|<span data-ttu-id="ee7f2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ee7f2-165">Int32</span></span>|<span data-ttu-id="ee7f2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-166">Version of the device configuration.</span></span> <span data-ttu-id="ee7f2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee7f2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee7f2-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="ee7f2-168">connectionName</span></span>|<span data-ttu-id="ee7f2-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-169">String</span></span>|<span data-ttu-id="ee7f2-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ee7f2-171">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="ee7f2-171">connectionType</span></span>|[<span data-ttu-id="ee7f2-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ee7f2-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="ee7f2-173">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-173">Connection type.</span></span> <span data-ttu-id="ee7f2-174">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="ee7f2-175">role</span><span class="sxs-lookup"><span data-stu-id="ee7f2-175">role</span></span>|<span data-ttu-id="ee7f2-176">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-176">String</span></span>|<span data-ttu-id="ee7f2-177">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ee7f2-178">область</span><span class="sxs-lookup"><span data-stu-id="ee7f2-178">realm</span></span>|<span data-ttu-id="ee7f2-179">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-179">String</span></span>|<span data-ttu-id="ee7f2-180">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ee7f2-181">серверы</span><span class="sxs-lookup"><span data-stu-id="ee7f2-181">servers</span></span>|<span data-ttu-id="ee7f2-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ee7f2-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ee7f2-183">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="ee7f2-184">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ee7f2-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ee7f2-186">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="ee7f2-186">fingerprint</span></span>|<span data-ttu-id="ee7f2-187">Строка</span><span class="sxs-lookup"><span data-stu-id="ee7f2-187">String</span></span>|<span data-ttu-id="ee7f2-188">Отпечаток является строку, которая будет использоваться для проверки VPN-сервер может быть доверенным, который применяется только для проверки VPN капсула точка — это тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ee7f2-189">customData</span><span class="sxs-lookup"><span data-stu-id="ee7f2-189">customData</span></span>|<span data-ttu-id="ee7f2-190">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ee7f2-191">Пользовательские данные Citrix задается тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ee7f2-192">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ee7f2-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ee7f2-193">customKeyValueData</span></span>|<span data-ttu-id="ee7f2-194">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ee7f2-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ee7f2-195">Пользовательские данные Citrix задается тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ee7f2-196">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ee7f2-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ee7f2-197">authenticationMethod</span></span>|[<span data-ttu-id="ee7f2-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ee7f2-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ee7f2-199">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-199">Authentication method.</span></span> <span data-ttu-id="ee7f2-200">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="ee7f2-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee7f2-201">Response</span></span>
<span data-ttu-id="ee7f2-202">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-202">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee7f2-203">Пример</span><span class="sxs-lookup"><span data-stu-id="ee7f2-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee7f2-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee7f2-204">Request</span></span>
<span data-ttu-id="ee7f2-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee7f2-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee7f2-206">Response</span></span>
<span data-ttu-id="ee7f2-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee7f2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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





