---
title: Обновление Андроиддевицеовнервпнконфигуратион
description: Обновление свойств объекта Андроиддевицеовнервпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7d7fbcaf9fc2fac5f08493ed709f2ebb1ffa451
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954134"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="872e3-103">Обновление Андроиддевицеовнервпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="872e3-103">Update androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="872e3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="872e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="872e3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="872e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="872e3-106">Обновление свойств объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="872e3-106">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="872e3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="872e3-107">Prerequisites</span></span>
<span data-ttu-id="872e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="872e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="872e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="872e3-110">Permission type</span></span>|<span data-ttu-id="872e3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="872e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="872e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="872e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="872e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="872e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="872e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="872e3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="872e3-115">Not supported.</span></span>|
|<span data-ttu-id="872e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="872e3-116">Application</span></span>|<span data-ttu-id="872e3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872e3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="872e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="872e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="872e3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="872e3-119">Request headers</span></span>
|<span data-ttu-id="872e3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="872e3-120">Header</span></span>|<span data-ttu-id="872e3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="872e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="872e3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="872e3-122">Authorization</span></span>|<span data-ttu-id="872e3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="872e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="872e3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="872e3-124">Accept</span></span>|<span data-ttu-id="872e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="872e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="872e3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="872e3-126">Request body</span></span>
<span data-ttu-id="872e3-127">В тексте запроса добавьте представление объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="872e3-127">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="872e3-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-128">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="872e3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="872e3-129">Property</span></span>|<span data-ttu-id="872e3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="872e3-130">Type</span></span>|<span data-ttu-id="872e3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="872e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="872e3-132">id</span><span class="sxs-lookup"><span data-stu-id="872e3-132">id</span></span>|<span data-ttu-id="872e3-133">String</span><span class="sxs-lookup"><span data-stu-id="872e3-133">String</span></span>|<span data-ttu-id="872e3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="872e3-134">Key of the entity.</span></span> <span data-ttu-id="872e3-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="872e3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="872e3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="872e3-137">DateTimeOffset</span></span>|<span data-ttu-id="872e3-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="872e3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="872e3-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="872e3-140">roleScopeTagIds</span></span>|<span data-ttu-id="872e3-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="872e3-141">String collection</span></span>|<span data-ttu-id="872e3-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="872e3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="872e3-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="872e3-144">supportsScopeTags</span></span>|<span data-ttu-id="872e3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="872e3-145">Boolean</span></span>|<span data-ttu-id="872e3-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="872e3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="872e3-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="872e3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="872e3-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="872e3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="872e3-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="872e3-149">This property is read-only.</span></span> <span data-ttu-id="872e3-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="872e3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="872e3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="872e3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="872e3-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="872e3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="872e3-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="872e3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="872e3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="872e3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="872e3-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="872e3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="872e3-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="872e3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="872e3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="872e3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="872e3-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="872e3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="872e3-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="872e3-163">createdDateTime</span></span>|<span data-ttu-id="872e3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="872e3-164">DateTimeOffset</span></span>|<span data-ttu-id="872e3-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="872e3-165">DateTime the object was created.</span></span> <span data-ttu-id="872e3-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-167">description</span><span class="sxs-lookup"><span data-stu-id="872e3-167">description</span></span>|<span data-ttu-id="872e3-168">String</span><span class="sxs-lookup"><span data-stu-id="872e3-168">String</span></span>|<span data-ttu-id="872e3-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="872e3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="872e3-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="872e3-171">displayName</span></span>|<span data-ttu-id="872e3-172">Строка</span><span class="sxs-lookup"><span data-stu-id="872e3-172">String</span></span>|<span data-ttu-id="872e3-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="872e3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="872e3-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-175">version</span><span class="sxs-lookup"><span data-stu-id="872e3-175">version</span></span>|<span data-ttu-id="872e3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="872e3-176">Int32</span></span>|<span data-ttu-id="872e3-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="872e3-177">Version of the device configuration.</span></span> <span data-ttu-id="872e3-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="872e3-179">authenticationMethod</span></span>|[<span data-ttu-id="872e3-180">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="872e3-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="872e3-181">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="872e3-181">Authentication method.</span></span> <span data-ttu-id="872e3-182">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="872e3-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="872e3-183">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="872e3-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="872e3-184">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="872e3-184">connectionName</span></span>|<span data-ttu-id="872e3-185">Строка</span><span class="sxs-lookup"><span data-stu-id="872e3-185">String</span></span>|<span data-ttu-id="872e3-186">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="872e3-186">Connection name displayed to the user.</span></span> <span data-ttu-id="872e3-187">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="872e3-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-188">role</span><span class="sxs-lookup"><span data-stu-id="872e3-188">role</span></span>|<span data-ttu-id="872e3-189">Строка</span><span class="sxs-lookup"><span data-stu-id="872e3-189">String</span></span>|<span data-ttu-id="872e3-190">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="872e3-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="872e3-191">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="872e3-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-192">область</span><span class="sxs-lookup"><span data-stu-id="872e3-192">realm</span></span>|<span data-ttu-id="872e3-193">Строка</span><span class="sxs-lookup"><span data-stu-id="872e3-193">String</span></span>|<span data-ttu-id="872e3-194">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="872e3-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="872e3-195">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="872e3-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-196">серверами</span><span class="sxs-lookup"><span data-stu-id="872e3-196">servers</span></span>|<span data-ttu-id="872e3-197">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="872e3-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="872e3-198">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="872e3-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="872e3-199">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="872e3-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="872e3-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="872e3-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="872e3-201">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="872e3-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="872e3-202">connectionType</span><span class="sxs-lookup"><span data-stu-id="872e3-202">connectionType</span></span>|[<span data-ttu-id="872e3-203">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="872e3-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="872e3-204">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="872e3-204">Connection type.</span></span> <span data-ttu-id="872e3-205">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="872e3-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="872e3-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="872e3-206">Response</span></span>
<span data-ttu-id="872e3-207">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="872e3-207">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="872e3-208">Пример</span><span class="sxs-lookup"><span data-stu-id="872e3-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="872e3-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="872e3-209">Request</span></span>
<span data-ttu-id="872e3-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="872e3-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1417

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
  "connectionType": "pulseSecure"
}
```

### <a name="response"></a><span data-ttu-id="872e3-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="872e3-211">Response</span></span>
<span data-ttu-id="872e3-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="872e3-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1589

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
  "connectionType": "pulseSecure"
}
```





