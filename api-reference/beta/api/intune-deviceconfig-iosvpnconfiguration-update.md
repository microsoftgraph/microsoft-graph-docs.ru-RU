---
title: Обновление Иосвпнконфигуратион
description: Обновление свойств объекта Иосвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96a22e4fc2e12f4bc9bdf480f6722d01615ba9cc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977046"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="e7da9-103">Обновление Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e7da9-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="e7da9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7da9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7da9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7da9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7da9-106">Обновление свойств объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e7da9-106">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7da9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e7da9-107">Prerequisites</span></span>
<span data-ttu-id="e7da9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7da9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7da9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7da9-110">Permission type</span></span>|<span data-ttu-id="e7da9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7da9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7da9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7da9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7da9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7da9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7da9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7da9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7da9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7da9-115">Not supported.</span></span>|
|<span data-ttu-id="e7da9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7da9-116">Application</span></span>|<span data-ttu-id="e7da9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7da9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7da9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7da9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7da9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7da9-119">Request headers</span></span>
|<span data-ttu-id="e7da9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7da9-120">Header</span></span>|<span data-ttu-id="e7da9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e7da9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7da9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7da9-122">Authorization</span></span>|<span data-ttu-id="e7da9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7da9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7da9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7da9-124">Accept</span></span>|<span data-ttu-id="e7da9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7da9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7da9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7da9-126">Request body</span></span>
<span data-ttu-id="e7da9-127">В тексте запроса добавьте представление объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7da9-127">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="e7da9-128">В следующей таблице приведены свойства, необходимые при создании [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-128">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="e7da9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7da9-129">Property</span></span>|<span data-ttu-id="e7da9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7da9-130">Type</span></span>|<span data-ttu-id="e7da9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7da9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7da9-132">id</span><span class="sxs-lookup"><span data-stu-id="e7da9-132">id</span></span>|<span data-ttu-id="e7da9-133">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-133">String</span></span>|<span data-ttu-id="e7da9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7da9-134">Key of the entity.</span></span> <span data-ttu-id="e7da9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7da9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7da9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7da9-137">DateTimeOffset</span></span>|<span data-ttu-id="e7da9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e7da9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7da9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7da9-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7da9-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7da9-141">String collection</span></span>|<span data-ttu-id="e7da9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e7da9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7da9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e7da9-144">supportsScopeTags</span></span>|<span data-ttu-id="e7da9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7da9-145">Boolean</span></span>|<span data-ttu-id="e7da9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e7da9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7da9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e7da9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7da9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e7da9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7da9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7da9-149">This property is read-only.</span></span> <span data-ttu-id="e7da9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7da9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e7da9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7da9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e7da9-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e7da9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e7da9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7da9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e7da9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7da9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e7da9-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e7da9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e7da9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e7da9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e7da9-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e7da9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e7da9-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e7da9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e7da9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7da9-163">createdDateTime</span></span>|<span data-ttu-id="e7da9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7da9-164">DateTimeOffset</span></span>|<span data-ttu-id="e7da9-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e7da9-165">DateTime the object was created.</span></span> <span data-ttu-id="e7da9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-167">description</span><span class="sxs-lookup"><span data-stu-id="e7da9-167">description</span></span>|<span data-ttu-id="e7da9-168">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-168">String</span></span>|<span data-ttu-id="e7da9-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7da9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7da9-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e7da9-171">displayName</span></span>|<span data-ttu-id="e7da9-172">Строка</span><span class="sxs-lookup"><span data-stu-id="e7da9-172">String</span></span>|<span data-ttu-id="e7da9-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7da9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7da9-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-175">version</span><span class="sxs-lookup"><span data-stu-id="e7da9-175">version</span></span>|<span data-ttu-id="e7da9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e7da9-176">Int32</span></span>|<span data-ttu-id="e7da9-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7da9-177">Version of the device configuration.</span></span> <span data-ttu-id="e7da9-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-179">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="e7da9-179">connectionName</span></span>|<span data-ttu-id="e7da9-180">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-180">String</span></span>|<span data-ttu-id="e7da9-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7da9-181">Connection name displayed to the user.</span></span> <span data-ttu-id="e7da9-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="e7da9-183">connectionType</span></span>|[<span data-ttu-id="e7da9-184">Апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="e7da9-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="e7da9-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="e7da9-185">Connection type.</span></span> <span data-ttu-id="e7da9-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e7da9-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,. `ikEv2`</span><span class="sxs-lookup"><span data-stu-id="e7da9-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="e7da9-188">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="e7da9-188">loginGroupOrDomain</span></span>|<span data-ttu-id="e7da9-189">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-189">String</span></span>|<span data-ttu-id="e7da9-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="e7da9-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="e7da9-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-192">role</span><span class="sxs-lookup"><span data-stu-id="e7da9-192">role</span></span>|<span data-ttu-id="e7da9-193">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-193">String</span></span>|<span data-ttu-id="e7da9-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e7da9-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e7da9-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-196">область</span><span class="sxs-lookup"><span data-stu-id="e7da9-196">realm</span></span>|<span data-ttu-id="e7da9-197">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-197">String</span></span>|<span data-ttu-id="e7da9-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e7da9-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e7da9-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-200">сервер</span><span class="sxs-lookup"><span data-stu-id="e7da9-200">server</span></span>|[<span data-ttu-id="e7da9-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="e7da9-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="e7da9-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="e7da9-202">VPN Server on the network.</span></span> <span data-ttu-id="e7da9-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="e7da9-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="e7da9-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="e7da9-205">identifier</span></span>|<span data-ttu-id="e7da9-206">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-206">String</span></span>|<span data-ttu-id="e7da9-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="e7da9-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e7da9-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="e7da9-209">customData</span></span>|<span data-ttu-id="e7da9-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e7da9-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e7da9-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e7da9-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e7da9-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e7da9-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e7da9-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e7da9-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e7da9-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e7da9-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e7da9-216">customKeyValueData</span></span>|<span data-ttu-id="e7da9-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e7da9-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e7da9-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e7da9-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e7da9-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e7da9-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e7da9-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e7da9-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e7da9-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e7da9-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-223">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="e7da9-223">enableSplitTunneling</span></span>|<span data-ttu-id="e7da9-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7da9-224">Boolean</span></span>|<span data-ttu-id="e7da9-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="e7da9-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="e7da9-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e7da9-227">authenticationMethod</span></span>|[<span data-ttu-id="e7da9-228">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e7da9-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e7da9-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="e7da9-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="e7da9-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7da9-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e7da9-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e7da9-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e7da9-232">Енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="e7da9-232">enablePerApp</span></span>|<span data-ttu-id="e7da9-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7da9-233">Boolean</span></span>|<span data-ttu-id="e7da9-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7da9-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="e7da9-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-236">Сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="e7da9-236">safariDomains</span></span>|<span data-ttu-id="e7da9-237">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7da9-237">String collection</span></span>|<span data-ttu-id="e7da9-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="e7da9-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="e7da9-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="e7da9-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="e7da9-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-241">Ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="e7da9-241">onDemandRules</span></span>|<span data-ttu-id="e7da9-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="e7da9-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="e7da9-243">On-Demand Rules.</span></span> <span data-ttu-id="e7da9-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e7da9-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e7da9-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="e7da9-246">proxyServer</span></span>|[<span data-ttu-id="e7da9-247">Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="e7da9-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="e7da9-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-248">Proxy Server.</span></span> <span data-ttu-id="e7da9-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-250">Оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="e7da9-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="e7da9-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7da9-251">Boolean</span></span>|<span data-ttu-id="e7da9-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="e7da9-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="e7da9-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7da9-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e7da9-254">providerType</span><span class="sxs-lookup"><span data-stu-id="e7da9-254">providerType</span></span>|[<span data-ttu-id="e7da9-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="e7da9-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="e7da9-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="e7da9-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="e7da9-257">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="e7da9-257">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="e7da9-258">userDomain</span><span class="sxs-lookup"><span data-stu-id="e7da9-258">userDomain</span></span>|<span data-ttu-id="e7da9-259">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-259">String</span></span>|<span data-ttu-id="e7da9-260">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-260">Zscaler only.</span></span> <span data-ttu-id="e7da9-261">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-261">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="e7da9-262">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7da9-262">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="e7da9-263">Стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="e7da9-263">strictEnforcement</span></span>|<span data-ttu-id="e7da9-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7da9-264">Boolean</span></span>|<span data-ttu-id="e7da9-265">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-265">Zscaler only.</span></span> <span data-ttu-id="e7da9-266">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-266">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="e7da9-267">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="e7da9-267">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="e7da9-268">Клауднаме</span><span class="sxs-lookup"><span data-stu-id="e7da9-268">cloudName</span></span>|<span data-ttu-id="e7da9-269">String</span><span class="sxs-lookup"><span data-stu-id="e7da9-269">String</span></span>|<span data-ttu-id="e7da9-270">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-270">Zscaler only.</span></span> <span data-ttu-id="e7da9-271">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="e7da9-271">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="e7da9-272">excludeList</span><span class="sxs-lookup"><span data-stu-id="e7da9-272">excludeList</span></span>|<span data-ttu-id="e7da9-273">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7da9-273">String collection</span></span>|<span data-ttu-id="e7da9-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-274">Zscaler only.</span></span> <span data-ttu-id="e7da9-275">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e7da9-275">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="e7da9-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7da9-276">Response</span></span>
<span data-ttu-id="e7da9-277">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7da9-277">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7da9-278">Пример</span><span class="sxs-lookup"><span data-stu-id="e7da9-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7da9-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7da9-279">Request</span></span>
<span data-ttu-id="e7da9-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7da9-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="e7da9-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7da9-281">Response</span></span>
<span data-ttu-id="e7da9-p134">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7da9-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





