---
title: Создание iosVpnConfiguration
description: Создайте новый объект iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0eb0de1d8cd2521292533e76cea5f0fad2f9428
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129876"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="ce4cf-103">Создание iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce4cf-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="ce4cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce4cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce4cf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce4cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce4cf-107">Создайте новый [объект iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce4cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce4cf-108">Prerequisites</span></span>
<span data-ttu-id="ce4cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce4cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce4cf-111">Permission type</span></span>|<span data-ttu-id="ce4cf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce4cf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce4cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce4cf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce4cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-116">Not supported.</span></span>|
|<span data-ttu-id="ce4cf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce4cf-117">Application</span></span>|<span data-ttu-id="ce4cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce4cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce4cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce4cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce4cf-120">Request headers</span></span>
|<span data-ttu-id="ce4cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce4cf-121">Header</span></span>|<span data-ttu-id="ce4cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce4cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce4cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce4cf-123">Authorization</span></span>|<span data-ttu-id="ce4cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce4cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce4cf-125">Accept</span></span>|<span data-ttu-id="ce4cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce4cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce4cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce4cf-127">Request body</span></span>
<span data-ttu-id="ce4cf-128">В теле запроса поставляем представление JSON для объекта iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="ce4cf-129">В следующей таблице показаны свойства, необходимые при создании iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="ce4cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce4cf-130">Property</span></span>|<span data-ttu-id="ce4cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ce4cf-131">Type</span></span>|<span data-ttu-id="ce4cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ce4cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce4cf-133">id</span><span class="sxs-lookup"><span data-stu-id="ce4cf-133">id</span></span>|<span data-ttu-id="ce4cf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-134">String</span></span>|<span data-ttu-id="ce4cf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-135">Key of the entity.</span></span> <span data-ttu-id="ce4cf-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce4cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ce4cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce4cf-138">DateTimeOffset</span></span>|<span data-ttu-id="ce4cf-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ce4cf-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce4cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="ce4cf-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce4cf-142">String collection</span></span>|<span data-ttu-id="ce4cf-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce4cf-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce4cf-145">supportsScopeTags</span></span>|<span data-ttu-id="ce4cf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4cf-146">Boolean</span></span>|<span data-ttu-id="ce4cf-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce4cf-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce4cf-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce4cf-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-150">This property is read-only.</span></span> <span data-ttu-id="ce4cf-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce4cf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ce4cf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce4cf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ce4cf-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ce4cf-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce4cf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ce4cf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce4cf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ce4cf-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ce4cf-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce4cf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ce4cf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce4cf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ce4cf-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ce4cf-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce4cf-164">createdDateTime</span></span>|<span data-ttu-id="ce4cf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce4cf-165">DateTimeOffset</span></span>|<span data-ttu-id="ce4cf-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-166">DateTime the object was created.</span></span> <span data-ttu-id="ce4cf-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-168">description</span><span class="sxs-lookup"><span data-stu-id="ce4cf-168">description</span></span>|<span data-ttu-id="ce4cf-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-169">String</span></span>|<span data-ttu-id="ce4cf-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce4cf-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ce4cf-172">displayName</span></span>|<span data-ttu-id="ce4cf-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-173">String</span></span>|<span data-ttu-id="ce4cf-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce4cf-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-176">version</span><span class="sxs-lookup"><span data-stu-id="ce4cf-176">version</span></span>|<span data-ttu-id="ce4cf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ce4cf-177">Int32</span></span>|<span data-ttu-id="ce4cf-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-178">Version of the device configuration.</span></span> <span data-ttu-id="ce4cf-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="ce4cf-180">connectionName</span></span>|<span data-ttu-id="ce4cf-181">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-181">String</span></span>|<span data-ttu-id="ce4cf-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-182">Connection name displayed to the user.</span></span> <span data-ttu-id="ce4cf-183">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="ce4cf-184">connectionType</span></span>|[<span data-ttu-id="ce4cf-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ce4cf-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ce4cf-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-186">Connection type.</span></span> <span data-ttu-id="ce4cf-187">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ce4cf-188">Возможные значения: `ciscoAnyConnect` `pulseSecure` , , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` , , `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="ce4cf-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="ce4cf-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ce4cf-189">loginGroupOrDomain</span></span>|<span data-ttu-id="ce4cf-190">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-190">String</span></span>|<span data-ttu-id="ce4cf-191">Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ce4cf-192">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-193">role</span><span class="sxs-lookup"><span data-stu-id="ce4cf-193">role</span></span>|<span data-ttu-id="ce4cf-194">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-194">String</span></span>|<span data-ttu-id="ce4cf-195">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ce4cf-196">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-197">realm</span><span class="sxs-lookup"><span data-stu-id="ce4cf-197">realm</span></span>|<span data-ttu-id="ce4cf-198">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-198">String</span></span>|<span data-ttu-id="ce4cf-199">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ce4cf-200">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-201">сервер</span><span class="sxs-lookup"><span data-stu-id="ce4cf-201">server</span></span>|[<span data-ttu-id="ce4cf-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="ce4cf-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ce4cf-203">VPN Server в сети.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-203">VPN Server on the network.</span></span> <span data-ttu-id="ce4cf-204">Убедитесь, что конечные пользователи могут получить доступ к этому расположению сети.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="ce4cf-205">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="ce4cf-206">identifier</span></span>|<span data-ttu-id="ce4cf-207">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-207">String</span></span>|<span data-ttu-id="ce4cf-208">Идентификатор, предоставляемый поставщиком VPN при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ce4cf-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin, унаследованный от [appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-210">customData</span><span class="sxs-lookup"><span data-stu-id="ce4cf-210">customData</span></span>|<span data-ttu-id="ce4cf-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ce4cf-212">Настраиваемые данные при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ce4cf-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ce4cf-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ce4cf-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ce4cf-216">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ce4cf-217">customKeyValueData</span></span>|<span data-ttu-id="ce4cf-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ce4cf-219">Настраиваемые данные при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ce4cf-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ce4cf-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ce4cf-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ce4cf-223">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ce4cf-224">enableSplitTunneling</span></span>|<span data-ttu-id="ce4cf-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4cf-225">Boolean</span></span>|<span data-ttu-id="ce4cf-226">Отправка всего сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="ce4cf-227">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ce4cf-228">authenticationMethod</span></span>|[<span data-ttu-id="ce4cf-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ce4cf-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ce4cf-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ce4cf-231">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ce4cf-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ce4cf-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="ce4cf-233">enablePerApp</span></span>|<span data-ttu-id="ce4cf-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4cf-234">Boolean</span></span>|<span data-ttu-id="ce4cf-235">Настройка этого параметра создает Per-App, которая впоследствии может быть связана с приложениями, которые могут запускать этот VPN-коннекцитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ce4cf-236">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="ce4cf-237">safariDomains</span></span>|<span data-ttu-id="ce4cf-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce4cf-238">String collection</span></span>|<span data-ttu-id="ce4cf-239">Домены Safari при включении этого параметра VPN для приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ce4cf-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ce4cf-241">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="ce4cf-242">onDemandRules</span></span>|<span data-ttu-id="ce4cf-243">[коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ce4cf-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-244">On-Demand Rules.</span></span> <span data-ttu-id="ce4cf-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ce4cf-246">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-247">providerType</span><span class="sxs-lookup"><span data-stu-id="ce4cf-247">providerType</span></span>|[<span data-ttu-id="ce4cf-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="ce4cf-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="ce4cf-249">Тип поставщика для VPN-приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="ce4cf-250">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce4cf-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ce4cf-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="ce4cf-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="ce4cf-252">associatedDomains</span></span>|<span data-ttu-id="ce4cf-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce4cf-253">String collection</span></span>|<span data-ttu-id="ce4cf-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="ce4cf-255">excludedDomains</span></span>|<span data-ttu-id="ce4cf-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce4cf-256">String collection</span></span>|<span data-ttu-id="ce4cf-257">Домены, которые доступны через общедоступный интернет, а не через VPN, даже если VPN для каждого приложения активируется, наследуется [из appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="ce4cf-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="ce4cf-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4cf-259">Boolean</span></span>|<span data-ttu-id="ce4cf-260">Переключение, чтобы предотвратить отключение автоматического VPN в приложении "Параметры", унаследованных от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ce4cf-261">proxyServer</span></span>|[<span data-ttu-id="ce4cf-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ce4cf-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ce4cf-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-263">Proxy Server.</span></span> <span data-ttu-id="ce4cf-264">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="ce4cf-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ce4cf-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4cf-266">Boolean</span></span>|<span data-ttu-id="ce4cf-267">Opt-In совместное использование Id устройства сторонним vpn-клиентам для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ce4cf-268">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ce4cf-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="ce4cf-269">userDomain</span></span>|<span data-ttu-id="ce4cf-270">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-270">String</span></span>|<span data-ttu-id="ce4cf-271">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-271">Zscaler only.</span></span> <span data-ttu-id="ce4cf-272">Введите статический домен для предварительного заполнения поля входа в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="ce4cf-273">Если этот домен останется пустым, вместо него будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="ce4cf-274">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="ce4cf-274">strictEnforcement</span></span>|<span data-ttu-id="ce4cf-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4cf-275">Boolean</span></span>|<span data-ttu-id="ce4cf-276">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-276">Zscaler only.</span></span> <span data-ttu-id="ce4cf-277">Блокирует сетевой трафик до тех пор, пока пользователь не впишется в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-277">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="ce4cf-278">"True" означает, что трафик заблокирован.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-278">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="ce4cf-279">cloudName</span><span class="sxs-lookup"><span data-stu-id="ce4cf-279">cloudName</span></span>|<span data-ttu-id="ce4cf-280">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-280">String</span></span>|<span data-ttu-id="ce4cf-281">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-281">Zscaler only.</span></span> <span data-ttu-id="ce4cf-282">Облако Zscaler, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-282">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="ce4cf-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="ce4cf-283">excludeList</span></span>|<span data-ttu-id="ce4cf-284">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce4cf-284">String collection</span></span>|<span data-ttu-id="ce4cf-285">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-285">Zscaler only.</span></span> <span data-ttu-id="ce4cf-286">Список сетевых адресов, которые не отправляются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-286">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="ce4cf-287">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ce4cf-287">targetedMobileApps</span></span>|<span data-ttu-id="ce4cf-288">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ce4cf-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ce4cf-289">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-289">Targeted mobile apps.</span></span> <span data-ttu-id="ce4cf-290">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-290">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ce4cf-291">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="ce4cf-291">microsoftTunnelSiteId</span></span>|<span data-ttu-id="ce4cf-292">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4cf-292">String</span></span>|<span data-ttu-id="ce4cf-293">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-293">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="ce4cf-294">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce4cf-294">Response</span></span>
<span data-ttu-id="ce4cf-295">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-295">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce4cf-296">Пример</span><span class="sxs-lookup"><span data-stu-id="ce4cf-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce4cf-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce4cf-297">Request</span></span>
<span data-ttu-id="ce4cf-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3298

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
  "providerType": "appProxy",
  "associatedDomains": [
    "Associated Domains value"
  ],
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
  "optInToDeviceIdSharing": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="ce4cf-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce4cf-299">Response</span></span>
<span data-ttu-id="ce4cf-p135">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce4cf-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3470

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
  "providerType": "appProxy",
  "associatedDomains": [
    "Associated Domains value"
  ],
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
  "optInToDeviceIdSharing": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




