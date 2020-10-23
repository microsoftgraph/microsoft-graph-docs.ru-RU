---
title: Обновление Андроиддевицеовнервпнконфигуратион
description: Обновление свойств объекта Андроиддевицеовнервпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c76e937bc30a3d6d3c49829eca582c5a200d30a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726985"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="96657-103">Обновление Андроиддевицеовнервпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="96657-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="96657-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96657-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96657-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96657-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96657-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96657-107">Обновление свойств объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="96657-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96657-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96657-108">Prerequisites</span></span>
<span data-ttu-id="96657-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96657-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96657-111">Permission type</span></span>|<span data-ttu-id="96657-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96657-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96657-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96657-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96657-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96657-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96657-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96657-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96657-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96657-116">Not supported.</span></span>|
|<span data-ttu-id="96657-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96657-117">Application</span></span>|<span data-ttu-id="96657-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96657-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96657-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96657-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="96657-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96657-120">Request headers</span></span>
|<span data-ttu-id="96657-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96657-121">Header</span></span>|<span data-ttu-id="96657-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96657-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96657-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96657-123">Authorization</span></span>|<span data-ttu-id="96657-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96657-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96657-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96657-125">Accept</span></span>|<span data-ttu-id="96657-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96657-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96657-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96657-127">Request body</span></span>
<span data-ttu-id="96657-128">В тексте запроса добавьте представление объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96657-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="96657-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="96657-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="96657-130">Property</span></span>|<span data-ttu-id="96657-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96657-131">Type</span></span>|<span data-ttu-id="96657-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96657-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96657-133">id</span><span class="sxs-lookup"><span data-stu-id="96657-133">id</span></span>|<span data-ttu-id="96657-134">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-134">String</span></span>|<span data-ttu-id="96657-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96657-135">Key of the entity.</span></span> <span data-ttu-id="96657-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96657-137">lastModifiedDateTime</span></span>|<span data-ttu-id="96657-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96657-138">DateTimeOffset</span></span>|<span data-ttu-id="96657-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="96657-139">DateTime the object was last modified.</span></span> <span data-ttu-id="96657-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96657-141">roleScopeTagIds</span></span>|<span data-ttu-id="96657-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96657-142">String collection</span></span>|<span data-ttu-id="96657-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="96657-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96657-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="96657-145">supportsScopeTags</span></span>|<span data-ttu-id="96657-146">Логический</span><span class="sxs-lookup"><span data-stu-id="96657-146">Boolean</span></span>|<span data-ttu-id="96657-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="96657-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="96657-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="96657-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="96657-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="96657-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="96657-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96657-150">This property is read-only.</span></span> <span data-ttu-id="96657-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="96657-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="96657-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="96657-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="96657-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96657-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="96657-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="96657-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="96657-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="96657-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="96657-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96657-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="96657-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="96657-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="96657-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="96657-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="96657-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96657-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="96657-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96657-164">createdDateTime</span></span>|<span data-ttu-id="96657-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96657-165">DateTimeOffset</span></span>|<span data-ttu-id="96657-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="96657-166">DateTime the object was created.</span></span> <span data-ttu-id="96657-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-168">description</span><span class="sxs-lookup"><span data-stu-id="96657-168">description</span></span>|<span data-ttu-id="96657-169">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-169">String</span></span>|<span data-ttu-id="96657-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96657-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96657-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-172">displayName</span><span class="sxs-lookup"><span data-stu-id="96657-172">displayName</span></span>|<span data-ttu-id="96657-173">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-173">String</span></span>|<span data-ttu-id="96657-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96657-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96657-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-176">version</span><span class="sxs-lookup"><span data-stu-id="96657-176">version</span></span>|<span data-ttu-id="96657-177">Int32</span><span class="sxs-lookup"><span data-stu-id="96657-177">Int32</span></span>|<span data-ttu-id="96657-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96657-178">Version of the device configuration.</span></span> <span data-ttu-id="96657-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96657-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="96657-180">authenticationMethod</span></span>|[<span data-ttu-id="96657-181">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="96657-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="96657-182">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="96657-182">Authentication method.</span></span> <span data-ttu-id="96657-183">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96657-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="96657-184">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="96657-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="96657-185">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="96657-185">connectionName</span></span>|<span data-ttu-id="96657-186">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-186">String</span></span>|<span data-ttu-id="96657-187">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="96657-187">Connection name displayed to the user.</span></span> <span data-ttu-id="96657-188">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96657-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="96657-189">role</span><span class="sxs-lookup"><span data-stu-id="96657-189">role</span></span>|<span data-ttu-id="96657-190">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-190">String</span></span>|<span data-ttu-id="96657-191">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="96657-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="96657-192">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96657-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="96657-193">область</span><span class="sxs-lookup"><span data-stu-id="96657-193">realm</span></span>|<span data-ttu-id="96657-194">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-194">String</span></span>|<span data-ttu-id="96657-195">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="96657-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="96657-196">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96657-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="96657-197">серверами</span><span class="sxs-lookup"><span data-stu-id="96657-197">servers</span></span>|<span data-ttu-id="96657-198">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="96657-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="96657-199">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="96657-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="96657-200">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="96657-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="96657-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="96657-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="96657-202">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96657-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="96657-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="96657-203">connectionType</span></span>|[<span data-ttu-id="96657-204">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="96657-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="96657-205">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="96657-205">Connection type.</span></span> <span data-ttu-id="96657-206">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span><span class="sxs-lookup"><span data-stu-id="96657-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="96657-207">проксисервер</span><span class="sxs-lookup"><span data-stu-id="96657-207">proxyServer</span></span>|[<span data-ttu-id="96657-208">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="96657-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="96657-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="96657-209">Proxy server.</span></span>|
|<span data-ttu-id="96657-210">таржетедпаккажеидс</span><span class="sxs-lookup"><span data-stu-id="96657-210">targetedPackageIds</span></span>|<span data-ttu-id="96657-211">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96657-211">String collection</span></span>|<span data-ttu-id="96657-212">Идентификаторы целевых пакетов приложений.</span><span class="sxs-lookup"><span data-stu-id="96657-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="96657-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="96657-213">targetedMobileApps</span></span>|<span data-ttu-id="96657-214">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="96657-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="96657-215">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="96657-215">Targeted mobile apps.</span></span> <span data-ttu-id="96657-216">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="96657-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="96657-217">Группа</span><span class="sxs-lookup"><span data-stu-id="96657-217">alwaysOn</span></span>|<span data-ttu-id="96657-218">Логический</span><span class="sxs-lookup"><span data-stu-id="96657-218">Boolean</span></span>|<span data-ttu-id="96657-219">Указывает, следует ли включить постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="96657-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="96657-220">алвайсонлоккдовн</span><span class="sxs-lookup"><span data-stu-id="96657-220">alwaysOnLockdown</span></span>|<span data-ttu-id="96657-221">Логический</span><span class="sxs-lookup"><span data-stu-id="96657-221">Boolean</span></span>|<span data-ttu-id="96657-222">Если включено постоянное VPN-подключение, независимо от того, следует ли блокировать сетевой трафик при отключении VPN.</span><span class="sxs-lookup"><span data-stu-id="96657-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="96657-223">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="96657-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="96657-224">Строка</span><span class="sxs-lookup"><span data-stu-id="96657-224">String</span></span>|<span data-ttu-id="96657-225">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="96657-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="96657-226">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="96657-226">customData</span></span>|<span data-ttu-id="96657-227">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="96657-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="96657-228">Пользовательские данные, определяющие пары "ключ-значение", характерные для поставщика услуг VPN.</span><span class="sxs-lookup"><span data-stu-id="96657-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="96657-229">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="96657-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="96657-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="96657-230">customKeyValueData</span></span>|<span data-ttu-id="96657-231">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="96657-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="96657-232">Пользовательские данные, определяющие пары "ключ-значение", характерные для поставщика услуг VPN.</span><span class="sxs-lookup"><span data-stu-id="96657-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="96657-233">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="96657-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="96657-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="96657-234">Response</span></span>
<span data-ttu-id="96657-235">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96657-235">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96657-236">Пример</span><span class="sxs-lookup"><span data-stu-id="96657-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="96657-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="96657-237">Request</span></span>
<span data-ttu-id="96657-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96657-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96657-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="96657-239">Response</span></span>
<span data-ttu-id="96657-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96657-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





