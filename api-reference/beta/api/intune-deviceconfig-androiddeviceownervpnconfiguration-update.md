---
title: Обновление androidDeviceOwnerVpnConfiguration
description: Обновление свойств объекта androidDeviceOwnerVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3185d467a4d28cf7f24e15fda11ddaf320a4934
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138500"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="b1c56-103">Обновление androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1c56-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="b1c56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1c56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1c56-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1c56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1c56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1c56-107">Обновление свойств объекта [androidDeviceOwnerVpnConfiguration.](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1c56-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1c56-108">Prerequisites</span></span>
<span data-ttu-id="b1c56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1c56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c56-111">Permission type</span></span>|<span data-ttu-id="b1c56-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1c56-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1c56-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1c56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1c56-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c56-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1c56-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1c56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1c56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c56-116">Not supported.</span></span>|
|<span data-ttu-id="b1c56-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1c56-117">Application</span></span>|<span data-ttu-id="b1c56-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c56-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1c56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1c56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b1c56-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1c56-120">Request headers</span></span>
|<span data-ttu-id="b1c56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1c56-121">Header</span></span>|<span data-ttu-id="b1c56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1c56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1c56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1c56-123">Authorization</span></span>|<span data-ttu-id="b1c56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1c56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1c56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1c56-125">Accept</span></span>|<span data-ttu-id="b1c56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1c56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1c56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1c56-127">Request body</span></span>
<span data-ttu-id="b1c56-128">В теле запроса предоставляем представление JSON для [объекта androidDeviceOwnerVpnConfiguration.](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="b1c56-129">В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerVpnConfiguration.](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="b1c56-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1c56-130">Property</span></span>|<span data-ttu-id="b1c56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1c56-131">Type</span></span>|<span data-ttu-id="b1c56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1c56-133">id</span><span class="sxs-lookup"><span data-stu-id="b1c56-133">id</span></span>|<span data-ttu-id="b1c56-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-134">String</span></span>|<span data-ttu-id="b1c56-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1c56-135">Key of the entity.</span></span> <span data-ttu-id="b1c56-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1c56-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b1c56-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1c56-138">DateTimeOffset</span></span>|<span data-ttu-id="b1c56-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b1c56-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b1c56-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1c56-141">roleScopeTagIds</span></span>|<span data-ttu-id="b1c56-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1c56-142">String collection</span></span>|<span data-ttu-id="b1c56-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="b1c56-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1c56-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b1c56-145">supportsScopeTags</span></span>|<span data-ttu-id="b1c56-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1c56-146">Boolean</span></span>|<span data-ttu-id="b1c56-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b1c56-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b1c56-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="b1c56-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b1c56-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b1c56-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b1c56-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1c56-150">This property is read-only.</span></span> <span data-ttu-id="b1c56-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1c56-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b1c56-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1c56-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b1c56-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b1c56-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b1c56-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1c56-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b1c56-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1c56-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b1c56-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b1c56-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b1c56-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1c56-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b1c56-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1c56-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b1c56-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b1c56-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b1c56-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1c56-164">createdDateTime</span></span>|<span data-ttu-id="b1c56-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1c56-165">DateTimeOffset</span></span>|<span data-ttu-id="b1c56-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b1c56-166">DateTime the object was created.</span></span> <span data-ttu-id="b1c56-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-168">description</span><span class="sxs-lookup"><span data-stu-id="b1c56-168">description</span></span>|<span data-ttu-id="b1c56-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-169">String</span></span>|<span data-ttu-id="b1c56-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1c56-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1c56-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b1c56-172">displayName</span></span>|<span data-ttu-id="b1c56-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-173">String</span></span>|<span data-ttu-id="b1c56-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1c56-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1c56-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-176">version</span><span class="sxs-lookup"><span data-stu-id="b1c56-176">version</span></span>|<span data-ttu-id="b1c56-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b1c56-177">Int32</span></span>|<span data-ttu-id="b1c56-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b1c56-178">Version of the device configuration.</span></span> <span data-ttu-id="b1c56-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b1c56-180">authenticationMethod</span></span>|[<span data-ttu-id="b1c56-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b1c56-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b1c56-182">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b1c56-182">Authentication method.</span></span> <span data-ttu-id="b1c56-183">Унаследовано от [VPNConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c56-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="b1c56-184">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="b1c56-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="b1c56-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="b1c56-185">connectionName</span></span>|<span data-ttu-id="b1c56-186">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-186">String</span></span>|<span data-ttu-id="b1c56-187">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="b1c56-187">Connection name displayed to the user.</span></span> <span data-ttu-id="b1c56-188">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-189">role</span><span class="sxs-lookup"><span data-stu-id="b1c56-189">role</span></span>|<span data-ttu-id="b1c56-190">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-190">String</span></span>|<span data-ttu-id="b1c56-191">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="b1c56-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b1c56-192">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-193">realm</span><span class="sxs-lookup"><span data-stu-id="b1c56-193">realm</span></span>|<span data-ttu-id="b1c56-194">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-194">String</span></span>|<span data-ttu-id="b1c56-195">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="b1c56-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b1c56-196">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-197">серверы</span><span class="sxs-lookup"><span data-stu-id="b1c56-197">servers</span></span>|<span data-ttu-id="b1c56-198">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b1c56-199">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="b1c56-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="b1c56-200">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="b1c56-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b1c56-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b1c56-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b1c56-202">Унаследованный от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b1c56-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="b1c56-203">connectionType</span></span>|[<span data-ttu-id="b1c56-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b1c56-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="b1c56-205">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="b1c56-205">Connection type.</span></span> <span data-ttu-id="b1c56-206">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span><span class="sxs-lookup"><span data-stu-id="b1c56-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="b1c56-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b1c56-207">proxyServer</span></span>|[<span data-ttu-id="b1c56-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b1c56-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b1c56-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="b1c56-209">Proxy server.</span></span>|
|<span data-ttu-id="b1c56-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="b1c56-210">targetedPackageIds</span></span>|<span data-ttu-id="b1c56-211">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1c56-211">String collection</span></span>|<span data-ttu-id="b1c56-212">Целевые ID-адресов пакета приложений.</span><span class="sxs-lookup"><span data-stu-id="b1c56-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="b1c56-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b1c56-213">targetedMobileApps</span></span>|<span data-ttu-id="b1c56-214">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b1c56-215">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="b1c56-215">Targeted mobile apps.</span></span> <span data-ttu-id="b1c56-216">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b1c56-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b1c56-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="b1c56-217">alwaysOn</span></span>|<span data-ttu-id="b1c56-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1c56-218">Boolean</span></span>|<span data-ttu-id="b1c56-219">Включить или не включить всегда на VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="b1c56-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="b1c56-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="b1c56-220">alwaysOnLockdown</span></span>|<span data-ttu-id="b1c56-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1c56-221">Boolean</span></span>|<span data-ttu-id="b1c56-222">Если включено всегда подключение к VPN, следует ли заблокировать сетевой трафик при отключении ЭТОГО VPN.</span><span class="sxs-lookup"><span data-stu-id="b1c56-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="b1c56-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="b1c56-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="b1c56-224">Строка</span><span class="sxs-lookup"><span data-stu-id="b1c56-224">String</span></span>|<span data-ttu-id="b1c56-225">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="b1c56-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="b1c56-226">customData</span><span class="sxs-lookup"><span data-stu-id="b1c56-226">customData</span></span>|<span data-ttu-id="b1c56-227">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b1c56-228">Настраиваемые данные для определения пар ключей и значений, определенных поставщику VPN.</span><span class="sxs-lookup"><span data-stu-id="b1c56-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="b1c56-229">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="b1c56-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b1c56-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b1c56-230">customKeyValueData</span></span>|<span data-ttu-id="b1c56-231">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b1c56-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b1c56-232">Настраиваемые данные для определения пар ключей и значений, определенных поставщику VPN.</span><span class="sxs-lookup"><span data-stu-id="b1c56-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="b1c56-233">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="b1c56-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b1c56-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c56-234">Response</span></span>
<span data-ttu-id="b1c56-235">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1c56-235">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1c56-236">Пример</span><span class="sxs-lookup"><span data-stu-id="b1c56-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1c56-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1c56-237">Request</span></span>
<span data-ttu-id="b1c56-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1c56-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="b1c56-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c56-239">Response</span></span>
<span data-ttu-id="b1c56-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1c56-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




