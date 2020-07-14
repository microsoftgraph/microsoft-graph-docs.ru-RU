---
title: Создание Иосвпнконфигуратион
description: Создание нового объекта Иосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b1dcad6f33c7bba7c6690b580ad984217884423
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123045"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="3dd90-103">Создание Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3dd90-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="3dd90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dd90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3dd90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dd90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3dd90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dd90-107">Создание нового объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3dd90-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dd90-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3dd90-108">Prerequisites</span></span>
<span data-ttu-id="3dd90-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3dd90-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3dd90-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dd90-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dd90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dd90-111">Permission type</span></span>|<span data-ttu-id="3dd90-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dd90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dd90-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dd90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3dd90-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dd90-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3dd90-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dd90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dd90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd90-116">Not supported.</span></span>|
|<span data-ttu-id="3dd90-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3dd90-117">Application</span></span>|<span data-ttu-id="3dd90-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dd90-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dd90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dd90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3dd90-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3dd90-120">Request headers</span></span>
|<span data-ttu-id="3dd90-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3dd90-121">Header</span></span>|<span data-ttu-id="3dd90-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3dd90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dd90-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3dd90-123">Authorization</span></span>|<span data-ttu-id="3dd90-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dd90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dd90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3dd90-125">Accept</span></span>|<span data-ttu-id="3dd90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dd90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dd90-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3dd90-127">Request body</span></span>
<span data-ttu-id="3dd90-128">В тексте запроса добавьте представление объекта Иосвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3dd90-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="3dd90-129">В следующей таблице приведены свойства, необходимые при создании Иосвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="3dd90-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="3dd90-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dd90-130">Property</span></span>|<span data-ttu-id="3dd90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3dd90-131">Type</span></span>|<span data-ttu-id="3dd90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dd90-133">id</span><span class="sxs-lookup"><span data-stu-id="3dd90-133">id</span></span>|<span data-ttu-id="3dd90-134">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-134">String</span></span>|<span data-ttu-id="3dd90-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3dd90-135">Key of the entity.</span></span> <span data-ttu-id="3dd90-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dd90-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3dd90-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dd90-138">DateTimeOffset</span></span>|<span data-ttu-id="3dd90-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3dd90-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3dd90-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3dd90-141">roleScopeTagIds</span></span>|<span data-ttu-id="3dd90-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3dd90-142">String collection</span></span>|<span data-ttu-id="3dd90-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3dd90-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3dd90-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3dd90-145">supportsScopeTags</span></span>|<span data-ttu-id="3dd90-146">Логический</span><span class="sxs-lookup"><span data-stu-id="3dd90-146">Boolean</span></span>|<span data-ttu-id="3dd90-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3dd90-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3dd90-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3dd90-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3dd90-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3dd90-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3dd90-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3dd90-150">This property is read-only.</span></span> <span data-ttu-id="3dd90-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3dd90-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3dd90-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3dd90-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3dd90-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3dd90-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3dd90-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3dd90-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3dd90-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3dd90-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3dd90-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3dd90-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3dd90-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3dd90-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3dd90-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3dd90-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3dd90-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3dd90-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3dd90-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dd90-164">createdDateTime</span></span>|<span data-ttu-id="3dd90-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dd90-165">DateTimeOffset</span></span>|<span data-ttu-id="3dd90-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3dd90-166">DateTime the object was created.</span></span> <span data-ttu-id="3dd90-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-168">description</span><span class="sxs-lookup"><span data-stu-id="3dd90-168">description</span></span>|<span data-ttu-id="3dd90-169">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-169">String</span></span>|<span data-ttu-id="3dd90-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3dd90-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3dd90-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3dd90-172">displayName</span></span>|<span data-ttu-id="3dd90-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3dd90-173">String</span></span>|<span data-ttu-id="3dd90-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3dd90-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3dd90-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-176">version</span><span class="sxs-lookup"><span data-stu-id="3dd90-176">version</span></span>|<span data-ttu-id="3dd90-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3dd90-177">Int32</span></span>|<span data-ttu-id="3dd90-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3dd90-178">Version of the device configuration.</span></span> <span data-ttu-id="3dd90-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="3dd90-180">connectionName</span></span>|<span data-ttu-id="3dd90-181">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-181">String</span></span>|<span data-ttu-id="3dd90-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dd90-182">Connection name displayed to the user.</span></span> <span data-ttu-id="3dd90-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="3dd90-184">connectionType</span></span>|[<span data-ttu-id="3dd90-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="3dd90-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="3dd90-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="3dd90-186">Connection type.</span></span> <span data-ttu-id="3dd90-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="3dd90-188">Возможные значения: `ciscoAnyConnect` , `pulseSecure` ,,,,, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` ,,, `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` ,,, `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` , `microsoftTunnel` .</span><span class="sxs-lookup"><span data-stu-id="3dd90-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="3dd90-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="3dd90-189">loginGroupOrDomain</span></span>|<span data-ttu-id="3dd90-190">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-190">String</span></span>|<span data-ttu-id="3dd90-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="3dd90-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="3dd90-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-193">role</span><span class="sxs-lookup"><span data-stu-id="3dd90-193">role</span></span>|<span data-ttu-id="3dd90-194">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-194">String</span></span>|<span data-ttu-id="3dd90-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="3dd90-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3dd90-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-197">область</span><span class="sxs-lookup"><span data-stu-id="3dd90-197">realm</span></span>|<span data-ttu-id="3dd90-198">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-198">String</span></span>|<span data-ttu-id="3dd90-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="3dd90-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3dd90-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-201">сервер</span><span class="sxs-lookup"><span data-stu-id="3dd90-201">server</span></span>|[<span data-ttu-id="3dd90-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="3dd90-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="3dd90-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="3dd90-203">VPN Server on the network.</span></span> <span data-ttu-id="3dd90-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="3dd90-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="3dd90-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="3dd90-206">identifier</span></span>|<span data-ttu-id="3dd90-207">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-207">String</span></span>|<span data-ttu-id="3dd90-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="3dd90-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3dd90-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="3dd90-210">customData</span></span>|<span data-ttu-id="3dd90-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="3dd90-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="3dd90-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3dd90-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="3dd90-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3dd90-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="3dd90-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3dd90-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="3dd90-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="3dd90-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="3dd90-217">customKeyValueData</span></span>|<span data-ttu-id="3dd90-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3dd90-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="3dd90-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3dd90-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="3dd90-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3dd90-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="3dd90-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3dd90-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="3dd90-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="3dd90-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="3dd90-224">enableSplitTunneling</span></span>|<span data-ttu-id="3dd90-225">Логический</span><span class="sxs-lookup"><span data-stu-id="3dd90-225">Boolean</span></span>|<span data-ttu-id="3dd90-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="3dd90-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="3dd90-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="3dd90-228">authenticationMethod</span></span>|[<span data-ttu-id="3dd90-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="3dd90-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3dd90-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="3dd90-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="3dd90-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3dd90-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="3dd90-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="3dd90-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="3dd90-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="3dd90-233">enablePerApp</span></span>|<span data-ttu-id="3dd90-234">Логический</span><span class="sxs-lookup"><span data-stu-id="3dd90-234">Boolean</span></span>|<span data-ttu-id="3dd90-235">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dd90-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="3dd90-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="3dd90-237">safariDomains</span></span>|<span data-ttu-id="3dd90-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3dd90-238">String collection</span></span>|<span data-ttu-id="3dd90-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="3dd90-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="3dd90-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="3dd90-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="3dd90-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="3dd90-242">onDemandRules</span></span>|<span data-ttu-id="3dd90-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="3dd90-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="3dd90-244">On-Demand Rules.</span></span> <span data-ttu-id="3dd90-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3dd90-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3dd90-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-247">проксисервер</span><span class="sxs-lookup"><span data-stu-id="3dd90-247">proxyServer</span></span>|[<span data-ttu-id="3dd90-248">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="3dd90-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="3dd90-249">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-249">Proxy Server.</span></span> <span data-ttu-id="3dd90-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-251">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="3dd90-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="3dd90-252">Логический</span><span class="sxs-lookup"><span data-stu-id="3dd90-252">Boolean</span></span>|<span data-ttu-id="3dd90-253">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="3dd90-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="3dd90-254">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3dd90-255">providerType</span><span class="sxs-lookup"><span data-stu-id="3dd90-255">providerType</span></span>|[<span data-ttu-id="3dd90-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="3dd90-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="3dd90-257">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="3dd90-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="3dd90-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="3dd90-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="3dd90-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="3dd90-259">userDomain</span></span>|<span data-ttu-id="3dd90-260">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-260">String</span></span>|<span data-ttu-id="3dd90-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-261">Zscaler only.</span></span> <span data-ttu-id="3dd90-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="3dd90-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dd90-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="3dd90-264">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="3dd90-264">strictEnforcement</span></span>|<span data-ttu-id="3dd90-265">Логический</span><span class="sxs-lookup"><span data-stu-id="3dd90-265">Boolean</span></span>|<span data-ttu-id="3dd90-266">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-266">Zscaler only.</span></span> <span data-ttu-id="3dd90-267">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-267">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="3dd90-268">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="3dd90-268">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="3dd90-269">клауднаме</span><span class="sxs-lookup"><span data-stu-id="3dd90-269">cloudName</span></span>|<span data-ttu-id="3dd90-270">String</span><span class="sxs-lookup"><span data-stu-id="3dd90-270">String</span></span>|<span data-ttu-id="3dd90-271">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-271">Zscaler only.</span></span> <span data-ttu-id="3dd90-272">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="3dd90-272">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="3dd90-273">excludeList</span><span class="sxs-lookup"><span data-stu-id="3dd90-273">excludeList</span></span>|<span data-ttu-id="3dd90-274">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3dd90-274">String collection</span></span>|<span data-ttu-id="3dd90-275">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-275">Zscaler only.</span></span> <span data-ttu-id="3dd90-276">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="3dd90-276">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="3dd90-277">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3dd90-277">targetedMobileApps</span></span>|<span data-ttu-id="3dd90-278">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3dd90-278">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3dd90-279">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="3dd90-279">Targeted mobile apps.</span></span> <span data-ttu-id="3dd90-280">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3dd90-280">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3dd90-281">Ответ</span><span class="sxs-lookup"><span data-stu-id="3dd90-281">Response</span></span>
<span data-ttu-id="3dd90-282">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3dd90-282">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dd90-283">Пример</span><span class="sxs-lookup"><span data-stu-id="3dd90-283">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dd90-284">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dd90-284">Request</span></span>
<span data-ttu-id="3dd90-285">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3dd90-285">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3072

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
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3dd90-286">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dd90-286">Response</span></span>
<span data-ttu-id="3dd90-287">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3dd90-287">Here is an example of the response.</span></span> <span data-ttu-id="3dd90-288">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3dd90-288">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3dd90-289">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3dd90-289">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3244

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
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```



