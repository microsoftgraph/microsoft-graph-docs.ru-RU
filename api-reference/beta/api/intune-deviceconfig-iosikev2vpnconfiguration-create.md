---
title: Создание iosikEv2VpnConfiguration
description: Создание нового объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aff0878c6bd2a921fc5f1c40a072555a6524d383
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123129"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="a3a9d-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3a9d-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="a3a9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3a9d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3a9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3a9d-107">Создание нового объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a3a9d-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3a9d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3a9d-108">Prerequisites</span></span>
<span data-ttu-id="a3a9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3a9d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3a9d-111">Permission type</span></span>|<span data-ttu-id="a3a9d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3a9d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3a9d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3a9d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3a9d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3a9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-116">Not supported.</span></span>|
|<span data-ttu-id="a3a9d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3a9d-117">Application</span></span>|<span data-ttu-id="a3a9d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3a9d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3a9d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3a9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3a9d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a3a9d-120">Request headers</span></span>
|<span data-ttu-id="a3a9d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3a9d-121">Header</span></span>|<span data-ttu-id="a3a9d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3a9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3a9d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3a9d-123">Authorization</span></span>|<span data-ttu-id="a3a9d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3a9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3a9d-125">Accept</span></span>|<span data-ttu-id="a3a9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3a9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a9d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3a9d-127">Request body</span></span>
<span data-ttu-id="a3a9d-128">В тексте запроса добавьте представление объекта iosikEv2VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="a3a9d-129">В следующей таблице приведены свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="a3a9d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3a9d-130">Property</span></span>|<span data-ttu-id="a3a9d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a9d-131">Type</span></span>|<span data-ttu-id="a3a9d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3a9d-133">id</span><span class="sxs-lookup"><span data-stu-id="a3a9d-133">id</span></span>|<span data-ttu-id="a3a9d-134">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-134">String</span></span>|<span data-ttu-id="a3a9d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-135">Key of the entity.</span></span> <span data-ttu-id="a3a9d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3a9d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a3a9d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3a9d-138">DateTimeOffset</span></span>|<span data-ttu-id="a3a9d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a3a9d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3a9d-141">roleScopeTagIds</span></span>|<span data-ttu-id="a3a9d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-142">String collection</span></span>|<span data-ttu-id="a3a9d-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a3a9d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a3a9d-145">supportsScopeTags</span></span>|<span data-ttu-id="a3a9d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-146">Boolean</span></span>|<span data-ttu-id="a3a9d-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a3a9d-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a3a9d-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a3a9d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-150">This property is read-only.</span></span> <span data-ttu-id="a3a9d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a3a9d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a3a9d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a3a9d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a3a9d-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a3a9d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a3a9d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a3a9d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a3a9d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a3a9d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a3a9d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a3a9d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a3a9d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a3a9d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a3a9d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a3a9d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3a9d-164">createdDateTime</span></span>|<span data-ttu-id="a3a9d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3a9d-165">DateTimeOffset</span></span>|<span data-ttu-id="a3a9d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-166">DateTime the object was created.</span></span> <span data-ttu-id="a3a9d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-168">description</span><span class="sxs-lookup"><span data-stu-id="a3a9d-168">description</span></span>|<span data-ttu-id="a3a9d-169">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-169">String</span></span>|<span data-ttu-id="a3a9d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3a9d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a3a9d-172">displayName</span></span>|<span data-ttu-id="a3a9d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a3a9d-173">String</span></span>|<span data-ttu-id="a3a9d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3a9d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-176">version</span><span class="sxs-lookup"><span data-stu-id="a3a9d-176">version</span></span>|<span data-ttu-id="a3a9d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a3a9d-177">Int32</span></span>|<span data-ttu-id="a3a9d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-178">Version of the device configuration.</span></span> <span data-ttu-id="a3a9d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="a3a9d-180">connectionName</span></span>|<span data-ttu-id="a3a9d-181">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-181">String</span></span>|<span data-ttu-id="a3a9d-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-182">Connection name displayed to the user.</span></span> <span data-ttu-id="a3a9d-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="a3a9d-184">connectionType</span></span>|[<span data-ttu-id="a3a9d-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="a3a9d-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="a3a9d-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-186">Connection type.</span></span> <span data-ttu-id="a3a9d-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a3a9d-188">Возможные значения: `ciscoAnyConnect` , `pulseSecure` ,,,,, `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` ,,, `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` ,,, `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` , `microsoftTunnel` .</span><span class="sxs-lookup"><span data-stu-id="a3a9d-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="a3a9d-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="a3a9d-189">loginGroupOrDomain</span></span>|<span data-ttu-id="a3a9d-190">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-190">String</span></span>|<span data-ttu-id="a3a9d-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="a3a9d-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-193">role</span><span class="sxs-lookup"><span data-stu-id="a3a9d-193">role</span></span>|<span data-ttu-id="a3a9d-194">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-194">String</span></span>|<span data-ttu-id="a3a9d-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="a3a9d-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-197">область</span><span class="sxs-lookup"><span data-stu-id="a3a9d-197">realm</span></span>|<span data-ttu-id="a3a9d-198">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-198">String</span></span>|<span data-ttu-id="a3a9d-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="a3a9d-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-201">сервер</span><span class="sxs-lookup"><span data-stu-id="a3a9d-201">server</span></span>|[<span data-ttu-id="a3a9d-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="a3a9d-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-203">VPN Server on the network.</span></span> <span data-ttu-id="a3a9d-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="a3a9d-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="a3a9d-206">identifier</span></span>|<span data-ttu-id="a3a9d-207">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-207">String</span></span>|<span data-ttu-id="a3a9d-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a3a9d-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="a3a9d-210">customData</span></span>|<span data-ttu-id="a3a9d-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="a3a9d-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a3a9d-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a3a9d-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a3a9d-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a3a9d-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="a3a9d-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="a3a9d-217">customKeyValueData</span></span>|<span data-ttu-id="a3a9d-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a3a9d-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a3a9d-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a3a9d-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a3a9d-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a3a9d-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="a3a9d-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="a3a9d-224">enableSplitTunneling</span></span>|<span data-ttu-id="a3a9d-225">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-225">Boolean</span></span>|<span data-ttu-id="a3a9d-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="a3a9d-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="a3a9d-228">authenticationMethod</span></span>|[<span data-ttu-id="a3a9d-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="a3a9d-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="a3a9d-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="a3a9d-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a3a9d-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="a3a9d-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="a3a9d-233">enablePerApp</span></span>|<span data-ttu-id="a3a9d-234">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-234">Boolean</span></span>|<span data-ttu-id="a3a9d-235">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="a3a9d-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="a3a9d-237">safariDomains</span></span>|<span data-ttu-id="a3a9d-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-238">String collection</span></span>|<span data-ttu-id="a3a9d-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="a3a9d-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="a3a9d-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="a3a9d-242">onDemandRules</span></span>|<span data-ttu-id="a3a9d-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="a3a9d-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-244">On-Demand Rules.</span></span> <span data-ttu-id="a3a9d-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a3a9d-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-247">проксисервер</span><span class="sxs-lookup"><span data-stu-id="a3a9d-247">proxyServer</span></span>|[<span data-ttu-id="a3a9d-248">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="a3a9d-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="a3a9d-249">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-249">Proxy Server.</span></span> <span data-ttu-id="a3a9d-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-251">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="a3a9d-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="a3a9d-252">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-252">Boolean</span></span>|<span data-ttu-id="a3a9d-253">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="a3a9d-254">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-255">providerType</span><span class="sxs-lookup"><span data-stu-id="a3a9d-255">providerType</span></span>|[<span data-ttu-id="a3a9d-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="a3a9d-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="a3a9d-257">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="a3a9d-258">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="a3a9d-259">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="a3a9d-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="a3a9d-260">userDomain</span></span>|<span data-ttu-id="a3a9d-261">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-261">String</span></span>|<span data-ttu-id="a3a9d-262">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-262">Zscaler only.</span></span> <span data-ttu-id="a3a9d-263">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="a3a9d-264">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="a3a9d-265">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-266">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="a3a9d-266">strictEnforcement</span></span>|<span data-ttu-id="a3a9d-267">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-267">Boolean</span></span>|<span data-ttu-id="a3a9d-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-268">Zscaler only.</span></span> <span data-ttu-id="a3a9d-269">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="a3a9d-270">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="a3a9d-271">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-272">клауднаме</span><span class="sxs-lookup"><span data-stu-id="a3a9d-272">cloudName</span></span>|<span data-ttu-id="a3a9d-273">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-273">String</span></span>|<span data-ttu-id="a3a9d-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-274">Zscaler only.</span></span> <span data-ttu-id="a3a9d-275">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="a3a9d-276">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-277">excludeList</span><span class="sxs-lookup"><span data-stu-id="a3a9d-277">excludeList</span></span>|<span data-ttu-id="a3a9d-278">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-278">String collection</span></span>|<span data-ttu-id="a3a9d-279">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-279">Zscaler only.</span></span> <span data-ttu-id="a3a9d-280">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="a3a9d-281">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-282">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a3a9d-282">targetedMobileApps</span></span>|<span data-ttu-id="a3a9d-283">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a3a9d-284">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-284">Targeted mobile apps.</span></span> <span data-ttu-id="a3a9d-285">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-285">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a3a9d-286">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3a9d-286">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a3a9d-287">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a3a9d-287">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="a3a9d-288">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="a3a9d-288">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="a3a9d-289">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="a3a9d-289">Child Security Association Parameters</span></span>|
|<span data-ttu-id="a3a9d-290">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="a3a9d-290">clientAuthenticationType</span></span>|[<span data-ttu-id="a3a9d-291">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="a3a9d-291">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="a3a9d-292">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-292">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="a3a9d-293">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-293">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="a3a9d-294">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="a3a9d-294">deadPeerDetectionRate</span></span>|[<span data-ttu-id="a3a9d-295">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="a3a9d-295">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="a3a9d-296">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-296">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="a3a9d-297">.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-297">.</span></span> <span data-ttu-id="a3a9d-298">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-298">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="a3a9d-299">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="a3a9d-299">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="a3a9d-300">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-300">Boolean</span></span>|<span data-ttu-id="a3a9d-301">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="a3a9d-301">Disable MOBIKE</span></span>|
|<span data-ttu-id="a3a9d-302">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="a3a9d-302">disableRedirect</span></span>|<span data-ttu-id="a3a9d-303">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-303">Boolean</span></span>|<span data-ttu-id="a3a9d-304">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="a3a9d-304">Disable Redirect</span></span>|
|<span data-ttu-id="a3a9d-305">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="a3a9d-305">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="a3a9d-306">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-306">Boolean</span></span>|<span data-ttu-id="a3a9d-307">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="a3a9d-307">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="a3a9d-308">енаблиап</span><span class="sxs-lookup"><span data-stu-id="a3a9d-308">enableEAP</span></span>|<span data-ttu-id="a3a9d-309">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-309">Boolean</span></span>|<span data-ttu-id="a3a9d-310">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="a3a9d-310">Enables EAP only authentication</span></span>|
|<span data-ttu-id="a3a9d-311">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="a3a9d-311">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="a3a9d-312">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-312">Boolean</span></span>|<span data-ttu-id="a3a9d-313">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="a3a9d-313">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="a3a9d-314">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="a3a9d-314">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="a3a9d-315">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-315">Boolean</span></span>|<span data-ttu-id="a3a9d-316">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-316">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="a3a9d-317">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="a3a9d-317">localIdentifier</span></span>|[<span data-ttu-id="a3a9d-318">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="a3a9d-318">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="a3a9d-319">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-319">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="a3a9d-320">.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-320">.</span></span> <span data-ttu-id="a3a9d-321">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-321">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="a3a9d-322">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="a3a9d-322">remoteIdentifier</span></span>|<span data-ttu-id="a3a9d-323">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-323">String</span></span>|<span data-ttu-id="a3a9d-324">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-324">Address of the IKEv2 server.</span></span> <span data-ttu-id="a3a9d-325">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="a3a9d-325">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="a3a9d-326">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a3a9d-326">securityAssociationParameters</span></span>|[<span data-ttu-id="a3a9d-327">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="a3a9d-327">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="a3a9d-328">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="a3a9d-328">Security Association Parameters</span></span>|
|<span data-ttu-id="a3a9d-329">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="a3a9d-329">serverCertificateCommonName</span></span>|<span data-ttu-id="a3a9d-330">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-330">String</span></span>|<span data-ttu-id="a3a9d-331">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="a3a9d-331">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="a3a9d-332">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="a3a9d-332">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="a3a9d-333">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-333">String</span></span>|<span data-ttu-id="a3a9d-334">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="a3a9d-334">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="a3a9d-335">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="a3a9d-335">serverCertificateType</span></span>|[<span data-ttu-id="a3a9d-336">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="a3a9d-336">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="a3a9d-337">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-337">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="a3a9d-338">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-338">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="a3a9d-339">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="a3a9d-339">sharedSecret</span></span>|<span data-ttu-id="a3a9d-340">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-340">String</span></span>|<span data-ttu-id="a3a9d-341">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="a3a9d-341">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="a3a9d-342">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="a3a9d-342">tlsMaximumVersion</span></span>|<span data-ttu-id="a3a9d-343">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-343">String</span></span>|<span data-ttu-id="a3a9d-344">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="a3a9d-344">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="a3a9d-345">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="a3a9d-345">tlsMinimumVersion</span></span>|<span data-ttu-id="a3a9d-346">String</span><span class="sxs-lookup"><span data-stu-id="a3a9d-346">String</span></span>|<span data-ttu-id="a3a9d-347">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="a3a9d-347">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="a3a9d-348">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a3a9d-348">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="a3a9d-349">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-349">Boolean</span></span>|<span data-ttu-id="a3a9d-350">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-350">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="a3a9d-351">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a3a9d-351">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="a3a9d-352">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-352">Boolean</span></span>|<span data-ttu-id="a3a9d-353">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-353">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="a3a9d-354">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a3a9d-354">alwaysOnConfiguration</span></span>|[<span data-ttu-id="a3a9d-355">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3a9d-355">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="a3a9d-356">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="a3a9d-356">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="a3a9d-357">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a3a9d-357">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="a3a9d-358">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a9d-358">Boolean</span></span>|<span data-ttu-id="a3a9d-359">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="a3a9d-359">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="a3a9d-360">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3a9d-360">Response</span></span>
<span data-ttu-id="a3a9d-361">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-361">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3a9d-362">Пример</span><span class="sxs-lookup"><span data-stu-id="a3a9d-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3a9d-363">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3a9d-363">Request</span></span>
<span data-ttu-id="a3a9d-364">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-364">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5241

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
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
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```

### <a name="response"></a><span data-ttu-id="a3a9d-365">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3a9d-365">Response</span></span>
<span data-ttu-id="a3a9d-p140">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3a9d-p140">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5413

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
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
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```



