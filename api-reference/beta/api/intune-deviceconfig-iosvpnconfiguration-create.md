---
title: Создание Иосвпнконфигуратион
description: Создание нового объекта Иосвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab01add46427f8831e761c94d00264b8a949c180
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442567"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="fa777-103">Создание Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="fa777-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="fa777-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa777-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa777-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa777-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa777-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa777-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa777-107">Создание нового объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fa777-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa777-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa777-108">Prerequisites</span></span>
<span data-ttu-id="fa777-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa777-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa777-111">Permission type</span></span>|<span data-ttu-id="fa777-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa777-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa777-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa777-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa777-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa777-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa777-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa777-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa777-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa777-116">Not supported.</span></span>|
|<span data-ttu-id="fa777-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa777-117">Application</span></span>|<span data-ttu-id="fa777-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa777-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa777-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa777-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa777-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa777-120">Request headers</span></span>
|<span data-ttu-id="fa777-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa777-121">Header</span></span>|<span data-ttu-id="fa777-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa777-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa777-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa777-123">Authorization</span></span>|<span data-ttu-id="fa777-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa777-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa777-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa777-125">Accept</span></span>|<span data-ttu-id="fa777-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa777-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa777-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa777-127">Request body</span></span>
<span data-ttu-id="fa777-128">В тексте запроса добавьте представление объекта Иосвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa777-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="fa777-129">В следующей таблице приведены свойства, необходимые при создании Иосвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="fa777-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="fa777-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa777-130">Property</span></span>|<span data-ttu-id="fa777-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa777-131">Type</span></span>|<span data-ttu-id="fa777-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa777-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa777-133">id</span><span class="sxs-lookup"><span data-stu-id="fa777-133">id</span></span>|<span data-ttu-id="fa777-134">String</span><span class="sxs-lookup"><span data-stu-id="fa777-134">String</span></span>|<span data-ttu-id="fa777-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fa777-135">Key of the entity.</span></span> <span data-ttu-id="fa777-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa777-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fa777-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa777-138">DateTimeOffset</span></span>|<span data-ttu-id="fa777-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fa777-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fa777-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fa777-141">roleScopeTagIds</span></span>|<span data-ttu-id="fa777-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa777-142">String collection</span></span>|<span data-ttu-id="fa777-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fa777-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fa777-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fa777-145">supportsScopeTags</span></span>|<span data-ttu-id="fa777-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fa777-146">Boolean</span></span>|<span data-ttu-id="fa777-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fa777-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fa777-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fa777-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fa777-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fa777-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fa777-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa777-150">This property is read-only.</span></span> <span data-ttu-id="fa777-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fa777-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fa777-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fa777-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fa777-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fa777-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fa777-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fa777-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fa777-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fa777-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fa777-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fa777-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fa777-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fa777-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fa777-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fa777-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fa777-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fa777-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fa777-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa777-164">createdDateTime</span></span>|<span data-ttu-id="fa777-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa777-165">DateTimeOffset</span></span>|<span data-ttu-id="fa777-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fa777-166">DateTime the object was created.</span></span> <span data-ttu-id="fa777-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-168">description</span><span class="sxs-lookup"><span data-stu-id="fa777-168">description</span></span>|<span data-ttu-id="fa777-169">String</span><span class="sxs-lookup"><span data-stu-id="fa777-169">String</span></span>|<span data-ttu-id="fa777-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fa777-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fa777-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fa777-172">displayName</span></span>|<span data-ttu-id="fa777-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fa777-173">String</span></span>|<span data-ttu-id="fa777-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fa777-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fa777-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-176">version</span><span class="sxs-lookup"><span data-stu-id="fa777-176">version</span></span>|<span data-ttu-id="fa777-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fa777-177">Int32</span></span>|<span data-ttu-id="fa777-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fa777-178">Version of the device configuration.</span></span> <span data-ttu-id="fa777-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="fa777-180">connectionName</span></span>|<span data-ttu-id="fa777-181">String</span><span class="sxs-lookup"><span data-stu-id="fa777-181">String</span></span>|<span data-ttu-id="fa777-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa777-182">Connection name displayed to the user.</span></span> <span data-ttu-id="fa777-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="fa777-184">connectionType</span></span>|[<span data-ttu-id="fa777-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="fa777-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="fa777-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="fa777-186">Connection type.</span></span> <span data-ttu-id="fa777-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="fa777-188">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="fa777-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="fa777-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="fa777-189">loginGroupOrDomain</span></span>|<span data-ttu-id="fa777-190">String</span><span class="sxs-lookup"><span data-stu-id="fa777-190">String</span></span>|<span data-ttu-id="fa777-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="fa777-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="fa777-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-193">role</span><span class="sxs-lookup"><span data-stu-id="fa777-193">role</span></span>|<span data-ttu-id="fa777-194">String</span><span class="sxs-lookup"><span data-stu-id="fa777-194">String</span></span>|<span data-ttu-id="fa777-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="fa777-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="fa777-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-197">область</span><span class="sxs-lookup"><span data-stu-id="fa777-197">realm</span></span>|<span data-ttu-id="fa777-198">String</span><span class="sxs-lookup"><span data-stu-id="fa777-198">String</span></span>|<span data-ttu-id="fa777-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="fa777-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="fa777-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-201">сервер</span><span class="sxs-lookup"><span data-stu-id="fa777-201">server</span></span>|[<span data-ttu-id="fa777-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="fa777-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="fa777-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="fa777-203">VPN Server on the network.</span></span> <span data-ttu-id="fa777-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="fa777-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="fa777-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="fa777-206">identifier</span></span>|<span data-ttu-id="fa777-207">String</span><span class="sxs-lookup"><span data-stu-id="fa777-207">String</span></span>|<span data-ttu-id="fa777-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="fa777-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="fa777-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="fa777-210">customData</span></span>|<span data-ttu-id="fa777-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="fa777-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="fa777-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="fa777-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="fa777-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="fa777-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="fa777-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="fa777-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="fa777-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="fa777-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="fa777-217">customKeyValueData</span></span>|<span data-ttu-id="fa777-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fa777-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="fa777-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="fa777-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="fa777-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="fa777-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="fa777-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="fa777-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="fa777-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="fa777-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="fa777-224">enableSplitTunneling</span></span>|<span data-ttu-id="fa777-225">Логический</span><span class="sxs-lookup"><span data-stu-id="fa777-225">Boolean</span></span>|<span data-ttu-id="fa777-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="fa777-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="fa777-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="fa777-228">authenticationMethod</span></span>|[<span data-ttu-id="fa777-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="fa777-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="fa777-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="fa777-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="fa777-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa777-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="fa777-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="fa777-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="fa777-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="fa777-233">enablePerApp</span></span>|<span data-ttu-id="fa777-234">Логический</span><span class="sxs-lookup"><span data-stu-id="fa777-234">Boolean</span></span>|<span data-ttu-id="fa777-235">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa777-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="fa777-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="fa777-237">safariDomains</span></span>|<span data-ttu-id="fa777-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa777-238">String collection</span></span>|<span data-ttu-id="fa777-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="fa777-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="fa777-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="fa777-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="fa777-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="fa777-242">onDemandRules</span></span>|<span data-ttu-id="fa777-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="fa777-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="fa777-244">On-Demand Rules.</span></span> <span data-ttu-id="fa777-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fa777-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fa777-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-247">проксисервер</span><span class="sxs-lookup"><span data-stu-id="fa777-247">proxyServer</span></span>|[<span data-ttu-id="fa777-248">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="fa777-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="fa777-249">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="fa777-249">Proxy Server.</span></span> <span data-ttu-id="fa777-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-251">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="fa777-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="fa777-252">Логический</span><span class="sxs-lookup"><span data-stu-id="fa777-252">Boolean</span></span>|<span data-ttu-id="fa777-253">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="fa777-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="fa777-254">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa777-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="fa777-255">providerType</span><span class="sxs-lookup"><span data-stu-id="fa777-255">providerType</span></span>|[<span data-ttu-id="fa777-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="fa777-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="fa777-257">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="fa777-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="fa777-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="fa777-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="fa777-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="fa777-259">userDomain</span></span>|<span data-ttu-id="fa777-260">String</span><span class="sxs-lookup"><span data-stu-id="fa777-260">String</span></span>|<span data-ttu-id="fa777-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-261">Zscaler only.</span></span> <span data-ttu-id="fa777-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="fa777-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa777-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="fa777-264">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="fa777-264">strictEnforcement</span></span>|<span data-ttu-id="fa777-265">Логический</span><span class="sxs-lookup"><span data-stu-id="fa777-265">Boolean</span></span>|<span data-ttu-id="fa777-266">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-266">Zscaler only.</span></span> <span data-ttu-id="fa777-267">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-267">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="fa777-268">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="fa777-268">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="fa777-269">клауднаме</span><span class="sxs-lookup"><span data-stu-id="fa777-269">cloudName</span></span>|<span data-ttu-id="fa777-270">String</span><span class="sxs-lookup"><span data-stu-id="fa777-270">String</span></span>|<span data-ttu-id="fa777-271">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-271">Zscaler only.</span></span> <span data-ttu-id="fa777-272">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="fa777-272">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="fa777-273">excludeList</span><span class="sxs-lookup"><span data-stu-id="fa777-273">excludeList</span></span>|<span data-ttu-id="fa777-274">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa777-274">String collection</span></span>|<span data-ttu-id="fa777-275">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-275">Zscaler only.</span></span> <span data-ttu-id="fa777-276">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="fa777-276">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="fa777-277">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa777-277">Response</span></span>
<span data-ttu-id="fa777-278">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa777-278">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa777-279">Пример</span><span class="sxs-lookup"><span data-stu-id="fa777-279">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa777-280">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa777-280">Request</span></span>
<span data-ttu-id="fa777-281">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa777-281">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa777-282">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa777-282">Response</span></span>
<span data-ttu-id="fa777-p134">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa777-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





