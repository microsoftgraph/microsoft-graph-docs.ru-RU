---
title: Создание iosVpnConfiguration
description: Создание нового объекта iosVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9276c36cdc281c7b535ef71e97a407b7848655ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819128"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="36dcd-103">Создание iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="36dcd-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="36dcd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36dcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36dcd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dcd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36dcd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36dcd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36dcd-107">Создание нового объекта [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="36dcd-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36dcd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36dcd-108">Prerequisites</span></span>
<span data-ttu-id="36dcd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36dcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36dcd-111">Permission type</span></span>|<span data-ttu-id="36dcd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36dcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36dcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36dcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36dcd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36dcd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36dcd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36dcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dcd-116">Not supported.</span></span>|
|<span data-ttu-id="36dcd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36dcd-117">Application</span></span>|<span data-ttu-id="36dcd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dcd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36dcd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36dcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36dcd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36dcd-120">Request headers</span></span>
|<span data-ttu-id="36dcd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36dcd-121">Header</span></span>|<span data-ttu-id="36dcd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36dcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36dcd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36dcd-123">Authorization</span></span>|<span data-ttu-id="36dcd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="36dcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36dcd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36dcd-125">Accept</span></span>|<span data-ttu-id="36dcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36dcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36dcd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36dcd-127">Request body</span></span>
<span data-ttu-id="36dcd-128">В тексте запроса укажите представление JSON для объекта iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="36dcd-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="36dcd-129">В следующей таблице показаны свойства, которые необходимы для создания iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="36dcd-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="36dcd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36dcd-130">Property</span></span>|<span data-ttu-id="36dcd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36dcd-131">Type</span></span>|<span data-ttu-id="36dcd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36dcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36dcd-133">id</span><span class="sxs-lookup"><span data-stu-id="36dcd-133">id</span></span>|<span data-ttu-id="36dcd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-134">String</span></span>|<span data-ttu-id="36dcd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="36dcd-135">Key of the entity.</span></span> <span data-ttu-id="36dcd-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36dcd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="36dcd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36dcd-138">DateTimeOffset</span></span>|<span data-ttu-id="36dcd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="36dcd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="36dcd-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36dcd-141">roleScopeTagIds</span></span>|<span data-ttu-id="36dcd-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="36dcd-142">String collection</span></span>|<span data-ttu-id="36dcd-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="36dcd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36dcd-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36dcd-145">supportsScopeTags</span></span>|<span data-ttu-id="36dcd-146">Логический</span><span class="sxs-lookup"><span data-stu-id="36dcd-146">Boolean</span></span>|<span data-ttu-id="36dcd-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="36dcd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36dcd-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="36dcd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36dcd-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="36dcd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36dcd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36dcd-150">This property is read-only.</span></span> <span data-ttu-id="36dcd-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36dcd-152">createdDateTime</span></span>|<span data-ttu-id="36dcd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36dcd-153">DateTimeOffset</span></span>|<span data-ttu-id="36dcd-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="36dcd-154">DateTime the object was created.</span></span> <span data-ttu-id="36dcd-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-156">описание</span><span class="sxs-lookup"><span data-stu-id="36dcd-156">description</span></span>|<span data-ttu-id="36dcd-157">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-157">String</span></span>|<span data-ttu-id="36dcd-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36dcd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36dcd-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="36dcd-160">displayName</span></span>|<span data-ttu-id="36dcd-161">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-161">String</span></span>|<span data-ttu-id="36dcd-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36dcd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36dcd-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-164">version</span><span class="sxs-lookup"><span data-stu-id="36dcd-164">version</span></span>|<span data-ttu-id="36dcd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="36dcd-165">Int32</span></span>|<span data-ttu-id="36dcd-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36dcd-166">Version of the device configuration.</span></span> <span data-ttu-id="36dcd-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="36dcd-168">connectionName</span></span>|<span data-ttu-id="36dcd-169">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-169">String</span></span>|<span data-ttu-id="36dcd-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="36dcd-170">Connection name displayed to the user.</span></span> <span data-ttu-id="36dcd-171">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-172">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="36dcd-172">connectionType</span></span>|[<span data-ttu-id="36dcd-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="36dcd-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="36dcd-174">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="36dcd-174">Connection type.</span></span> <span data-ttu-id="36dcd-175">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="36dcd-176">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="36dcd-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="36dcd-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="36dcd-177">loginGroupOrDomain</span></span>|<span data-ttu-id="36dcd-178">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-178">String</span></span>|<span data-ttu-id="36dcd-179">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="36dcd-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="36dcd-180">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-181">role</span><span class="sxs-lookup"><span data-stu-id="36dcd-181">role</span></span>|<span data-ttu-id="36dcd-182">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-182">String</span></span>|<span data-ttu-id="36dcd-183">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="36dcd-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="36dcd-184">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-185">область</span><span class="sxs-lookup"><span data-stu-id="36dcd-185">realm</span></span>|<span data-ttu-id="36dcd-186">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-186">String</span></span>|<span data-ttu-id="36dcd-187">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="36dcd-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="36dcd-188">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-189">сервер</span><span class="sxs-lookup"><span data-stu-id="36dcd-189">server</span></span>|[<span data-ttu-id="36dcd-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="36dcd-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="36dcd-191">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="36dcd-191">VPN Server on the network.</span></span> <span data-ttu-id="36dcd-192">Убедитесь, что конечные пользователи могут получить доступ к этой сетевой папке.</span><span class="sxs-lookup"><span data-stu-id="36dcd-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="36dcd-193">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-194">идентификатор</span><span class="sxs-lookup"><span data-stu-id="36dcd-194">identifier</span></span>|<span data-ttu-id="36dcd-195">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-195">String</span></span>|<span data-ttu-id="36dcd-196">Идентификатор предоставлена поставщиком VPN, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="36dcd-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="36dcd-197">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-198">customData</span><span class="sxs-lookup"><span data-stu-id="36dcd-198">customData</span></span>|<span data-ttu-id="36dcd-199">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="36dcd-200">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="36dcd-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="36dcd-201">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="36dcd-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="36dcd-202">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="36dcd-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="36dcd-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="36dcd-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="36dcd-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="36dcd-205">customKeyValueData</span></span>|<span data-ttu-id="36dcd-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="36dcd-207">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="36dcd-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="36dcd-208">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="36dcd-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="36dcd-209">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="36dcd-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="36dcd-210">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="36dcd-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="36dcd-211">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="36dcd-212">enableSplitTunneling</span></span>|<span data-ttu-id="36dcd-213">Логический</span><span class="sxs-lookup"><span data-stu-id="36dcd-213">Boolean</span></span>|<span data-ttu-id="36dcd-214">Отправьте все сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="36dcd-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="36dcd-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="36dcd-216">authenticationMethod</span></span>|[<span data-ttu-id="36dcd-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="36dcd-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="36dcd-218">Метод проверки подлинности для VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="36dcd-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="36dcd-219">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36dcd-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="36dcd-220">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="36dcd-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="36dcd-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="36dcd-221">enablePerApp</span></span>|<span data-ttu-id="36dcd-222">Логический</span><span class="sxs-lookup"><span data-stu-id="36dcd-222">Boolean</span></span>|<span data-ttu-id="36dcd-223">Установка значения true создает полезных данных VPN-App, который позднее можно сопоставить с приложениями, которые может активировать этот conneciton VPN на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="36dcd-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="36dcd-224">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="36dcd-225">safariDomains</span></span>|<span data-ttu-id="36dcd-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="36dcd-226">String collection</span></span>|<span data-ttu-id="36dcd-227">Safari доменов, при включении VPN каждого параметра приложения.</span><span class="sxs-lookup"><span data-stu-id="36dcd-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="36dcd-228">В дополнение к приложений, связанных с этой виртуальной частной сети Safari домены указанного здесь также будет иметь для запуска этой VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="36dcd-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="36dcd-229">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="36dcd-230">onDemandRules</span></span>|<span data-ttu-id="36dcd-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="36dcd-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="36dcd-232">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="36dcd-232">On-Demand Rules.</span></span> <span data-ttu-id="36dcd-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="36dcd-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="36dcd-234">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-235">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="36dcd-235">proxyServer</span></span>|[<span data-ttu-id="36dcd-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="36dcd-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="36dcd-237">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="36dcd-237">Proxy Server.</span></span> <span data-ttu-id="36dcd-238">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="36dcd-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="36dcd-240">Логический</span><span class="sxs-lookup"><span data-stu-id="36dcd-240">Boolean</span></span>|<span data-ttu-id="36dcd-241">Явного согласия пользователя к совместному использованию кода устройства сторонних производителей VPN-клиентов для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="36dcd-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="36dcd-242">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36dcd-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="36dcd-243">providerType</span><span class="sxs-lookup"><span data-stu-id="36dcd-243">providerType</span></span>|[<span data-ttu-id="36dcd-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="36dcd-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="36dcd-245">Тип поставщика для VPN-app.</span><span class="sxs-lookup"><span data-stu-id="36dcd-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="36dcd-246">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="36dcd-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="36dcd-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="36dcd-247">userDomain</span></span>|<span data-ttu-id="36dcd-248">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-248">String</span></span>|<span data-ttu-id="36dcd-249">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="36dcd-249">Zscaler only.</span></span> <span data-ttu-id="36dcd-250">Введите статический домена для предварительного заполнения полей для входа с в приложении Zscaler.</span><span class="sxs-lookup"><span data-stu-id="36dcd-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="36dcd-251">Если оставлено пустым, будет использоваться Azure Active Directory пользователя домена.</span><span class="sxs-lookup"><span data-stu-id="36dcd-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="36dcd-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="36dcd-252">strictEnforcement</span></span>|<span data-ttu-id="36dcd-253">Логический</span><span class="sxs-lookup"><span data-stu-id="36dcd-253">Boolean</span></span>|<span data-ttu-id="36dcd-254">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="36dcd-254">Zscaler only.</span></span> <span data-ttu-id="36dcd-255">Блокирует сетевой трафик до пользователь входит в Zscaler приложения.</span><span class="sxs-lookup"><span data-stu-id="36dcd-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="36dcd-256">Значение «true» означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="36dcd-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="36dcd-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="36dcd-257">cloudName</span></span>|<span data-ttu-id="36dcd-258">Строка</span><span class="sxs-lookup"><span data-stu-id="36dcd-258">String</span></span>|<span data-ttu-id="36dcd-259">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="36dcd-259">Zscaler only.</span></span> <span data-ttu-id="36dcd-260">Облако Zscaler, которое назначается пользователя.</span><span class="sxs-lookup"><span data-stu-id="36dcd-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="36dcd-261">список исключений</span><span class="sxs-lookup"><span data-stu-id="36dcd-261">excludeList</span></span>|<span data-ttu-id="36dcd-262">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="36dcd-262">String collection</span></span>|<span data-ttu-id="36dcd-263">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="36dcd-263">Zscaler only.</span></span> <span data-ttu-id="36dcd-264">Список сетевых адресов, которые не передаются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="36dcd-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="36dcd-265">Ответ</span><span class="sxs-lookup"><span data-stu-id="36dcd-265">Response</span></span>
<span data-ttu-id="36dcd-266">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36dcd-266">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36dcd-267">Пример</span><span class="sxs-lookup"><span data-stu-id="36dcd-267">Example</span></span>
### <a name="request"></a><span data-ttu-id="36dcd-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="36dcd-268">Request</span></span>
<span data-ttu-id="36dcd-269">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36dcd-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2106

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="36dcd-270">Ответ</span><span class="sxs-lookup"><span data-stu-id="36dcd-270">Response</span></span>
<span data-ttu-id="36dcd-p132">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="36dcd-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





