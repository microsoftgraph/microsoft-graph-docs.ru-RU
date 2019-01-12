---
title: Создание macOSVpnConfiguration
description: Создание нового объекта macOSVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e72f517296539f0b7f7a388dab315c7e0441fa36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938946"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="f6a93-103">Создание macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f6a93-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="f6a93-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f6a93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6a93-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6a93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6a93-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f6a93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6a93-107">Создание нового объекта [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f6a93-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6a93-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6a93-108">Prerequisites</span></span>
<span data-ttu-id="f6a93-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6a93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6a93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6a93-111">Permission type</span></span>|<span data-ttu-id="f6a93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6a93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6a93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6a93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6a93-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6a93-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6a93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6a93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6a93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6a93-116">Not supported.</span></span>|
|<span data-ttu-id="f6a93-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6a93-117">Application</span></span>|<span data-ttu-id="f6a93-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6a93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6a93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6a93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6a93-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6a93-120">Request headers</span></span>
|<span data-ttu-id="f6a93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6a93-121">Header</span></span>|<span data-ttu-id="f6a93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6a93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6a93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6a93-123">Authorization</span></span>|<span data-ttu-id="f6a93-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f6a93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6a93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6a93-125">Accept</span></span>|<span data-ttu-id="f6a93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6a93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6a93-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6a93-127">Request body</span></span>
<span data-ttu-id="f6a93-128">В тексте запроса укажите представление JSON для объекта macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f6a93-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="f6a93-129">В следующей таблице показаны свойства, которые необходимы для создания macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f6a93-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="f6a93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6a93-130">Property</span></span>|<span data-ttu-id="f6a93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6a93-131">Type</span></span>|<span data-ttu-id="f6a93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6a93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6a93-133">id</span><span class="sxs-lookup"><span data-stu-id="f6a93-133">id</span></span>|<span data-ttu-id="f6a93-134">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-134">String</span></span>|<span data-ttu-id="f6a93-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a93-135">Key of the entity.</span></span> <span data-ttu-id="f6a93-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6a93-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f6a93-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6a93-138">DateTimeOffset</span></span>|<span data-ttu-id="f6a93-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a93-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f6a93-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6a93-141">roleScopeTagIds</span></span>|<span data-ttu-id="f6a93-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f6a93-142">String collection</span></span>|<span data-ttu-id="f6a93-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f6a93-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6a93-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f6a93-145">supportsScopeTags</span></span>|<span data-ttu-id="f6a93-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6a93-146">Boolean</span></span>|<span data-ttu-id="f6a93-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f6a93-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f6a93-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f6a93-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f6a93-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f6a93-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f6a93-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6a93-150">This property is read-only.</span></span> <span data-ttu-id="f6a93-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6a93-152">createdDateTime</span></span>|<span data-ttu-id="f6a93-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6a93-153">DateTimeOffset</span></span>|<span data-ttu-id="f6a93-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a93-154">DateTime the object was created.</span></span> <span data-ttu-id="f6a93-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-156">описание</span><span class="sxs-lookup"><span data-stu-id="f6a93-156">description</span></span>|<span data-ttu-id="f6a93-157">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-157">String</span></span>|<span data-ttu-id="f6a93-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6a93-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6a93-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f6a93-160">displayName</span></span>|<span data-ttu-id="f6a93-161">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-161">String</span></span>|<span data-ttu-id="f6a93-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6a93-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6a93-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-164">version</span><span class="sxs-lookup"><span data-stu-id="f6a93-164">version</span></span>|<span data-ttu-id="f6a93-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f6a93-165">Int32</span></span>|<span data-ttu-id="f6a93-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6a93-166">Version of the device configuration.</span></span> <span data-ttu-id="f6a93-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f6a93-168">connectionName</span></span>|<span data-ttu-id="f6a93-169">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-169">String</span></span>|<span data-ttu-id="f6a93-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6a93-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f6a93-171">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-172">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="f6a93-172">connectionType</span></span>|[<span data-ttu-id="f6a93-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f6a93-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f6a93-174">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f6a93-174">Connection type.</span></span> <span data-ttu-id="f6a93-175">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f6a93-176">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="f6a93-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="f6a93-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f6a93-177">loginGroupOrDomain</span></span>|<span data-ttu-id="f6a93-178">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-178">String</span></span>|<span data-ttu-id="f6a93-179">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="f6a93-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f6a93-180">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-181">role</span><span class="sxs-lookup"><span data-stu-id="f6a93-181">role</span></span>|<span data-ttu-id="f6a93-182">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-182">String</span></span>|<span data-ttu-id="f6a93-183">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="f6a93-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f6a93-184">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-185">область</span><span class="sxs-lookup"><span data-stu-id="f6a93-185">realm</span></span>|<span data-ttu-id="f6a93-186">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-186">String</span></span>|<span data-ttu-id="f6a93-187">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="f6a93-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f6a93-188">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-189">сервер</span><span class="sxs-lookup"><span data-stu-id="f6a93-189">server</span></span>|[<span data-ttu-id="f6a93-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f6a93-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f6a93-191">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="f6a93-191">VPN Server on the network.</span></span> <span data-ttu-id="f6a93-192">Убедитесь, что конечные пользователи могут получить доступ к этой сетевой папке.</span><span class="sxs-lookup"><span data-stu-id="f6a93-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="f6a93-193">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-194">идентификатор</span><span class="sxs-lookup"><span data-stu-id="f6a93-194">identifier</span></span>|<span data-ttu-id="f6a93-195">String</span><span class="sxs-lookup"><span data-stu-id="f6a93-195">String</span></span>|<span data-ttu-id="f6a93-196">Идентификатор предоставлена поставщиком VPN, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="f6a93-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f6a93-197">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-198">customData</span><span class="sxs-lookup"><span data-stu-id="f6a93-198">customData</span></span>|<span data-ttu-id="f6a93-199">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f6a93-200">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="f6a93-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f6a93-201">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="f6a93-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f6a93-202">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="f6a93-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f6a93-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f6a93-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f6a93-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f6a93-205">customKeyValueData</span></span>|<span data-ttu-id="f6a93-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f6a93-207">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="f6a93-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f6a93-208">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="f6a93-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f6a93-209">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="f6a93-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f6a93-210">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f6a93-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f6a93-211">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f6a93-212">enableSplitTunneling</span></span>|<span data-ttu-id="f6a93-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6a93-213">Boolean</span></span>|<span data-ttu-id="f6a93-214">Отправьте все сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="f6a93-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="f6a93-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f6a93-216">authenticationMethod</span></span>|[<span data-ttu-id="f6a93-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f6a93-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f6a93-218">Метод проверки подлинности для VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="f6a93-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f6a93-219">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a93-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f6a93-220">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f6a93-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f6a93-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f6a93-221">enablePerApp</span></span>|<span data-ttu-id="f6a93-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6a93-222">Boolean</span></span>|<span data-ttu-id="f6a93-223">Установка значения true создает полезных данных VPN-App, который позднее можно сопоставить с приложениями, которые может активировать этот conneciton VPN на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6a93-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f6a93-224">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f6a93-225">safariDomains</span></span>|<span data-ttu-id="f6a93-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f6a93-226">String collection</span></span>|<span data-ttu-id="f6a93-227">Safari доменов, при включении VPN каждого параметра приложения.</span><span class="sxs-lookup"><span data-stu-id="f6a93-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f6a93-228">В дополнение к приложений, связанных с этой виртуальной частной сети Safari домены указанного здесь также будет иметь для запуска этой VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f6a93-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f6a93-229">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f6a93-230">onDemandRules</span></span>|<span data-ttu-id="f6a93-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f6a93-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f6a93-232">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="f6a93-232">On-Demand Rules.</span></span> <span data-ttu-id="f6a93-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f6a93-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f6a93-234">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-235">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="f6a93-235">proxyServer</span></span>|[<span data-ttu-id="f6a93-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f6a93-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f6a93-237">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f6a93-237">Proxy Server.</span></span> <span data-ttu-id="f6a93-238">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f6a93-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f6a93-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f6a93-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6a93-240">Boolean</span></span>|<span data-ttu-id="f6a93-241">Явного согласия пользователя к совместному использованию кода устройства сторонних производителей VPN-клиентов для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="f6a93-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f6a93-242">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a93-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f6a93-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6a93-243">Response</span></span>
<span data-ttu-id="f6a93-244">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f6a93-244">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6a93-245">Пример</span><span class="sxs-lookup"><span data-stu-id="f6a93-245">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6a93-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6a93-246">Request</span></span>
<span data-ttu-id="f6a93-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6a93-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1921

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="f6a93-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6a93-248">Response</span></span>
<span data-ttu-id="f6a93-p127">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f6a93-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "optInToDeviceIdSharing": true
}
```





