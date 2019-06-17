---
title: Создание Иосвпнконфигуратион
description: Создание нового объекта Иосвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f98b3a58043a3cf19e1702d815e3fc3ad0b32eb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977116"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="ba313-103">Создание Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ba313-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="ba313-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba313-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba313-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba313-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba313-106">Создание нового объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ba313-106">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba313-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba313-107">Prerequisites</span></span>
<span data-ttu-id="ba313-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba313-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba313-110">Permission type</span></span>|<span data-ttu-id="ba313-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba313-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba313-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba313-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba313-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba313-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba313-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba313-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba313-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba313-115">Not supported.</span></span>|
|<span data-ttu-id="ba313-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba313-116">Application</span></span>|<span data-ttu-id="ba313-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba313-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba313-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba313-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ba313-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba313-119">Request headers</span></span>
|<span data-ttu-id="ba313-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba313-120">Header</span></span>|<span data-ttu-id="ba313-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba313-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba313-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba313-122">Authorization</span></span>|<span data-ttu-id="ba313-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba313-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba313-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba313-124">Accept</span></span>|<span data-ttu-id="ba313-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba313-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba313-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba313-126">Request body</span></span>
<span data-ttu-id="ba313-127">В тексте запроса добавьте представление объекта Иосвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba313-127">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="ba313-128">В следующей таблице приведены свойства, необходимые при создании Иосвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="ba313-128">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="ba313-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba313-129">Property</span></span>|<span data-ttu-id="ba313-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba313-130">Type</span></span>|<span data-ttu-id="ba313-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba313-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba313-132">id</span><span class="sxs-lookup"><span data-stu-id="ba313-132">id</span></span>|<span data-ttu-id="ba313-133">String</span><span class="sxs-lookup"><span data-stu-id="ba313-133">String</span></span>|<span data-ttu-id="ba313-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba313-134">Key of the entity.</span></span> <span data-ttu-id="ba313-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba313-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ba313-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba313-137">DateTimeOffset</span></span>|<span data-ttu-id="ba313-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ba313-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ba313-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ba313-140">roleScopeTagIds</span></span>|<span data-ttu-id="ba313-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba313-141">String collection</span></span>|<span data-ttu-id="ba313-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ba313-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ba313-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ba313-144">supportsScopeTags</span></span>|<span data-ttu-id="ba313-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba313-145">Boolean</span></span>|<span data-ttu-id="ba313-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ba313-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ba313-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ba313-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ba313-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ba313-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ba313-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba313-149">This property is read-only.</span></span> <span data-ttu-id="ba313-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ba313-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ba313-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ba313-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ba313-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba313-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ba313-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ba313-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ba313-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ba313-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ba313-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba313-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ba313-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ba313-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ba313-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ba313-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ba313-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba313-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ba313-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba313-163">createdDateTime</span></span>|<span data-ttu-id="ba313-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba313-164">DateTimeOffset</span></span>|<span data-ttu-id="ba313-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ba313-165">DateTime the object was created.</span></span> <span data-ttu-id="ba313-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-167">description</span><span class="sxs-lookup"><span data-stu-id="ba313-167">description</span></span>|<span data-ttu-id="ba313-168">String</span><span class="sxs-lookup"><span data-stu-id="ba313-168">String</span></span>|<span data-ttu-id="ba313-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba313-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ba313-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ba313-171">displayName</span></span>|<span data-ttu-id="ba313-172">Строка</span><span class="sxs-lookup"><span data-stu-id="ba313-172">String</span></span>|<span data-ttu-id="ba313-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba313-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ba313-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-175">version</span><span class="sxs-lookup"><span data-stu-id="ba313-175">version</span></span>|<span data-ttu-id="ba313-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ba313-176">Int32</span></span>|<span data-ttu-id="ba313-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba313-177">Version of the device configuration.</span></span> <span data-ttu-id="ba313-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-179">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="ba313-179">connectionName</span></span>|<span data-ttu-id="ba313-180">String</span><span class="sxs-lookup"><span data-stu-id="ba313-180">String</span></span>|<span data-ttu-id="ba313-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba313-181">Connection name displayed to the user.</span></span> <span data-ttu-id="ba313-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="ba313-183">connectionType</span></span>|[<span data-ttu-id="ba313-184">Апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="ba313-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ba313-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ba313-185">Connection type.</span></span> <span data-ttu-id="ba313-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ba313-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,. `ikEv2`</span><span class="sxs-lookup"><span data-stu-id="ba313-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="ba313-188">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="ba313-188">loginGroupOrDomain</span></span>|<span data-ttu-id="ba313-189">String</span><span class="sxs-lookup"><span data-stu-id="ba313-189">String</span></span>|<span data-ttu-id="ba313-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="ba313-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ba313-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-192">role</span><span class="sxs-lookup"><span data-stu-id="ba313-192">role</span></span>|<span data-ttu-id="ba313-193">String</span><span class="sxs-lookup"><span data-stu-id="ba313-193">String</span></span>|<span data-ttu-id="ba313-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="ba313-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ba313-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-196">область</span><span class="sxs-lookup"><span data-stu-id="ba313-196">realm</span></span>|<span data-ttu-id="ba313-197">String</span><span class="sxs-lookup"><span data-stu-id="ba313-197">String</span></span>|<span data-ttu-id="ba313-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="ba313-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ba313-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-200">сервер</span><span class="sxs-lookup"><span data-stu-id="ba313-200">server</span></span>|[<span data-ttu-id="ba313-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="ba313-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ba313-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="ba313-202">VPN Server on the network.</span></span> <span data-ttu-id="ba313-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="ba313-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="ba313-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="ba313-205">identifier</span></span>|<span data-ttu-id="ba313-206">String</span><span class="sxs-lookup"><span data-stu-id="ba313-206">String</span></span>|<span data-ttu-id="ba313-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="ba313-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ba313-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="ba313-209">customData</span></span>|<span data-ttu-id="ba313-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ba313-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="ba313-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ba313-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="ba313-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ba313-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ba313-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ba313-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba313-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ba313-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ba313-216">customKeyValueData</span></span>|<span data-ttu-id="ba313-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ba313-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="ba313-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ba313-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="ba313-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ba313-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ba313-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ba313-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba313-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ba313-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-223">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="ba313-223">enableSplitTunneling</span></span>|<span data-ttu-id="ba313-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba313-224">Boolean</span></span>|<span data-ttu-id="ba313-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="ba313-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="ba313-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="ba313-227">authenticationMethod</span></span>|[<span data-ttu-id="ba313-228">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ba313-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ba313-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="ba313-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ba313-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ba313-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ba313-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ba313-232">Енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="ba313-232">enablePerApp</span></span>|<span data-ttu-id="ba313-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba313-233">Boolean</span></span>|<span data-ttu-id="ba313-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba313-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ba313-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-236">Сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="ba313-236">safariDomains</span></span>|<span data-ttu-id="ba313-237">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba313-237">String collection</span></span>|<span data-ttu-id="ba313-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="ba313-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ba313-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="ba313-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ba313-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-241">Ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="ba313-241">onDemandRules</span></span>|<span data-ttu-id="ba313-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ba313-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="ba313-243">On-Demand Rules.</span></span> <span data-ttu-id="ba313-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba313-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ba313-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="ba313-246">proxyServer</span></span>|[<span data-ttu-id="ba313-247">Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="ba313-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ba313-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ba313-248">Proxy Server.</span></span> <span data-ttu-id="ba313-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-250">Оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="ba313-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ba313-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba313-251">Boolean</span></span>|<span data-ttu-id="ba313-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="ba313-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ba313-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba313-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ba313-254">providerType</span><span class="sxs-lookup"><span data-stu-id="ba313-254">providerType</span></span>|[<span data-ttu-id="ba313-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="ba313-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="ba313-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="ba313-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="ba313-257">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="ba313-257">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="ba313-258">userDomain</span><span class="sxs-lookup"><span data-stu-id="ba313-258">userDomain</span></span>|<span data-ttu-id="ba313-259">String</span><span class="sxs-lookup"><span data-stu-id="ba313-259">String</span></span>|<span data-ttu-id="ba313-260">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-260">Zscaler only.</span></span> <span data-ttu-id="ba313-261">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-261">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="ba313-262">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba313-262">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="ba313-263">Стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="ba313-263">strictEnforcement</span></span>|<span data-ttu-id="ba313-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba313-264">Boolean</span></span>|<span data-ttu-id="ba313-265">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-265">Zscaler only.</span></span> <span data-ttu-id="ba313-266">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-266">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="ba313-267">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="ba313-267">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="ba313-268">Клауднаме</span><span class="sxs-lookup"><span data-stu-id="ba313-268">cloudName</span></span>|<span data-ttu-id="ba313-269">String</span><span class="sxs-lookup"><span data-stu-id="ba313-269">String</span></span>|<span data-ttu-id="ba313-270">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-270">Zscaler only.</span></span> <span data-ttu-id="ba313-271">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="ba313-271">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="ba313-272">excludeList</span><span class="sxs-lookup"><span data-stu-id="ba313-272">excludeList</span></span>|<span data-ttu-id="ba313-273">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba313-273">String collection</span></span>|<span data-ttu-id="ba313-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-274">Zscaler only.</span></span> <span data-ttu-id="ba313-275">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="ba313-275">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="ba313-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba313-276">Response</span></span>
<span data-ttu-id="ba313-277">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba313-277">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba313-278">Пример</span><span class="sxs-lookup"><span data-stu-id="ba313-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba313-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba313-279">Request</span></span>
<span data-ttu-id="ba313-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba313-280">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2815

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="ba313-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba313-281">Response</span></span>
<span data-ttu-id="ba313-p134">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba313-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2987

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  ]
}
```





