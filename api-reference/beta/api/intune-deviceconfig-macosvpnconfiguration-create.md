---
title: Создание macOSVpnConfiguration
description: Создание нового объекта macOSVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2c8e2aefb0aa7bfc3a73ac83d32823d9c3c44a3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416015"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="79c2a-103">Создание macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="79c2a-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="79c2a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79c2a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79c2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79c2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79c2a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79c2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79c2a-107">Создание нового объекта [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79c2a-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79c2a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="79c2a-108">Prerequisites</span></span>
<span data-ttu-id="79c2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="79c2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79c2a-111">Permission type</span></span>|<span data-ttu-id="79c2a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79c2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79c2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79c2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79c2a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79c2a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79c2a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79c2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79c2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79c2a-116">Not supported.</span></span>|
|<span data-ttu-id="79c2a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79c2a-117">Application</span></span>|<span data-ttu-id="79c2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79c2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79c2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79c2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79c2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79c2a-120">Request headers</span></span>
|<span data-ttu-id="79c2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79c2a-121">Header</span></span>|<span data-ttu-id="79c2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="79c2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79c2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79c2a-123">Authorization</span></span>|<span data-ttu-id="79c2a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="79c2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79c2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79c2a-125">Accept</span></span>|<span data-ttu-id="79c2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79c2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79c2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79c2a-127">Request body</span></span>
<span data-ttu-id="79c2a-128">В тексте запроса укажите представление JSON для объекта macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79c2a-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="79c2a-129">В следующей таблице показаны свойства, которые необходимы для создания macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79c2a-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="79c2a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="79c2a-130">Property</span></span>|<span data-ttu-id="79c2a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79c2a-131">Type</span></span>|<span data-ttu-id="79c2a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79c2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79c2a-133">id</span><span class="sxs-lookup"><span data-stu-id="79c2a-133">id</span></span>|<span data-ttu-id="79c2a-134">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-134">String</span></span>|<span data-ttu-id="79c2a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79c2a-135">Key of the entity.</span></span> <span data-ttu-id="79c2a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79c2a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="79c2a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c2a-138">DateTimeOffset</span></span>|<span data-ttu-id="79c2a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="79c2a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="79c2a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79c2a-141">roleScopeTagIds</span></span>|<span data-ttu-id="79c2a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79c2a-142">String collection</span></span>|<span data-ttu-id="79c2a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="79c2a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79c2a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="79c2a-145">supportsScopeTags</span></span>|<span data-ttu-id="79c2a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="79c2a-146">Boolean</span></span>|<span data-ttu-id="79c2a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="79c2a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79c2a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="79c2a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79c2a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="79c2a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79c2a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79c2a-150">This property is read-only.</span></span> <span data-ttu-id="79c2a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79c2a-152">createdDateTime</span></span>|<span data-ttu-id="79c2a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c2a-153">DateTimeOffset</span></span>|<span data-ttu-id="79c2a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="79c2a-154">DateTime the object was created.</span></span> <span data-ttu-id="79c2a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-156">description</span><span class="sxs-lookup"><span data-stu-id="79c2a-156">description</span></span>|<span data-ttu-id="79c2a-157">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-157">String</span></span>|<span data-ttu-id="79c2a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79c2a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79c2a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="79c2a-160">displayName</span></span>|<span data-ttu-id="79c2a-161">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-161">String</span></span>|<span data-ttu-id="79c2a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79c2a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79c2a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-164">version</span><span class="sxs-lookup"><span data-stu-id="79c2a-164">version</span></span>|<span data-ttu-id="79c2a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="79c2a-165">Int32</span></span>|<span data-ttu-id="79c2a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79c2a-166">Version of the device configuration.</span></span> <span data-ttu-id="79c2a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="79c2a-168">connectionName</span></span>|<span data-ttu-id="79c2a-169">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-169">String</span></span>|<span data-ttu-id="79c2a-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="79c2a-170">Connection name displayed to the user.</span></span> <span data-ttu-id="79c2a-171">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-172">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="79c2a-172">connectionType</span></span>|[<span data-ttu-id="79c2a-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="79c2a-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="79c2a-174">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="79c2a-174">Connection type.</span></span> <span data-ttu-id="79c2a-175">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="79c2a-176">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="79c2a-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="79c2a-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="79c2a-177">loginGroupOrDomain</span></span>|<span data-ttu-id="79c2a-178">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-178">String</span></span>|<span data-ttu-id="79c2a-179">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="79c2a-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="79c2a-180">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-181">role</span><span class="sxs-lookup"><span data-stu-id="79c2a-181">role</span></span>|<span data-ttu-id="79c2a-182">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-182">String</span></span>|<span data-ttu-id="79c2a-183">Роль, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="79c2a-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="79c2a-184">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-185">область</span><span class="sxs-lookup"><span data-stu-id="79c2a-185">realm</span></span>|<span data-ttu-id="79c2a-186">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-186">String</span></span>|<span data-ttu-id="79c2a-187">Область, если тип подключения для обеспечения безопасности Pulse.</span><span class="sxs-lookup"><span data-stu-id="79c2a-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="79c2a-188">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-189">сервер</span><span class="sxs-lookup"><span data-stu-id="79c2a-189">server</span></span>|[<span data-ttu-id="79c2a-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="79c2a-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="79c2a-191">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="79c2a-191">VPN Server on the network.</span></span> <span data-ttu-id="79c2a-192">Убедитесь, что конечные пользователи могут получить доступ к этой сетевой папке.</span><span class="sxs-lookup"><span data-stu-id="79c2a-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="79c2a-193">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-194">идентификатор</span><span class="sxs-lookup"><span data-stu-id="79c2a-194">identifier</span></span>|<span data-ttu-id="79c2a-195">String</span><span class="sxs-lookup"><span data-stu-id="79c2a-195">String</span></span>|<span data-ttu-id="79c2a-196">Идентификатор предоставлена поставщиком VPN, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="79c2a-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="79c2a-197">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-198">customData</span><span class="sxs-lookup"><span data-stu-id="79c2a-198">customData</span></span>|<span data-ttu-id="79c2a-199">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="79c2a-200">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="79c2a-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="79c2a-201">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="79c2a-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="79c2a-202">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="79c2a-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="79c2a-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="79c2a-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="79c2a-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="79c2a-205">customKeyValueData</span></span>|<span data-ttu-id="79c2a-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="79c2a-207">Пользовательские данные, если тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="79c2a-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="79c2a-208">Это поле используется для включения функциональных возможностей, не поддерживаемых Intune, но доступны в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="79c2a-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="79c2a-209">Обратитесь к поставщику сети VPN, чтобы узнать, как добавить эти ключ значение пары.</span><span class="sxs-lookup"><span data-stu-id="79c2a-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="79c2a-210">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="79c2a-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="79c2a-211">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="79c2a-212">enableSplitTunneling</span></span>|<span data-ttu-id="79c2a-213">Логический</span><span class="sxs-lookup"><span data-stu-id="79c2a-213">Boolean</span></span>|<span data-ttu-id="79c2a-214">Отправьте все сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="79c2a-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="79c2a-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="79c2a-216">authenticationMethod</span></span>|[<span data-ttu-id="79c2a-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="79c2a-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="79c2a-218">Метод проверки подлинности для VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="79c2a-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="79c2a-219">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79c2a-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="79c2a-220">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="79c2a-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="79c2a-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="79c2a-221">enablePerApp</span></span>|<span data-ttu-id="79c2a-222">Логический</span><span class="sxs-lookup"><span data-stu-id="79c2a-222">Boolean</span></span>|<span data-ttu-id="79c2a-223">Установка значения true создает полезных данных VPN-App, который позднее можно сопоставить с приложениями, которые может активировать этот conneciton VPN на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="79c2a-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="79c2a-224">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="79c2a-225">safariDomains</span></span>|<span data-ttu-id="79c2a-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79c2a-226">String collection</span></span>|<span data-ttu-id="79c2a-227">Safari доменов, при включении VPN каждого параметра приложения.</span><span class="sxs-lookup"><span data-stu-id="79c2a-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="79c2a-228">В дополнение к приложений, связанных с этой виртуальной частной сети Safari домены указанного здесь также будет иметь для запуска этой VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="79c2a-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="79c2a-229">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="79c2a-230">onDemandRules</span></span>|<span data-ttu-id="79c2a-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="79c2a-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="79c2a-232">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="79c2a-232">On-Demand Rules.</span></span> <span data-ttu-id="79c2a-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="79c2a-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="79c2a-234">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-235">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="79c2a-235">proxyServer</span></span>|[<span data-ttu-id="79c2a-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="79c2a-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="79c2a-237">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="79c2a-237">Proxy Server.</span></span> <span data-ttu-id="79c2a-238">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="79c2a-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="79c2a-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="79c2a-240">Логический</span><span class="sxs-lookup"><span data-stu-id="79c2a-240">Boolean</span></span>|<span data-ttu-id="79c2a-241">Явного согласия пользователя к совместному использованию кода устройства сторонних производителей VPN-клиентов для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="79c2a-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="79c2a-242">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79c2a-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="79c2a-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c2a-243">Response</span></span>
<span data-ttu-id="79c2a-244">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="79c2a-244">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79c2a-245">Пример</span><span class="sxs-lookup"><span data-stu-id="79c2a-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="79c2a-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="79c2a-246">Request</span></span>
<span data-ttu-id="79c2a-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79c2a-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="79c2a-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c2a-248">Response</span></span>
<span data-ttu-id="79c2a-p127">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79c2a-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




