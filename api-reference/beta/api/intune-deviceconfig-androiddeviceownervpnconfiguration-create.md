---
title: Создание Андроиддевицеовнервпнконфигуратион
description: Создание нового объекта Андроиддевицеовнервпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6730061b9136129b76ec3a8f08bac2d33a7fc3cb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954876"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="3e30d-103">Создание Андроиддевицеовнервпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3e30d-103">Create androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="3e30d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e30d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e30d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e30d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e30d-106">Создание нового объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3e30d-106">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e30d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e30d-107">Prerequisites</span></span>
<span data-ttu-id="3e30d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e30d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e30d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e30d-110">Permission type</span></span>|<span data-ttu-id="3e30d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e30d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e30d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e30d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e30d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e30d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e30d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e30d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e30d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e30d-115">Not supported.</span></span>|
|<span data-ttu-id="3e30d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e30d-116">Application</span></span>|<span data-ttu-id="3e30d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e30d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e30d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e30d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e30d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e30d-119">Request headers</span></span>
|<span data-ttu-id="3e30d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e30d-120">Header</span></span>|<span data-ttu-id="3e30d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e30d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e30d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e30d-122">Authorization</span></span>|<span data-ttu-id="3e30d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e30d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e30d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e30d-124">Accept</span></span>|<span data-ttu-id="3e30d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e30d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e30d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e30d-126">Request body</span></span>
<span data-ttu-id="3e30d-127">В тексте запроса добавьте представление объекта Андроиддевицеовнервпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e30d-127">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="3e30d-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнервпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="3e30d-128">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="3e30d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e30d-129">Property</span></span>|<span data-ttu-id="3e30d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e30d-130">Type</span></span>|<span data-ttu-id="3e30d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e30d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e30d-132">id</span><span class="sxs-lookup"><span data-stu-id="3e30d-132">id</span></span>|<span data-ttu-id="3e30d-133">String</span><span class="sxs-lookup"><span data-stu-id="3e30d-133">String</span></span>|<span data-ttu-id="3e30d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e30d-134">Key of the entity.</span></span> <span data-ttu-id="3e30d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e30d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3e30d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e30d-137">DateTimeOffset</span></span>|<span data-ttu-id="3e30d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e30d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3e30d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e30d-140">roleScopeTagIds</span></span>|<span data-ttu-id="3e30d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e30d-141">String collection</span></span>|<span data-ttu-id="3e30d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3e30d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3e30d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3e30d-144">supportsScopeTags</span></span>|<span data-ttu-id="3e30d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e30d-145">Boolean</span></span>|<span data-ttu-id="3e30d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3e30d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3e30d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3e30d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3e30d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3e30d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3e30d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e30d-149">This property is read-only.</span></span> <span data-ttu-id="3e30d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3e30d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3e30d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3e30d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3e30d-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3e30d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3e30d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3e30d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3e30d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3e30d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3e30d-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3e30d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3e30d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3e30d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3e30d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3e30d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3e30d-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3e30d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3e30d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e30d-163">createdDateTime</span></span>|<span data-ttu-id="3e30d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e30d-164">DateTimeOffset</span></span>|<span data-ttu-id="3e30d-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3e30d-165">DateTime the object was created.</span></span> <span data-ttu-id="3e30d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-167">description</span><span class="sxs-lookup"><span data-stu-id="3e30d-167">description</span></span>|<span data-ttu-id="3e30d-168">String</span><span class="sxs-lookup"><span data-stu-id="3e30d-168">String</span></span>|<span data-ttu-id="3e30d-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e30d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e30d-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="3e30d-171">displayName</span></span>|<span data-ttu-id="3e30d-172">Строка</span><span class="sxs-lookup"><span data-stu-id="3e30d-172">String</span></span>|<span data-ttu-id="3e30d-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e30d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e30d-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-175">version</span><span class="sxs-lookup"><span data-stu-id="3e30d-175">version</span></span>|<span data-ttu-id="3e30d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3e30d-176">Int32</span></span>|<span data-ttu-id="3e30d-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e30d-177">Version of the device configuration.</span></span> <span data-ttu-id="3e30d-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="3e30d-179">authenticationMethod</span></span>|[<span data-ttu-id="3e30d-180">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="3e30d-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3e30d-181">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3e30d-181">Authentication method.</span></span> <span data-ttu-id="3e30d-182">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e30d-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="3e30d-183">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="3e30d-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="3e30d-184">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="3e30d-184">connectionName</span></span>|<span data-ttu-id="3e30d-185">Строка</span><span class="sxs-lookup"><span data-stu-id="3e30d-185">String</span></span>|<span data-ttu-id="3e30d-186">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e30d-186">Connection name displayed to the user.</span></span> <span data-ttu-id="3e30d-187">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e30d-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-188">role</span><span class="sxs-lookup"><span data-stu-id="3e30d-188">role</span></span>|<span data-ttu-id="3e30d-189">Строка</span><span class="sxs-lookup"><span data-stu-id="3e30d-189">String</span></span>|<span data-ttu-id="3e30d-190">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="3e30d-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3e30d-191">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e30d-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-192">область</span><span class="sxs-lookup"><span data-stu-id="3e30d-192">realm</span></span>|<span data-ttu-id="3e30d-193">Строка</span><span class="sxs-lookup"><span data-stu-id="3e30d-193">String</span></span>|<span data-ttu-id="3e30d-194">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="3e30d-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3e30d-195">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e30d-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-196">серверами</span><span class="sxs-lookup"><span data-stu-id="3e30d-196">servers</span></span>|<span data-ttu-id="3e30d-197">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="3e30d-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3e30d-198">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="3e30d-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="3e30d-199">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="3e30d-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3e30d-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e30d-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3e30d-201">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e30d-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3e30d-202">connectionType</span><span class="sxs-lookup"><span data-stu-id="3e30d-202">connectionType</span></span>|[<span data-ttu-id="3e30d-203">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="3e30d-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="3e30d-204">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="3e30d-204">Connection type.</span></span> <span data-ttu-id="3e30d-205">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="3e30d-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="3e30d-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e30d-206">Response</span></span>
<span data-ttu-id="3e30d-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e30d-207">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e30d-208">Пример</span><span class="sxs-lookup"><span data-stu-id="3e30d-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e30d-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e30d-209">Request</span></span>
<span data-ttu-id="3e30d-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e30d-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3e30d-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e30d-211">Response</span></span>
<span data-ttu-id="3e30d-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e30d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





