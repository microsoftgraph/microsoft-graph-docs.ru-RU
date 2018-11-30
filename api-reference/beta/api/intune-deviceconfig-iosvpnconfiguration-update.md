---
title: Обновление iosVpnConfiguration
description: Обновление свойства объекта iosVpnConfiguration.
ms.openlocfilehash: b5cf6b9fd40ee31c9136dc4e09f467a2e201dabc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076338"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="fc560-103">Обновление iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc560-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="fc560-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc560-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc560-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc560-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc560-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc560-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc560-107">Обновление свойства объекта [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fc560-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc560-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc560-108">Prerequisites</span></span>
<span data-ttu-id="fc560-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc560-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc560-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc560-111">Permission type</span></span>|<span data-ttu-id="fc560-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc560-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc560-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc560-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc560-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc560-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc560-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc560-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc560-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc560-116">Not supported.</span></span>|
|<span data-ttu-id="fc560-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc560-117">Application</span></span>|<span data-ttu-id="fc560-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc560-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc560-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc560-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fc560-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc560-120">Request headers</span></span>
|<span data-ttu-id="fc560-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc560-121">Header</span></span>|<span data-ttu-id="fc560-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc560-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc560-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc560-123">Authorization</span></span>|<span data-ttu-id="fc560-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fc560-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc560-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc560-125">Accept</span></span>|<span data-ttu-id="fc560-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc560-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc560-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc560-127">Request body</span></span>
<span data-ttu-id="fc560-128">В тексте запроса укажите представление JSON для объекта [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fc560-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="fc560-129">В следующей таблице показаны свойства, которые необходимы для создания [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="fc560-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc560-130">Property</span></span>|<span data-ttu-id="fc560-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fc560-131">Type</span></span>|<span data-ttu-id="fc560-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fc560-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc560-133">id</span><span class="sxs-lookup"><span data-stu-id="fc560-133">id</span></span>|<span data-ttu-id="fc560-134">String</span><span class="sxs-lookup"><span data-stu-id="fc560-134">String</span></span>|<span data-ttu-id="fc560-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc560-135">Key of the entity.</span></span> <span data-ttu-id="fc560-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc560-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fc560-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc560-138">DateTimeOffset</span></span>|<span data-ttu-id="fc560-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc560-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fc560-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc560-141">roleScopeTagIds</span></span>|<span data-ttu-id="fc560-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc560-142">String collection</span></span>|<span data-ttu-id="fc560-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fc560-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fc560-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fc560-145">supportsScopeTags</span></span>|<span data-ttu-id="fc560-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fc560-146">Boolean</span></span>|<span data-ttu-id="fc560-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fc560-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fc560-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fc560-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fc560-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fc560-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fc560-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc560-150">This property is read-only.</span></span> <span data-ttu-id="fc560-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc560-152">createdDateTime</span></span>|<span data-ttu-id="fc560-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc560-153">DateTimeOffset</span></span>|<span data-ttu-id="fc560-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fc560-154">DateTime the object was created.</span></span> <span data-ttu-id="fc560-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-156">описание</span><span class="sxs-lookup"><span data-stu-id="fc560-156">description</span></span>|<span data-ttu-id="fc560-157">String</span><span class="sxs-lookup"><span data-stu-id="fc560-157">String</span></span>|<span data-ttu-id="fc560-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc560-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc560-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fc560-160">displayName</span></span>|<span data-ttu-id="fc560-161">String</span><span class="sxs-lookup"><span data-stu-id="fc560-161">String</span></span>|<span data-ttu-id="fc560-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc560-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc560-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-164">version</span><span class="sxs-lookup"><span data-stu-id="fc560-164">version</span></span>|<span data-ttu-id="fc560-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fc560-165">Int32</span></span>|<span data-ttu-id="fc560-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc560-166">Version of the device configuration.</span></span> <span data-ttu-id="fc560-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="fc560-168">connectionName</span></span>|<span data-ttu-id="fc560-169">String</span><span class="sxs-lookup"><span data-stu-id="fc560-169">String</span></span>|<span data-ttu-id="fc560-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc560-170">Connection name displayed to the user.</span></span> <span data-ttu-id="fc560-171">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-172">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="fc560-172">connectionType</span></span>|[<span data-ttu-id="fc560-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="fc560-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="fc560-174">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="fc560-174">Connection type.</span></span> <span data-ttu-id="fc560-175">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="fc560-176">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="fc560-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="fc560-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="fc560-177">loginGroupOrDomain</span></span>|<span data-ttu-id="fc560-178">String</span><span class="sxs-lookup"><span data-stu-id="fc560-178">String</span></span>|<span data-ttu-id="fc560-179">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="fc560-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="fc560-180">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-181">role</span><span class="sxs-lookup"><span data-stu-id="fc560-181">role</span></span>|<span data-ttu-id="fc560-182">String</span><span class="sxs-lookup"><span data-stu-id="fc560-182">String</span></span>|<span data-ttu-id="fc560-183">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="fc560-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="fc560-184">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-185">область</span><span class="sxs-lookup"><span data-stu-id="fc560-185">realm</span></span>|<span data-ttu-id="fc560-186">String</span><span class="sxs-lookup"><span data-stu-id="fc560-186">String</span></span>|<span data-ttu-id="fc560-187">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="fc560-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="fc560-188">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-189">сервер</span><span class="sxs-lookup"><span data-stu-id="fc560-189">server</span></span>|[<span data-ttu-id="fc560-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="fc560-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="fc560-191">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="fc560-191">VPN Server on the network.</span></span> <span data-ttu-id="fc560-192">Убедитесь, что конечные пользователи могут получить доступ к этой сетевой папке.</span><span class="sxs-lookup"><span data-stu-id="fc560-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="fc560-193">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-194">идентификатор</span><span class="sxs-lookup"><span data-stu-id="fc560-194">identifier</span></span>|<span data-ttu-id="fc560-195">String</span><span class="sxs-lookup"><span data-stu-id="fc560-195">String</span></span>|<span data-ttu-id="fc560-196">Идентификатор предоставлена поставщиком VPN, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="fc560-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="fc560-197">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-198">customData</span><span class="sxs-lookup"><span data-stu-id="fc560-198">customData</span></span>|<span data-ttu-id="fc560-199">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="fc560-200">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="fc560-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="fc560-201">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="fc560-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="fc560-202">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="fc560-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="fc560-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc560-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="fc560-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="fc560-205">customKeyValueData</span></span>|<span data-ttu-id="fc560-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fc560-207">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="fc560-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="fc560-208">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="fc560-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="fc560-209">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="fc560-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="fc560-210">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc560-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="fc560-211">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="fc560-212">enableSplitTunneling</span></span>|<span data-ttu-id="fc560-213">Логический</span><span class="sxs-lookup"><span data-stu-id="fc560-213">Boolean</span></span>|<span data-ttu-id="fc560-214">Отправьте все сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="fc560-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="fc560-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fc560-216">authenticationMethod</span></span>|[<span data-ttu-id="fc560-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fc560-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="fc560-218">Метод проверки подлинности для VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="fc560-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="fc560-219">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc560-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="fc560-220">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="fc560-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="fc560-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="fc560-221">enablePerApp</span></span>|<span data-ttu-id="fc560-222">Логический</span><span class="sxs-lookup"><span data-stu-id="fc560-222">Boolean</span></span>|<span data-ttu-id="fc560-223">Установка значения true создает полезных данных VPN-App, который позднее можно сопоставить с приложениями, которые может активировать этот conneciton VPN на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc560-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="fc560-224">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="fc560-225">safariDomains</span></span>|<span data-ttu-id="fc560-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc560-226">String collection</span></span>|<span data-ttu-id="fc560-227">Safari доменов, при включении VPN каждого параметра приложения.</span><span class="sxs-lookup"><span data-stu-id="fc560-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="fc560-228">В дополнение к приложений, связанных с этой виртуальной частной сети Safari домены указанного здесь также будет иметь для запуска этой VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="fc560-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="fc560-229">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="fc560-230">onDemandRules</span></span>|<span data-ttu-id="fc560-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fc560-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="fc560-232">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="fc560-232">On-Demand Rules.</span></span> <span data-ttu-id="fc560-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc560-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fc560-234">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-235">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="fc560-235">proxyServer</span></span>|[<span data-ttu-id="fc560-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="fc560-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="fc560-237">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="fc560-237">Proxy Server.</span></span> <span data-ttu-id="fc560-238">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="fc560-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="fc560-240">Логический</span><span class="sxs-lookup"><span data-stu-id="fc560-240">Boolean</span></span>|<span data-ttu-id="fc560-241">Явного согласия пользователя к совместному использованию кода устройства сторонних производителей VPN-клиентов для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="fc560-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="fc560-242">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc560-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc560-243">providerType</span><span class="sxs-lookup"><span data-stu-id="fc560-243">providerType</span></span>|[<span data-ttu-id="fc560-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="fc560-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="fc560-245">Тип поставщика для VPN-app.</span><span class="sxs-lookup"><span data-stu-id="fc560-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="fc560-246">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="fc560-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="fc560-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="fc560-247">userDomain</span></span>|<span data-ttu-id="fc560-248">String</span><span class="sxs-lookup"><span data-stu-id="fc560-248">String</span></span>|<span data-ttu-id="fc560-249">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="fc560-249">Zscaler only.</span></span> <span data-ttu-id="fc560-250">Введите статический домена для предварительного заполнения полей для входа с в приложении Zscaler.</span><span class="sxs-lookup"><span data-stu-id="fc560-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="fc560-251">Если оставлено пустым, будет использоваться Azure Active Directory пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="fc560-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="fc560-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="fc560-252">strictEnforcement</span></span>|<span data-ttu-id="fc560-253">Логический</span><span class="sxs-lookup"><span data-stu-id="fc560-253">Boolean</span></span>|<span data-ttu-id="fc560-254">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="fc560-254">Zscaler only.</span></span> <span data-ttu-id="fc560-255">Блокирует сетевой трафик до пользователь входит в Zscaler приложения.</span><span class="sxs-lookup"><span data-stu-id="fc560-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="fc560-256">Значение «true» означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="fc560-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="fc560-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="fc560-257">cloudName</span></span>|<span data-ttu-id="fc560-258">String</span><span class="sxs-lookup"><span data-stu-id="fc560-258">String</span></span>|<span data-ttu-id="fc560-259">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="fc560-259">Zscaler only.</span></span> <span data-ttu-id="fc560-260">Облако Zscaler, которое назначается пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc560-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="fc560-261">список исключений</span><span class="sxs-lookup"><span data-stu-id="fc560-261">excludeList</span></span>|<span data-ttu-id="fc560-262">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc560-262">String collection</span></span>|<span data-ttu-id="fc560-263">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="fc560-263">Zscaler only.</span></span> <span data-ttu-id="fc560-264">Список сетевых адресов, которые не передаются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="fc560-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="fc560-265">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc560-265">Response</span></span>
<span data-ttu-id="fc560-266">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fc560-266">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc560-267">Пример</span><span class="sxs-lookup"><span data-stu-id="fc560-267">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc560-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc560-268">Request</span></span>
<span data-ttu-id="fc560-269">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc560-269">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2048

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
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fc560-270">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc560-270">Response</span></span>
<span data-ttu-id="fc560-p132">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fc560-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```





