---
title: Создание androidDeviceOwnerVpnConfiguration
description: Создайте новый объект androidDeviceOwnerVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f407851267cd28928b4c7380e2aa97088102e170
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130527"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="f48c8-103">Создание androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f48c8-103">Create androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="f48c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f48c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f48c8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f48c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f48c8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f48c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f48c8-107">Создайте [новый объект androidDeviceOwnerVpnConfiguration.](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-107">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f48c8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f48c8-108">Prerequisites</span></span>
<span data-ttu-id="f48c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f48c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f48c8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f48c8-111">Permission type</span></span>|<span data-ttu-id="f48c8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f48c8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f48c8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f48c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f48c8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48c8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f48c8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f48c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f48c8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f48c8-116">Not supported.</span></span>|
|<span data-ttu-id="f48c8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f48c8-117">Application</span></span>|<span data-ttu-id="f48c8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48c8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f48c8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f48c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f48c8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f48c8-120">Request headers</span></span>
|<span data-ttu-id="f48c8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f48c8-121">Header</span></span>|<span data-ttu-id="f48c8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f48c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f48c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f48c8-123">Authorization</span></span>|<span data-ttu-id="f48c8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f48c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f48c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f48c8-125">Accept</span></span>|<span data-ttu-id="f48c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f48c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f48c8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f48c8-127">Request body</span></span>
<span data-ttu-id="f48c8-128">В теле запроса предоставляем представление JSON для объекта androidDeviceOwnerVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f48c8-128">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="f48c8-129">В следующей таблице показаны свойства, необходимые при создании androidDeviceOwnerVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f48c8-129">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="f48c8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f48c8-130">Property</span></span>|<span data-ttu-id="f48c8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f48c8-131">Type</span></span>|<span data-ttu-id="f48c8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f48c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f48c8-133">id</span><span class="sxs-lookup"><span data-stu-id="f48c8-133">id</span></span>|<span data-ttu-id="f48c8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-134">String</span></span>|<span data-ttu-id="f48c8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f48c8-135">Key of the entity.</span></span> <span data-ttu-id="f48c8-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f48c8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f48c8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f48c8-138">DateTimeOffset</span></span>|<span data-ttu-id="f48c8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f48c8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f48c8-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f48c8-141">roleScopeTagIds</span></span>|<span data-ttu-id="f48c8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f48c8-142">String collection</span></span>|<span data-ttu-id="f48c8-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="f48c8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f48c8-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f48c8-145">supportsScopeTags</span></span>|<span data-ttu-id="f48c8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f48c8-146">Boolean</span></span>|<span data-ttu-id="f48c8-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f48c8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f48c8-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="f48c8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f48c8-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f48c8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f48c8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f48c8-150">This property is read-only.</span></span> <span data-ttu-id="f48c8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f48c8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f48c8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f48c8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f48c8-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f48c8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f48c8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f48c8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f48c8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f48c8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f48c8-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f48c8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f48c8-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f48c8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f48c8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f48c8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f48c8-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f48c8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f48c8-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f48c8-164">createdDateTime</span></span>|<span data-ttu-id="f48c8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f48c8-165">DateTimeOffset</span></span>|<span data-ttu-id="f48c8-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f48c8-166">DateTime the object was created.</span></span> <span data-ttu-id="f48c8-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-168">description</span><span class="sxs-lookup"><span data-stu-id="f48c8-168">description</span></span>|<span data-ttu-id="f48c8-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-169">String</span></span>|<span data-ttu-id="f48c8-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f48c8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f48c8-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f48c8-172">displayName</span></span>|<span data-ttu-id="f48c8-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-173">String</span></span>|<span data-ttu-id="f48c8-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f48c8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f48c8-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-176">version</span><span class="sxs-lookup"><span data-stu-id="f48c8-176">version</span></span>|<span data-ttu-id="f48c8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f48c8-177">Int32</span></span>|<span data-ttu-id="f48c8-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f48c8-178">Version of the device configuration.</span></span> <span data-ttu-id="f48c8-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f48c8-180">authenticationMethod</span></span>|[<span data-ttu-id="f48c8-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f48c8-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f48c8-182">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f48c8-182">Authentication method.</span></span> <span data-ttu-id="f48c8-183">Унаследовано от [VPNConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f48c8-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="f48c8-184">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="f48c8-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="f48c8-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="f48c8-185">connectionName</span></span>|<span data-ttu-id="f48c8-186">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-186">String</span></span>|<span data-ttu-id="f48c8-187">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="f48c8-187">Connection name displayed to the user.</span></span> <span data-ttu-id="f48c8-188">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-189">role</span><span class="sxs-lookup"><span data-stu-id="f48c8-189">role</span></span>|<span data-ttu-id="f48c8-190">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-190">String</span></span>|<span data-ttu-id="f48c8-191">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="f48c8-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f48c8-192">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-193">realm</span><span class="sxs-lookup"><span data-stu-id="f48c8-193">realm</span></span>|<span data-ttu-id="f48c8-194">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-194">String</span></span>|<span data-ttu-id="f48c8-195">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="f48c8-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f48c8-196">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-197">серверы</span><span class="sxs-lookup"><span data-stu-id="f48c8-197">servers</span></span>|<span data-ttu-id="f48c8-198">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f48c8-199">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="f48c8-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="f48c8-200">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="f48c8-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f48c8-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f48c8-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f48c8-202">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f48c8-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="f48c8-203">connectionType</span></span>|[<span data-ttu-id="f48c8-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f48c8-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="f48c8-205">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f48c8-205">Connection type.</span></span> <span data-ttu-id="f48c8-206">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span><span class="sxs-lookup"><span data-stu-id="f48c8-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="f48c8-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f48c8-207">proxyServer</span></span>|[<span data-ttu-id="f48c8-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f48c8-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f48c8-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f48c8-209">Proxy server.</span></span>|
|<span data-ttu-id="f48c8-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="f48c8-210">targetedPackageIds</span></span>|<span data-ttu-id="f48c8-211">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f48c8-211">String collection</span></span>|<span data-ttu-id="f48c8-212">Целевые ID-адресов пакета приложений.</span><span class="sxs-lookup"><span data-stu-id="f48c8-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="f48c8-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f48c8-213">targetedMobileApps</span></span>|<span data-ttu-id="f48c8-214">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f48c8-215">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="f48c8-215">Targeted mobile apps.</span></span> <span data-ttu-id="f48c8-216">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f48c8-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f48c8-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="f48c8-217">alwaysOn</span></span>|<span data-ttu-id="f48c8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f48c8-218">Boolean</span></span>|<span data-ttu-id="f48c8-219">Включить или не включить всегда на VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f48c8-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="f48c8-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="f48c8-220">alwaysOnLockdown</span></span>|<span data-ttu-id="f48c8-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="f48c8-221">Boolean</span></span>|<span data-ttu-id="f48c8-222">Если включено всегда подключение к VPN, следует ли заблокировать сетевой трафик при отключении ЭТОГО VPN.</span><span class="sxs-lookup"><span data-stu-id="f48c8-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="f48c8-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="f48c8-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="f48c8-224">Строка</span><span class="sxs-lookup"><span data-stu-id="f48c8-224">String</span></span>|<span data-ttu-id="f48c8-225">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="f48c8-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="f48c8-226">customData</span><span class="sxs-lookup"><span data-stu-id="f48c8-226">customData</span></span>|<span data-ttu-id="f48c8-227">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f48c8-228">Настраиваемые данные для определения пар ключей и значений, определенных поставщику VPN.</span><span class="sxs-lookup"><span data-stu-id="f48c8-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="f48c8-229">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f48c8-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="f48c8-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f48c8-230">customKeyValueData</span></span>|<span data-ttu-id="f48c8-231">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f48c8-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f48c8-232">Настраиваемые данные для определения пар ключей и значений, определенных поставщику VPN.</span><span class="sxs-lookup"><span data-stu-id="f48c8-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="f48c8-233">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f48c8-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f48c8-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="f48c8-234">Response</span></span>
<span data-ttu-id="f48c8-235">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f48c8-235">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f48c8-236">Пример</span><span class="sxs-lookup"><span data-stu-id="f48c8-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="f48c8-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="f48c8-237">Request</span></span>
<span data-ttu-id="f48c8-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f48c8-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2383

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "connectionType": "pulseSecure",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "targetedPackageIds": [
    "Targeted Package Ids value"
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
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="f48c8-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="f48c8-239">Response</span></span>
<span data-ttu-id="f48c8-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f48c8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2555

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
  "id": "972962e3-62e3-9729-e362-2997e3622997",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "connectionType": "pulseSecure",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "targetedPackageIds": [
    "Targeted Package Ids value"
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
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  ]
}
```




