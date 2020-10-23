---
title: Создание Макосвпнконфигуратион
description: Создание нового объекта Макосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 364191ec5834c1308c5efd883e44dab47adc450f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709595"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="8f109-103">Создание Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8f109-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="8f109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f109-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f109-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f109-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f109-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f109-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f109-107">Создание нового объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8f109-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f109-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f109-108">Prerequisites</span></span>
<span data-ttu-id="8f109-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f109-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f109-111">Permission type</span></span>|<span data-ttu-id="8f109-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f109-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f109-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f109-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f109-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f109-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f109-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f109-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f109-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f109-116">Not supported.</span></span>|
|<span data-ttu-id="8f109-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f109-117">Application</span></span>|<span data-ttu-id="8f109-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f109-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f109-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f109-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f109-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8f109-120">Request headers</span></span>
|<span data-ttu-id="8f109-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f109-121">Header</span></span>|<span data-ttu-id="8f109-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f109-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f109-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f109-123">Authorization</span></span>|<span data-ttu-id="8f109-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f109-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f109-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f109-125">Accept</span></span>|<span data-ttu-id="8f109-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f109-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f109-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f109-127">Request body</span></span>
<span data-ttu-id="8f109-128">В тексте запроса добавьте представление объекта Макосвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f109-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="8f109-129">В следующей таблице приведены свойства, необходимые при создании Макосвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="8f109-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="8f109-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f109-130">Property</span></span>|<span data-ttu-id="8f109-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f109-131">Type</span></span>|<span data-ttu-id="8f109-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f109-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f109-133">id</span><span class="sxs-lookup"><span data-stu-id="8f109-133">id</span></span>|<span data-ttu-id="8f109-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-134">String</span></span>|<span data-ttu-id="8f109-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f109-135">Key of the entity.</span></span> <span data-ttu-id="8f109-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f109-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8f109-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f109-138">DateTimeOffset</span></span>|<span data-ttu-id="8f109-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8f109-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8f109-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f109-141">roleScopeTagIds</span></span>|<span data-ttu-id="8f109-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8f109-142">String collection</span></span>|<span data-ttu-id="8f109-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8f109-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8f109-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8f109-145">supportsScopeTags</span></span>|<span data-ttu-id="8f109-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8f109-146">Boolean</span></span>|<span data-ttu-id="8f109-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8f109-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8f109-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8f109-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8f109-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8f109-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8f109-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f109-150">This property is read-only.</span></span> <span data-ttu-id="8f109-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8f109-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8f109-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8f109-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8f109-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8f109-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8f109-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8f109-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8f109-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8f109-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8f109-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8f109-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8f109-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8f109-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8f109-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8f109-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8f109-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8f109-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8f109-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f109-164">createdDateTime</span></span>|<span data-ttu-id="8f109-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f109-165">DateTimeOffset</span></span>|<span data-ttu-id="8f109-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8f109-166">DateTime the object was created.</span></span> <span data-ttu-id="8f109-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-168">description</span><span class="sxs-lookup"><span data-stu-id="8f109-168">description</span></span>|<span data-ttu-id="8f109-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-169">String</span></span>|<span data-ttu-id="8f109-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8f109-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f109-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8f109-172">displayName</span></span>|<span data-ttu-id="8f109-173">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-173">String</span></span>|<span data-ttu-id="8f109-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8f109-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f109-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-176">version</span><span class="sxs-lookup"><span data-stu-id="8f109-176">version</span></span>|<span data-ttu-id="8f109-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8f109-177">Int32</span></span>|<span data-ttu-id="8f109-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8f109-178">Version of the device configuration.</span></span> <span data-ttu-id="8f109-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="8f109-180">connectionName</span></span>|<span data-ttu-id="8f109-181">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-181">String</span></span>|<span data-ttu-id="8f109-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f109-182">Connection name displayed to the user.</span></span> <span data-ttu-id="8f109-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="8f109-184">connectionType</span></span>|[<span data-ttu-id="8f109-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="8f109-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="8f109-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="8f109-186">Connection type.</span></span> <span data-ttu-id="8f109-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8f109-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="8f109-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="8f109-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="8f109-189">loginGroupOrDomain</span></span>|<span data-ttu-id="8f109-190">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-190">String</span></span>|<span data-ttu-id="8f109-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="8f109-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="8f109-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-193">role</span><span class="sxs-lookup"><span data-stu-id="8f109-193">role</span></span>|<span data-ttu-id="8f109-194">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-194">String</span></span>|<span data-ttu-id="8f109-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="8f109-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="8f109-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-197">область</span><span class="sxs-lookup"><span data-stu-id="8f109-197">realm</span></span>|<span data-ttu-id="8f109-198">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-198">String</span></span>|<span data-ttu-id="8f109-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="8f109-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="8f109-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-201">сервер</span><span class="sxs-lookup"><span data-stu-id="8f109-201">server</span></span>|[<span data-ttu-id="8f109-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="8f109-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="8f109-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="8f109-203">VPN Server on the network.</span></span> <span data-ttu-id="8f109-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="8f109-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="8f109-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="8f109-206">identifier</span></span>|<span data-ttu-id="8f109-207">Строка</span><span class="sxs-lookup"><span data-stu-id="8f109-207">String</span></span>|<span data-ttu-id="8f109-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="8f109-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8f109-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="8f109-210">customData</span></span>|<span data-ttu-id="8f109-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="8f109-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="8f109-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8f109-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="8f109-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="8f109-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="8f109-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="8f109-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="8f109-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="8f109-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="8f109-217">customKeyValueData</span></span>|<span data-ttu-id="8f109-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8f109-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="8f109-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8f109-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="8f109-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="8f109-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="8f109-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="8f109-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="8f109-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="8f109-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="8f109-224">enableSplitTunneling</span></span>|<span data-ttu-id="8f109-225">Логический</span><span class="sxs-lookup"><span data-stu-id="8f109-225">Boolean</span></span>|<span data-ttu-id="8f109-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="8f109-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="8f109-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="8f109-228">authenticationMethod</span></span>|[<span data-ttu-id="8f109-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="8f109-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="8f109-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="8f109-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="8f109-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8f109-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="8f109-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="8f109-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="8f109-233">enablePerApp</span></span>|<span data-ttu-id="8f109-234">Логический</span><span class="sxs-lookup"><span data-stu-id="8f109-234">Boolean</span></span>|<span data-ttu-id="8f109-235">Если задать для этого параметра значение true, будут созданы Per-App полезные данные VPN, которые позже могут быть связаны с приложениями, которые могут запускать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f109-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="8f109-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="8f109-237">safariDomains</span></span>|<span data-ttu-id="8f109-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8f109-238">String collection</span></span>|<span data-ttu-id="8f109-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="8f109-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="8f109-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="8f109-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="8f109-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="8f109-242">onDemandRules</span></span>|<span data-ttu-id="8f109-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="8f109-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="8f109-244">On-Demand Rules.</span></span> <span data-ttu-id="8f109-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8f109-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8f109-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-247">providerType</span><span class="sxs-lookup"><span data-stu-id="8f109-247">providerType</span></span>|[<span data-ttu-id="8f109-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="8f109-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="8f109-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="8f109-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="8f109-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f109-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8f109-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="8f109-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="8f109-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="8f109-252">excludedDomains</span></span>|<span data-ttu-id="8f109-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8f109-253">String collection</span></span>|<span data-ttu-id="8f109-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="8f109-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="8f109-256">Логический</span><span class="sxs-lookup"><span data-stu-id="8f109-256">Boolean</span></span>|<span data-ttu-id="8f109-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="8f109-258">proxyServer</span></span>|[<span data-ttu-id="8f109-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="8f109-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="8f109-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="8f109-260">Proxy Server.</span></span> <span data-ttu-id="8f109-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8f109-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="8f109-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="8f109-263">Логический</span><span class="sxs-lookup"><span data-stu-id="8f109-263">Boolean</span></span>|<span data-ttu-id="8f109-264">Opt-In для предоставления доступа к идентификатору устройства сторонним VPN-клиентам для использования в процессе проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="8f109-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="8f109-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f109-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8f109-266">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f109-266">Response</span></span>
<span data-ttu-id="8f109-267">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f109-267">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f109-268">Пример</span><span class="sxs-lookup"><span data-stu-id="8f109-268">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f109-269">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f109-269">Request</span></span>
<span data-ttu-id="8f109-270">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f109-270">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2761

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="8f109-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f109-271">Response</span></span>
<span data-ttu-id="8f109-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f109-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2933

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```





