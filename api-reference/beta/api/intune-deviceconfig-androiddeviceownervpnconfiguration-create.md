---
title: Создание Андроиддевицеовнервпнконфигуратион
description: Создание нового объекта Андроиддевицеовнервпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d60269458221b00472cca1a2ce082d9390a32b62
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123339"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="38deb-103">Создание Андроиддевицеовнервпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="38deb-103">Create androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="38deb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38deb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38deb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38deb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38deb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38deb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38deb-107">Создание нового объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="38deb-107">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38deb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38deb-108">Prerequisites</span></span>
<span data-ttu-id="38deb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="38deb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="38deb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38deb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38deb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38deb-111">Permission type</span></span>|<span data-ttu-id="38deb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38deb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38deb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38deb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38deb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38deb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38deb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38deb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38deb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38deb-116">Not supported.</span></span>|
|<span data-ttu-id="38deb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38deb-117">Application</span></span>|<span data-ttu-id="38deb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38deb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38deb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38deb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38deb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38deb-120">Request headers</span></span>
|<span data-ttu-id="38deb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38deb-121">Header</span></span>|<span data-ttu-id="38deb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="38deb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38deb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38deb-123">Authorization</span></span>|<span data-ttu-id="38deb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38deb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38deb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38deb-125">Accept</span></span>|<span data-ttu-id="38deb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38deb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38deb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38deb-127">Request body</span></span>
<span data-ttu-id="38deb-128">В тексте запроса добавьте представление объекта Андроиддевицеовнервпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38deb-128">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="38deb-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнервпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="38deb-129">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="38deb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="38deb-130">Property</span></span>|<span data-ttu-id="38deb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38deb-131">Type</span></span>|<span data-ttu-id="38deb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38deb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38deb-133">id</span><span class="sxs-lookup"><span data-stu-id="38deb-133">id</span></span>|<span data-ttu-id="38deb-134">String</span><span class="sxs-lookup"><span data-stu-id="38deb-134">String</span></span>|<span data-ttu-id="38deb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38deb-135">Key of the entity.</span></span> <span data-ttu-id="38deb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38deb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="38deb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38deb-138">DateTimeOffset</span></span>|<span data-ttu-id="38deb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="38deb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="38deb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38deb-141">roleScopeTagIds</span></span>|<span data-ttu-id="38deb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="38deb-142">String collection</span></span>|<span data-ttu-id="38deb-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="38deb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38deb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="38deb-145">supportsScopeTags</span></span>|<span data-ttu-id="38deb-146">Логический</span><span class="sxs-lookup"><span data-stu-id="38deb-146">Boolean</span></span>|<span data-ttu-id="38deb-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="38deb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="38deb-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="38deb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="38deb-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="38deb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="38deb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38deb-150">This property is read-only.</span></span> <span data-ttu-id="38deb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="38deb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="38deb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="38deb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="38deb-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="38deb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="38deb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="38deb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="38deb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="38deb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="38deb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="38deb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="38deb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="38deb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="38deb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="38deb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="38deb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="38deb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="38deb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38deb-164">createdDateTime</span></span>|<span data-ttu-id="38deb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38deb-165">DateTimeOffset</span></span>|<span data-ttu-id="38deb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="38deb-166">DateTime the object was created.</span></span> <span data-ttu-id="38deb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-168">description</span><span class="sxs-lookup"><span data-stu-id="38deb-168">description</span></span>|<span data-ttu-id="38deb-169">String</span><span class="sxs-lookup"><span data-stu-id="38deb-169">String</span></span>|<span data-ttu-id="38deb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38deb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38deb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="38deb-172">displayName</span></span>|<span data-ttu-id="38deb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="38deb-173">String</span></span>|<span data-ttu-id="38deb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38deb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38deb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-176">version</span><span class="sxs-lookup"><span data-stu-id="38deb-176">version</span></span>|<span data-ttu-id="38deb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="38deb-177">Int32</span></span>|<span data-ttu-id="38deb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38deb-178">Version of the device configuration.</span></span> <span data-ttu-id="38deb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="38deb-180">authenticationMethod</span></span>|[<span data-ttu-id="38deb-181">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="38deb-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="38deb-182">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="38deb-182">Authentication method.</span></span> <span data-ttu-id="38deb-183">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38deb-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="38deb-184">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="38deb-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="38deb-185">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="38deb-185">connectionName</span></span>|<span data-ttu-id="38deb-186">String</span><span class="sxs-lookup"><span data-stu-id="38deb-186">String</span></span>|<span data-ttu-id="38deb-187">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="38deb-187">Connection name displayed to the user.</span></span> <span data-ttu-id="38deb-188">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38deb-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-189">role</span><span class="sxs-lookup"><span data-stu-id="38deb-189">role</span></span>|<span data-ttu-id="38deb-190">String</span><span class="sxs-lookup"><span data-stu-id="38deb-190">String</span></span>|<span data-ttu-id="38deb-191">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="38deb-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="38deb-192">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38deb-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-193">область</span><span class="sxs-lookup"><span data-stu-id="38deb-193">realm</span></span>|<span data-ttu-id="38deb-194">String</span><span class="sxs-lookup"><span data-stu-id="38deb-194">String</span></span>|<span data-ttu-id="38deb-195">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="38deb-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="38deb-196">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38deb-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-197">серверами</span><span class="sxs-lookup"><span data-stu-id="38deb-197">servers</span></span>|<span data-ttu-id="38deb-198">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="38deb-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="38deb-199">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="38deb-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="38deb-200">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="38deb-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="38deb-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="38deb-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="38deb-202">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38deb-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="38deb-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="38deb-203">connectionType</span></span>|[<span data-ttu-id="38deb-204">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="38deb-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="38deb-205">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="38deb-205">Connection type.</span></span> <span data-ttu-id="38deb-206">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`.</span><span class="sxs-lookup"><span data-stu-id="38deb-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="38deb-207">проксисервер</span><span class="sxs-lookup"><span data-stu-id="38deb-207">proxyServer</span></span>|[<span data-ttu-id="38deb-208">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="38deb-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="38deb-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="38deb-209">Proxy server.</span></span>|
|<span data-ttu-id="38deb-210">таржетедпаккажеидс</span><span class="sxs-lookup"><span data-stu-id="38deb-210">targetedPackageIds</span></span>|<span data-ttu-id="38deb-211">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="38deb-211">String collection</span></span>|<span data-ttu-id="38deb-212">Идентификаторы целевых пакетов приложений.</span><span class="sxs-lookup"><span data-stu-id="38deb-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="38deb-213">Группа</span><span class="sxs-lookup"><span data-stu-id="38deb-213">alwaysOn</span></span>|<span data-ttu-id="38deb-214">Логический</span><span class="sxs-lookup"><span data-stu-id="38deb-214">Boolean</span></span>|<span data-ttu-id="38deb-215">Указывает, следует ли включить постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="38deb-215">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="38deb-216">алвайсонлоккдовн</span><span class="sxs-lookup"><span data-stu-id="38deb-216">alwaysOnLockdown</span></span>|<span data-ttu-id="38deb-217">Логический</span><span class="sxs-lookup"><span data-stu-id="38deb-217">Boolean</span></span>|<span data-ttu-id="38deb-218">Если включено постоянное VPN-подключение, независимо от того, следует ли блокировать сетевой трафик при отключении VPN.</span><span class="sxs-lookup"><span data-stu-id="38deb-218">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|



## <a name="response"></a><span data-ttu-id="38deb-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="38deb-219">Response</span></span>
<span data-ttu-id="38deb-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38deb-220">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38deb-221">Пример</span><span class="sxs-lookup"><span data-stu-id="38deb-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="38deb-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="38deb-222">Request</span></span>
<span data-ttu-id="38deb-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38deb-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1758

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
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```

### <a name="response"></a><span data-ttu-id="38deb-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="38deb-224">Response</span></span>
<span data-ttu-id="38deb-225">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="38deb-225">Here is an example of the response.</span></span> <span data-ttu-id="38deb-226">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="38deb-226">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="38deb-227">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="38deb-227">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1930

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
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```



