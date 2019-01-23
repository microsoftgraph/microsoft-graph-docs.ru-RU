---
title: Обновление macOSVpnConfiguration
description: Обновление свойства объекта macOSVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9836800e9a04e8137a746d9bc639dfc8b461d9c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399383"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="f08dc-103">Обновление macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f08dc-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="f08dc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f08dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f08dc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f08dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f08dc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f08dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f08dc-107">Обновление свойства объекта [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f08dc-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f08dc-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f08dc-108">Prerequisites</span></span>
<span data-ttu-id="f08dc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f08dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f08dc-111">Permission type</span></span>|<span data-ttu-id="f08dc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f08dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f08dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f08dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f08dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f08dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f08dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f08dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f08dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f08dc-116">Not supported.</span></span>|
|<span data-ttu-id="f08dc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f08dc-117">Application</span></span>|<span data-ttu-id="f08dc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f08dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f08dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f08dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f08dc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f08dc-120">Request headers</span></span>
|<span data-ttu-id="f08dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f08dc-121">Header</span></span>|<span data-ttu-id="f08dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f08dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f08dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f08dc-123">Authorization</span></span>|<span data-ttu-id="f08dc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f08dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f08dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f08dc-125">Accept</span></span>|<span data-ttu-id="f08dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f08dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f08dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f08dc-127">Request body</span></span>
<span data-ttu-id="f08dc-128">В тексте запроса укажите представление JSON для объекта [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f08dc-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="f08dc-129">В следующей таблице показаны свойства, которые необходимы для создания [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="f08dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f08dc-130">Property</span></span>|<span data-ttu-id="f08dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f08dc-131">Type</span></span>|<span data-ttu-id="f08dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f08dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f08dc-133">id</span><span class="sxs-lookup"><span data-stu-id="f08dc-133">id</span></span>|<span data-ttu-id="f08dc-134">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-134">String</span></span>|<span data-ttu-id="f08dc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f08dc-135">Key of the entity.</span></span> <span data-ttu-id="f08dc-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f08dc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f08dc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f08dc-138">DateTimeOffset</span></span>|<span data-ttu-id="f08dc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f08dc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f08dc-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f08dc-141">roleScopeTagIds</span></span>|<span data-ttu-id="f08dc-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f08dc-142">String collection</span></span>|<span data-ttu-id="f08dc-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f08dc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f08dc-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f08dc-145">supportsScopeTags</span></span>|<span data-ttu-id="f08dc-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f08dc-146">Boolean</span></span>|<span data-ttu-id="f08dc-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f08dc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f08dc-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f08dc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f08dc-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f08dc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f08dc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f08dc-150">This property is read-only.</span></span> <span data-ttu-id="f08dc-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f08dc-152">createdDateTime</span></span>|<span data-ttu-id="f08dc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f08dc-153">DateTimeOffset</span></span>|<span data-ttu-id="f08dc-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f08dc-154">DateTime the object was created.</span></span> <span data-ttu-id="f08dc-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-156">description</span><span class="sxs-lookup"><span data-stu-id="f08dc-156">description</span></span>|<span data-ttu-id="f08dc-157">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-157">String</span></span>|<span data-ttu-id="f08dc-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f08dc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f08dc-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f08dc-160">displayName</span></span>|<span data-ttu-id="f08dc-161">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-161">String</span></span>|<span data-ttu-id="f08dc-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f08dc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f08dc-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-164">version</span><span class="sxs-lookup"><span data-stu-id="f08dc-164">version</span></span>|<span data-ttu-id="f08dc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f08dc-165">Int32</span></span>|<span data-ttu-id="f08dc-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f08dc-166">Version of the device configuration.</span></span> <span data-ttu-id="f08dc-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f08dc-168">connectionName</span></span>|<span data-ttu-id="f08dc-169">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-169">String</span></span>|<span data-ttu-id="f08dc-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f08dc-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f08dc-171">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-172">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="f08dc-172">connectionType</span></span>|[<span data-ttu-id="f08dc-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f08dc-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f08dc-174">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f08dc-174">Connection type.</span></span> <span data-ttu-id="f08dc-175">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f08dc-176">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="f08dc-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="f08dc-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f08dc-177">loginGroupOrDomain</span></span>|<span data-ttu-id="f08dc-178">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-178">String</span></span>|<span data-ttu-id="f08dc-179">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="f08dc-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f08dc-180">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-181">role</span><span class="sxs-lookup"><span data-stu-id="f08dc-181">role</span></span>|<span data-ttu-id="f08dc-182">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-182">String</span></span>|<span data-ttu-id="f08dc-183">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="f08dc-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f08dc-184">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-185">область</span><span class="sxs-lookup"><span data-stu-id="f08dc-185">realm</span></span>|<span data-ttu-id="f08dc-186">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-186">String</span></span>|<span data-ttu-id="f08dc-187">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="f08dc-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f08dc-188">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-189">сервер</span><span class="sxs-lookup"><span data-stu-id="f08dc-189">server</span></span>|[<span data-ttu-id="f08dc-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f08dc-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f08dc-191">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="f08dc-191">VPN Server on the network.</span></span> <span data-ttu-id="f08dc-192">Убедитесь, что конечные пользователи могут получить доступ к этой сетевой папке.</span><span class="sxs-lookup"><span data-stu-id="f08dc-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="f08dc-193">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-194">идентификатор</span><span class="sxs-lookup"><span data-stu-id="f08dc-194">identifier</span></span>|<span data-ttu-id="f08dc-195">String</span><span class="sxs-lookup"><span data-stu-id="f08dc-195">String</span></span>|<span data-ttu-id="f08dc-196">Идентификатор предоставлена поставщиком VPN, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="f08dc-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f08dc-197">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-198">customData</span><span class="sxs-lookup"><span data-stu-id="f08dc-198">customData</span></span>|<span data-ttu-id="f08dc-199">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f08dc-200">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="f08dc-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f08dc-201">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="f08dc-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f08dc-202">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="f08dc-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f08dc-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08dc-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f08dc-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f08dc-205">customKeyValueData</span></span>|<span data-ttu-id="f08dc-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f08dc-207">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="f08dc-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f08dc-208">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="f08dc-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f08dc-209">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="f08dc-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f08dc-210">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08dc-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f08dc-211">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f08dc-212">enableSplitTunneling</span></span>|<span data-ttu-id="f08dc-213">Логический</span><span class="sxs-lookup"><span data-stu-id="f08dc-213">Boolean</span></span>|<span data-ttu-id="f08dc-214">Отправьте все сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="f08dc-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="f08dc-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f08dc-216">authenticationMethod</span></span>|[<span data-ttu-id="f08dc-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f08dc-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f08dc-218">Метод проверки подлинности для VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="f08dc-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f08dc-219">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08dc-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f08dc-220">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f08dc-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f08dc-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f08dc-221">enablePerApp</span></span>|<span data-ttu-id="f08dc-222">Логический</span><span class="sxs-lookup"><span data-stu-id="f08dc-222">Boolean</span></span>|<span data-ttu-id="f08dc-223">Установка значения true создает полезных данных VPN-App, который позднее можно сопоставить с приложениями, которые может активировать этот conneciton VPN на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f08dc-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f08dc-224">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f08dc-225">safariDomains</span></span>|<span data-ttu-id="f08dc-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f08dc-226">String collection</span></span>|<span data-ttu-id="f08dc-227">Safari доменов, при включении VPN каждого параметра приложения.</span><span class="sxs-lookup"><span data-stu-id="f08dc-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f08dc-228">В дополнение к приложений, связанных с этой виртуальной частной сети Safari домены указанного здесь также будет иметь для запуска этой VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f08dc-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f08dc-229">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f08dc-230">onDemandRules</span></span>|<span data-ttu-id="f08dc-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f08dc-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f08dc-232">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="f08dc-232">On-Demand Rules.</span></span> <span data-ttu-id="f08dc-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08dc-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f08dc-234">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-235">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="f08dc-235">proxyServer</span></span>|[<span data-ttu-id="f08dc-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f08dc-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f08dc-237">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f08dc-237">Proxy Server.</span></span> <span data-ttu-id="f08dc-238">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08dc-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f08dc-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f08dc-240">Логический</span><span class="sxs-lookup"><span data-stu-id="f08dc-240">Boolean</span></span>|<span data-ttu-id="f08dc-241">Явного согласия пользователя к совместному использованию кода устройства сторонних производителей VPN-клиентов для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="f08dc-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f08dc-242">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08dc-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f08dc-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="f08dc-243">Response</span></span>
<span data-ttu-id="f08dc-244">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f08dc-244">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f08dc-245">Пример</span><span class="sxs-lookup"><span data-stu-id="f08dc-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="f08dc-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="f08dc-246">Request</span></span>
<span data-ttu-id="f08dc-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f08dc-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="f08dc-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="f08dc-248">Response</span></span>
<span data-ttu-id="f08dc-p127">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f08dc-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




