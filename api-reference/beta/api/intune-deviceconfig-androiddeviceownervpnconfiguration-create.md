---
title: Создание Андроиддевицеовнервпнконфигуратион
description: Создание нового объекта Андроиддевицеовнервпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 162d2c3a71a00c62348a251a134ccc398c9ee2f1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706830"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="45491-103">Создание Андроиддевицеовнервпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="45491-103">Create androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="45491-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45491-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45491-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45491-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45491-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45491-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45491-107">Создание нового объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45491-107">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45491-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45491-108">Prerequisites</span></span>
<span data-ttu-id="45491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45491-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45491-111">Permission type</span></span>|<span data-ttu-id="45491-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45491-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45491-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45491-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45491-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45491-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45491-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45491-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45491-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45491-116">Not supported.</span></span>|
|<span data-ttu-id="45491-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45491-117">Application</span></span>|<span data-ttu-id="45491-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45491-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45491-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45491-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45491-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45491-120">Request headers</span></span>
|<span data-ttu-id="45491-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45491-121">Header</span></span>|<span data-ttu-id="45491-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45491-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45491-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45491-123">Authorization</span></span>|<span data-ttu-id="45491-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45491-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45491-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45491-125">Accept</span></span>|<span data-ttu-id="45491-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45491-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45491-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45491-127">Request body</span></span>
<span data-ttu-id="45491-128">В тексте запроса добавьте представление объекта Андроиддевицеовнервпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45491-128">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="45491-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнервпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="45491-129">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="45491-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="45491-130">Property</span></span>|<span data-ttu-id="45491-131">Тип</span><span class="sxs-lookup"><span data-stu-id="45491-131">Type</span></span>|<span data-ttu-id="45491-132">Описание</span><span class="sxs-lookup"><span data-stu-id="45491-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45491-133">id</span><span class="sxs-lookup"><span data-stu-id="45491-133">id</span></span>|<span data-ttu-id="45491-134">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-134">String</span></span>|<span data-ttu-id="45491-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="45491-135">Key of the entity.</span></span> <span data-ttu-id="45491-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45491-137">lastModifiedDateTime</span></span>|<span data-ttu-id="45491-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45491-138">DateTimeOffset</span></span>|<span data-ttu-id="45491-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="45491-139">DateTime the object was last modified.</span></span> <span data-ttu-id="45491-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45491-141">roleScopeTagIds</span></span>|<span data-ttu-id="45491-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="45491-142">String collection</span></span>|<span data-ttu-id="45491-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="45491-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45491-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="45491-145">supportsScopeTags</span></span>|<span data-ttu-id="45491-146">Логический</span><span class="sxs-lookup"><span data-stu-id="45491-146">Boolean</span></span>|<span data-ttu-id="45491-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="45491-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45491-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="45491-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45491-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="45491-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45491-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="45491-150">This property is read-only.</span></span> <span data-ttu-id="45491-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45491-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="45491-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45491-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="45491-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="45491-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="45491-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45491-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="45491-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45491-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="45491-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="45491-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="45491-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45491-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="45491-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45491-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="45491-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="45491-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="45491-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45491-164">createdDateTime</span></span>|<span data-ttu-id="45491-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45491-165">DateTimeOffset</span></span>|<span data-ttu-id="45491-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="45491-166">DateTime the object was created.</span></span> <span data-ttu-id="45491-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-168">description</span><span class="sxs-lookup"><span data-stu-id="45491-168">description</span></span>|<span data-ttu-id="45491-169">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-169">String</span></span>|<span data-ttu-id="45491-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="45491-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45491-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-172">displayName</span><span class="sxs-lookup"><span data-stu-id="45491-172">displayName</span></span>|<span data-ttu-id="45491-173">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-173">String</span></span>|<span data-ttu-id="45491-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="45491-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45491-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-176">version</span><span class="sxs-lookup"><span data-stu-id="45491-176">version</span></span>|<span data-ttu-id="45491-177">Int32</span><span class="sxs-lookup"><span data-stu-id="45491-177">Int32</span></span>|<span data-ttu-id="45491-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="45491-178">Version of the device configuration.</span></span> <span data-ttu-id="45491-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45491-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="45491-180">authenticationMethod</span></span>|[<span data-ttu-id="45491-181">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="45491-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="45491-182">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="45491-182">Authentication method.</span></span> <span data-ttu-id="45491-183">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45491-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="45491-184">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="45491-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="45491-185">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="45491-185">connectionName</span></span>|<span data-ttu-id="45491-186">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-186">String</span></span>|<span data-ttu-id="45491-187">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="45491-187">Connection name displayed to the user.</span></span> <span data-ttu-id="45491-188">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45491-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="45491-189">role</span><span class="sxs-lookup"><span data-stu-id="45491-189">role</span></span>|<span data-ttu-id="45491-190">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-190">String</span></span>|<span data-ttu-id="45491-191">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="45491-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="45491-192">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45491-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="45491-193">область</span><span class="sxs-lookup"><span data-stu-id="45491-193">realm</span></span>|<span data-ttu-id="45491-194">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-194">String</span></span>|<span data-ttu-id="45491-195">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="45491-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="45491-196">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45491-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="45491-197">серверами</span><span class="sxs-lookup"><span data-stu-id="45491-197">servers</span></span>|<span data-ttu-id="45491-198">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="45491-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="45491-199">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="45491-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="45491-200">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="45491-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="45491-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="45491-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="45491-202">Наследуется от [впнконфигуратион](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45491-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="45491-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="45491-203">connectionType</span></span>|[<span data-ttu-id="45491-204">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="45491-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="45491-205">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="45491-205">Connection type.</span></span> <span data-ttu-id="45491-206">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span><span class="sxs-lookup"><span data-stu-id="45491-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="45491-207">проксисервер</span><span class="sxs-lookup"><span data-stu-id="45491-207">proxyServer</span></span>|[<span data-ttu-id="45491-208">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="45491-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="45491-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="45491-209">Proxy server.</span></span>|
|<span data-ttu-id="45491-210">таржетедпаккажеидс</span><span class="sxs-lookup"><span data-stu-id="45491-210">targetedPackageIds</span></span>|<span data-ttu-id="45491-211">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="45491-211">String collection</span></span>|<span data-ttu-id="45491-212">Идентификаторы целевых пакетов приложений.</span><span class="sxs-lookup"><span data-stu-id="45491-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="45491-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="45491-213">targetedMobileApps</span></span>|<span data-ttu-id="45491-214">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="45491-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="45491-215">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="45491-215">Targeted mobile apps.</span></span> <span data-ttu-id="45491-216">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="45491-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="45491-217">Группа</span><span class="sxs-lookup"><span data-stu-id="45491-217">alwaysOn</span></span>|<span data-ttu-id="45491-218">Логический</span><span class="sxs-lookup"><span data-stu-id="45491-218">Boolean</span></span>|<span data-ttu-id="45491-219">Указывает, следует ли включить постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="45491-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="45491-220">алвайсонлоккдовн</span><span class="sxs-lookup"><span data-stu-id="45491-220">alwaysOnLockdown</span></span>|<span data-ttu-id="45491-221">Логический</span><span class="sxs-lookup"><span data-stu-id="45491-221">Boolean</span></span>|<span data-ttu-id="45491-222">Если включено постоянное VPN-подключение, независимо от того, следует ли блокировать сетевой трафик при отключении VPN.</span><span class="sxs-lookup"><span data-stu-id="45491-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="45491-223">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="45491-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="45491-224">Строка</span><span class="sxs-lookup"><span data-stu-id="45491-224">String</span></span>|<span data-ttu-id="45491-225">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="45491-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="45491-226">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="45491-226">customData</span></span>|<span data-ttu-id="45491-227">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="45491-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="45491-228">Пользовательские данные, определяющие пары "ключ-значение", характерные для поставщика услуг VPN.</span><span class="sxs-lookup"><span data-stu-id="45491-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="45491-229">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="45491-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="45491-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="45491-230">customKeyValueData</span></span>|<span data-ttu-id="45491-231">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="45491-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="45491-232">Пользовательские данные, определяющие пары "ключ-значение", характерные для поставщика услуг VPN.</span><span class="sxs-lookup"><span data-stu-id="45491-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="45491-233">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="45491-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="45491-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="45491-234">Response</span></span>
<span data-ttu-id="45491-235">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45491-235">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45491-236">Пример</span><span class="sxs-lookup"><span data-stu-id="45491-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="45491-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="45491-237">Request</span></span>
<span data-ttu-id="45491-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45491-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45491-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="45491-239">Response</span></span>
<span data-ttu-id="45491-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45491-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





