---
title: Обновление androidDeviceOwnerVpnConfiguration
description: Обновление свойств объекта androidDeviceOwnerVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e68d95eb8e6eeabf5a3c2a5e559c1ecdb1e88d03
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156135"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="d3d32-103">Обновление androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3d32-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="d3d32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3d32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3d32-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3d32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3d32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3d32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3d32-107">Обновление свойств объекта [androidDeviceOwnerVpnConfiguration.](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3d32-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3d32-108">Prerequisites</span></span>
<span data-ttu-id="d3d32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3d32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3d32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3d32-111">Permission type</span></span>|<span data-ttu-id="d3d32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3d32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3d32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3d32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3d32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3d32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3d32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3d32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3d32-116">Not supported.</span></span>|
|<span data-ttu-id="d3d32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3d32-117">Application</span></span>|<span data-ttu-id="d3d32-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d32-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3d32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3d32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d3d32-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3d32-120">Request headers</span></span>
|<span data-ttu-id="d3d32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3d32-121">Header</span></span>|<span data-ttu-id="d3d32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3d32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3d32-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3d32-123">Authorization</span></span>|<span data-ttu-id="d3d32-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3d32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3d32-125">Accept</span></span>|<span data-ttu-id="d3d32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3d32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3d32-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3d32-127">Request body</span></span>
<span data-ttu-id="d3d32-128">В теле запроса предоставляем представление объекта [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="d3d32-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="d3d32-129">В следующей таблице показаны свойства, необходимые при создании [объекта androidDeviceOwnerVpnConfiguration.](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="d3d32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3d32-130">Property</span></span>|<span data-ttu-id="d3d32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d32-131">Type</span></span>|<span data-ttu-id="d3d32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d32-133">id</span><span class="sxs-lookup"><span data-stu-id="d3d32-133">id</span></span>|<span data-ttu-id="d3d32-134">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-134">String</span></span>|<span data-ttu-id="d3d32-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d3d32-135">Key of the entity.</span></span> <span data-ttu-id="d3d32-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3d32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d3d32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d32-138">DateTimeOffset</span></span>|<span data-ttu-id="d3d32-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d3d32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d3d32-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3d32-141">roleScopeTagIds</span></span>|<span data-ttu-id="d3d32-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d3d32-142">String collection</span></span>|<span data-ttu-id="d3d32-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d3d32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d3d32-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d3d32-145">supportsScopeTags</span></span>|<span data-ttu-id="d3d32-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3d32-146">Boolean</span></span>|<span data-ttu-id="d3d32-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d3d32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d3d32-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d3d32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d3d32-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d3d32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d3d32-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3d32-150">This property is read-only.</span></span> <span data-ttu-id="d3d32-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d3d32-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d3d32-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d3d32-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d3d32-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d3d32-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d3d32-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d3d32-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d3d32-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d3d32-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d3d32-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d3d32-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d3d32-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d3d32-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d3d32-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d3d32-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d3d32-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d3d32-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d3d32-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3d32-164">createdDateTime</span></span>|<span data-ttu-id="d3d32-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d32-165">DateTimeOffset</span></span>|<span data-ttu-id="d3d32-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d3d32-166">DateTime the object was created.</span></span> <span data-ttu-id="d3d32-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-168">description</span><span class="sxs-lookup"><span data-stu-id="d3d32-168">description</span></span>|<span data-ttu-id="d3d32-169">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-169">String</span></span>|<span data-ttu-id="d3d32-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3d32-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d3d32-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d3d32-172">displayName</span></span>|<span data-ttu-id="d3d32-173">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-173">String</span></span>|<span data-ttu-id="d3d32-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3d32-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d3d32-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-176">version</span><span class="sxs-lookup"><span data-stu-id="d3d32-176">version</span></span>|<span data-ttu-id="d3d32-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d3d32-177">Int32</span></span>|<span data-ttu-id="d3d32-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3d32-178">Version of the device configuration.</span></span> <span data-ttu-id="d3d32-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3d32-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d3d32-180">authenticationMethod</span></span>|[<span data-ttu-id="d3d32-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d3d32-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d3d32-182">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d3d32-182">Authentication method.</span></span> <span data-ttu-id="d3d32-183">Наследуется от [vpnConfiguration.](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="d3d32-184">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="d3d32-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="d3d32-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="d3d32-185">connectionName</span></span>|<span data-ttu-id="d3d32-186">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-186">String</span></span>|<span data-ttu-id="d3d32-187">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3d32-187">Connection name displayed to the user.</span></span> <span data-ttu-id="d3d32-188">Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-189">role</span><span class="sxs-lookup"><span data-stu-id="d3d32-189">role</span></span>|<span data-ttu-id="d3d32-190">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-190">String</span></span>|<span data-ttu-id="d3d32-191">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="d3d32-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d3d32-192">Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-193">realm</span><span class="sxs-lookup"><span data-stu-id="d3d32-193">realm</span></span>|<span data-ttu-id="d3d32-194">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-194">String</span></span>|<span data-ttu-id="d3d32-195">Область, когда для типа подключения установлено безопасное пульса.</span><span class="sxs-lookup"><span data-stu-id="d3d32-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d3d32-196">Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-197">серверы</span><span class="sxs-lookup"><span data-stu-id="d3d32-197">servers</span></span>|<span data-ttu-id="d3d32-198">[Коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d3d32-199">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="d3d32-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="d3d32-200">Убедитесь, что конечные пользователи имеют доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="d3d32-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d3d32-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d3d32-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d3d32-202">Наследуется от [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d3d32-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="d3d32-203">connectionType</span></span>|[<span data-ttu-id="d3d32-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d3d32-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="d3d32-205">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="d3d32-205">Connection type.</span></span> <span data-ttu-id="d3d32-206">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span><span class="sxs-lookup"><span data-stu-id="d3d32-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="d3d32-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d3d32-207">proxyServer</span></span>|[<span data-ttu-id="d3d32-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d3d32-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="d3d32-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="d3d32-209">Proxy server.</span></span>|
|<span data-ttu-id="d3d32-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="d3d32-210">targetedPackageIds</span></span>|<span data-ttu-id="d3d32-211">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d3d32-211">String collection</span></span>|<span data-ttu-id="d3d32-212">ИД пакета целевого приложения.</span><span class="sxs-lookup"><span data-stu-id="d3d32-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="d3d32-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d3d32-213">targetedMobileApps</span></span>|<span data-ttu-id="d3d32-214">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d3d32-215">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="d3d32-215">Targeted mobile apps.</span></span> <span data-ttu-id="d3d32-216">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d3d32-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d3d32-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="d3d32-217">alwaysOn</span></span>|<span data-ttu-id="d3d32-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3d32-218">Boolean</span></span>|<span data-ttu-id="d3d32-219">Следует ли включить постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="d3d32-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="d3d32-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="d3d32-220">alwaysOnLockdown</span></span>|<span data-ttu-id="d3d32-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3d32-221">Boolean</span></span>|<span data-ttu-id="d3d32-222">Если включено постоянное VPN-подключение, следует ли заблокировать сетевой трафик при отключении vpn.</span><span class="sxs-lookup"><span data-stu-id="d3d32-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="d3d32-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="d3d32-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="d3d32-224">String</span><span class="sxs-lookup"><span data-stu-id="d3d32-224">String</span></span>|<span data-ttu-id="d3d32-225">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="d3d32-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="d3d32-226">customData</span><span class="sxs-lookup"><span data-stu-id="d3d32-226">customData</span></span>|<span data-ttu-id="d3d32-227">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="d3d32-228">Пользовательские данные для определения пар "ключ-значение", характерных для поставщика VPN.</span><span class="sxs-lookup"><span data-stu-id="d3d32-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="d3d32-229">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="d3d32-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="d3d32-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="d3d32-230">customKeyValueData</span></span>|<span data-ttu-id="d3d32-231">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d3d32-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d3d32-232">Пользовательские данные для определения пар "ключ-значение", характерных для поставщика VPN.</span><span class="sxs-lookup"><span data-stu-id="d3d32-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="d3d32-233">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="d3d32-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d3d32-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d32-234">Response</span></span>
<span data-ttu-id="d3d32-235">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3d32-235">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3d32-236">Пример</span><span class="sxs-lookup"><span data-stu-id="d3d32-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3d32-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3d32-237">Request</span></span>
<span data-ttu-id="d3d32-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3d32-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3d32-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d32-239">Response</span></span>
<span data-ttu-id="d3d32-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3d32-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




