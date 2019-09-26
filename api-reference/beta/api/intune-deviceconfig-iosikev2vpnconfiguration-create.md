---
title: Создание iosikEv2VpnConfiguration
description: Создание нового объекта iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a09ff78b55849dfcc358c040cc983324543107b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174384"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="b5741-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5741-103">Create iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="b5741-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5741-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5741-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5741-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5741-106">Создание нового объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b5741-106">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5741-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5741-107">Prerequisites</span></span>
<span data-ttu-id="b5741-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5741-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5741-110">Permission type</span></span>|<span data-ttu-id="b5741-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5741-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5741-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5741-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5741-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5741-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5741-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5741-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5741-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5741-115">Not supported.</span></span>|
|<span data-ttu-id="b5741-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5741-116">Application</span></span>|<span data-ttu-id="b5741-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5741-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5741-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5741-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b5741-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5741-119">Request headers</span></span>
|<span data-ttu-id="b5741-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5741-120">Header</span></span>|<span data-ttu-id="b5741-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b5741-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5741-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5741-122">Authorization</span></span>|<span data-ttu-id="b5741-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5741-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5741-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5741-124">Accept</span></span>|<span data-ttu-id="b5741-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5741-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5741-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5741-126">Request body</span></span>
<span data-ttu-id="b5741-127">В тексте запроса добавьте представление объекта iosikEv2VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5741-127">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="b5741-128">В следующей таблице приведены свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b5741-128">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="b5741-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5741-129">Property</span></span>|<span data-ttu-id="b5741-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b5741-130">Type</span></span>|<span data-ttu-id="b5741-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b5741-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5741-132">id</span><span class="sxs-lookup"><span data-stu-id="b5741-132">id</span></span>|<span data-ttu-id="b5741-133">String</span><span class="sxs-lookup"><span data-stu-id="b5741-133">String</span></span>|<span data-ttu-id="b5741-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b5741-134">Key of the entity.</span></span> <span data-ttu-id="b5741-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5741-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b5741-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5741-137">DateTimeOffset</span></span>|<span data-ttu-id="b5741-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b5741-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b5741-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5741-140">roleScopeTagIds</span></span>|<span data-ttu-id="b5741-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b5741-141">String collection</span></span>|<span data-ttu-id="b5741-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b5741-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5741-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b5741-144">supportsScopeTags</span></span>|<span data-ttu-id="b5741-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-145">Boolean</span></span>|<span data-ttu-id="b5741-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b5741-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5741-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b5741-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5741-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b5741-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5741-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5741-149">This property is read-only.</span></span> <span data-ttu-id="b5741-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5741-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5741-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5741-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5741-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b5741-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5741-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5741-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5741-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5741-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5741-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b5741-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5741-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="b5741-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5741-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="b5741-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5741-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b5741-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5741-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5741-163">createdDateTime</span></span>|<span data-ttu-id="b5741-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5741-164">DateTimeOffset</span></span>|<span data-ttu-id="b5741-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b5741-165">DateTime the object was created.</span></span> <span data-ttu-id="b5741-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-167">description</span><span class="sxs-lookup"><span data-stu-id="b5741-167">description</span></span>|<span data-ttu-id="b5741-168">String</span><span class="sxs-lookup"><span data-stu-id="b5741-168">String</span></span>|<span data-ttu-id="b5741-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b5741-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5741-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b5741-171">displayName</span></span>|<span data-ttu-id="b5741-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b5741-172">String</span></span>|<span data-ttu-id="b5741-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b5741-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5741-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-175">version</span><span class="sxs-lookup"><span data-stu-id="b5741-175">version</span></span>|<span data-ttu-id="b5741-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b5741-176">Int32</span></span>|<span data-ttu-id="b5741-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b5741-177">Version of the device configuration.</span></span> <span data-ttu-id="b5741-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="b5741-179">connectionName</span></span>|<span data-ttu-id="b5741-180">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-180">String</span></span>|<span data-ttu-id="b5741-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5741-181">Connection name displayed to the user.</span></span> <span data-ttu-id="b5741-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="b5741-183">connectionType</span></span>|[<span data-ttu-id="b5741-184">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="b5741-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="b5741-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="b5741-185">Connection type.</span></span> <span data-ttu-id="b5741-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b5741-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,. `ikEv2`</span><span class="sxs-lookup"><span data-stu-id="b5741-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="b5741-188">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="b5741-188">loginGroupOrDomain</span></span>|<span data-ttu-id="b5741-189">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-189">String</span></span>|<span data-ttu-id="b5741-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="b5741-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b5741-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-192">role</span><span class="sxs-lookup"><span data-stu-id="b5741-192">role</span></span>|<span data-ttu-id="b5741-193">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-193">String</span></span>|<span data-ttu-id="b5741-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="b5741-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b5741-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-196">область</span><span class="sxs-lookup"><span data-stu-id="b5741-196">realm</span></span>|<span data-ttu-id="b5741-197">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-197">String</span></span>|<span data-ttu-id="b5741-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="b5741-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b5741-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-200">сервер</span><span class="sxs-lookup"><span data-stu-id="b5741-200">server</span></span>|[<span data-ttu-id="b5741-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="b5741-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="b5741-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="b5741-202">VPN Server on the network.</span></span> <span data-ttu-id="b5741-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="b5741-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="b5741-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="b5741-205">identifier</span></span>|<span data-ttu-id="b5741-206">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-206">String</span></span>|<span data-ttu-id="b5741-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b5741-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="b5741-209">customData</span></span>|<span data-ttu-id="b5741-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b5741-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b5741-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b5741-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="b5741-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b5741-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="b5741-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b5741-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b5741-216">customKeyValueData</span></span>|<span data-ttu-id="b5741-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b5741-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b5741-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b5741-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="b5741-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b5741-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="b5741-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b5741-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-223">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="b5741-223">enableSplitTunneling</span></span>|<span data-ttu-id="b5741-224">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-224">Boolean</span></span>|<span data-ttu-id="b5741-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="b5741-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="b5741-227">authenticationMethod</span></span>|[<span data-ttu-id="b5741-228">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b5741-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b5741-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="b5741-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="b5741-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b5741-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b5741-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b5741-232">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="b5741-232">enablePerApp</span></span>|<span data-ttu-id="b5741-233">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-233">Boolean</span></span>|<span data-ttu-id="b5741-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5741-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="b5741-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-236">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="b5741-236">safariDomains</span></span>|<span data-ttu-id="b5741-237">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b5741-237">String collection</span></span>|<span data-ttu-id="b5741-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="b5741-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="b5741-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="b5741-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="b5741-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-241">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="b5741-241">onDemandRules</span></span>|<span data-ttu-id="b5741-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="b5741-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="b5741-243">On-Demand Rules.</span></span> <span data-ttu-id="b5741-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b5741-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b5741-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="b5741-246">proxyServer</span></span>|[<span data-ttu-id="b5741-247">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="b5741-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b5741-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="b5741-248">Proxy Server.</span></span> <span data-ttu-id="b5741-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-250">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="b5741-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="b5741-251">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-251">Boolean</span></span>|<span data-ttu-id="b5741-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="b5741-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="b5741-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-254">providerType</span><span class="sxs-lookup"><span data-stu-id="b5741-254">providerType</span></span>|[<span data-ttu-id="b5741-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="b5741-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="b5741-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="b5741-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="b5741-257">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5741-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="b5741-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="b5741-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="b5741-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="b5741-259">userDomain</span></span>|<span data-ttu-id="b5741-260">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-260">String</span></span>|<span data-ttu-id="b5741-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-261">Zscaler only.</span></span> <span data-ttu-id="b5741-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="b5741-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5741-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="b5741-264">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-265">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="b5741-265">strictEnforcement</span></span>|<span data-ttu-id="b5741-266">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-266">Boolean</span></span>|<span data-ttu-id="b5741-267">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-267">Zscaler only.</span></span> <span data-ttu-id="b5741-268">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="b5741-269">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="b5741-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="b5741-270">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-271">клауднаме</span><span class="sxs-lookup"><span data-stu-id="b5741-271">cloudName</span></span>|<span data-ttu-id="b5741-272">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-272">String</span></span>|<span data-ttu-id="b5741-273">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-273">Zscaler only.</span></span> <span data-ttu-id="b5741-274">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="b5741-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="b5741-275">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="b5741-276">excludeList</span></span>|<span data-ttu-id="b5741-277">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b5741-277">String collection</span></span>|<span data-ttu-id="b5741-278">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-278">Zscaler only.</span></span> <span data-ttu-id="b5741-279">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="b5741-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="b5741-280">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5741-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5741-281">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="b5741-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="b5741-282">иосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="b5741-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="b5741-283">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="b5741-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="b5741-284">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="b5741-284">clientAuthenticationType</span></span>|[<span data-ttu-id="b5741-285">впнклиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="b5741-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="b5741-286">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="b5741-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="b5741-287">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="b5741-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="b5741-288">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="b5741-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="b5741-289">впндеадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="b5741-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="b5741-290">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="b5741-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="b5741-291">.</span><span class="sxs-lookup"><span data-stu-id="b5741-291"></span></span> <span data-ttu-id="b5741-292">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b5741-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="b5741-293">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="b5741-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="b5741-294">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-294">Boolean</span></span>|<span data-ttu-id="b5741-295">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="b5741-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="b5741-296">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="b5741-296">disableRedirect</span></span>|<span data-ttu-id="b5741-297">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-297">Boolean</span></span>|<span data-ttu-id="b5741-298">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="b5741-298">Disable Redirect</span></span>|
|<span data-ttu-id="b5741-299">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="b5741-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="b5741-300">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-300">Boolean</span></span>|<span data-ttu-id="b5741-301">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="b5741-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="b5741-302">енаблиап</span><span class="sxs-lookup"><span data-stu-id="b5741-302">enableEAP</span></span>|<span data-ttu-id="b5741-303">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-303">Boolean</span></span>|<span data-ttu-id="b5741-304">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="b5741-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="b5741-305">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="b5741-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="b5741-306">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-306">Boolean</span></span>|<span data-ttu-id="b5741-307">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="b5741-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="b5741-308">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="b5741-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="b5741-309">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-309">Boolean</span></span>|<span data-ttu-id="b5741-310">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="b5741-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="b5741-311">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="b5741-311">localIdentifier</span></span>|[<span data-ttu-id="b5741-312">впнлокалидентифиер</span><span class="sxs-lookup"><span data-stu-id="b5741-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="b5741-313">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="b5741-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="b5741-314">.</span><span class="sxs-lookup"><span data-stu-id="b5741-314"></span></span> <span data-ttu-id="b5741-315">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="b5741-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="b5741-316">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="b5741-316">remoteIdentifier</span></span>|<span data-ttu-id="b5741-317">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-317">String</span></span>|<span data-ttu-id="b5741-318">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="b5741-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="b5741-319">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="b5741-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="b5741-320">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="b5741-320">securityAssociationParameters</span></span>|[<span data-ttu-id="b5741-321">иосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="b5741-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="b5741-322">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="b5741-322">Security Association Parameters</span></span>|
|<span data-ttu-id="b5741-323">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="b5741-323">serverCertificateCommonName</span></span>|<span data-ttu-id="b5741-324">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-324">String</span></span>|<span data-ttu-id="b5741-325">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="b5741-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="b5741-326">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="b5741-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="b5741-327">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-327">String</span></span>|<span data-ttu-id="b5741-328">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="b5741-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="b5741-329">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="b5741-329">serverCertificateType</span></span>|[<span data-ttu-id="b5741-330">впнсерверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="b5741-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="b5741-331">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b5741-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="b5741-332">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="b5741-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="b5741-333">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="b5741-333">sharedSecret</span></span>|<span data-ttu-id="b5741-334">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-334">String</span></span>|<span data-ttu-id="b5741-335">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="b5741-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="b5741-336">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="b5741-336">tlsMaximumVersion</span></span>|<span data-ttu-id="b5741-337">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-337">String</span></span>|<span data-ttu-id="b5741-338">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="b5741-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="b5741-339">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="b5741-339">tlsMinimumVersion</span></span>|<span data-ttu-id="b5741-340">String.</span><span class="sxs-lookup"><span data-stu-id="b5741-340">String</span></span>|<span data-ttu-id="b5741-341">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="b5741-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="b5741-342">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="b5741-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="b5741-343">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-343">Boolean</span></span>|<span data-ttu-id="b5741-344">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="b5741-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="b5741-345">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="b5741-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="b5741-346">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b5741-346">Boolean</span></span>|<span data-ttu-id="b5741-347">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="b5741-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|



## <a name="response"></a><span data-ttu-id="b5741-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5741-348">Response</span></span>
<span data-ttu-id="b5741-349">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5741-349">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5741-350">Пример</span><span class="sxs-lookup"><span data-stu-id="b5741-350">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5741-351">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5741-351">Request</span></span>
<span data-ttu-id="b5741-352">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5741-352">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4232

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```

### <a name="response"></a><span data-ttu-id="b5741-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5741-353">Response</span></span>
<span data-ttu-id="b5741-p139">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5741-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4404

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```




