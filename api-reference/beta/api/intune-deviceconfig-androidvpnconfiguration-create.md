---
title: Создание androidVpnConfiguration
description: Создание объекта androidVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 820b3336bd869668de638960d34799172b3f421e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156114"
---
# <a name="create-androidvpnconfiguration"></a><span data-ttu-id="99d26-103">Создание androidVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="99d26-103">Create androidVpnConfiguration</span></span>

<span data-ttu-id="99d26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99d26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99d26-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99d26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99d26-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99d26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99d26-107">Создание объекта [androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99d26-107">Create a new [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99d26-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99d26-108">Prerequisites</span></span>
<span data-ttu-id="99d26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99d26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99d26-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99d26-111">Permission type</span></span>|<span data-ttu-id="99d26-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99d26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99d26-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99d26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99d26-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d26-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99d26-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99d26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99d26-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99d26-116">Not supported.</span></span>|
|<span data-ttu-id="99d26-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99d26-117">Application</span></span>|<span data-ttu-id="99d26-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d26-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99d26-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99d26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="99d26-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99d26-120">Request headers</span></span>
|<span data-ttu-id="99d26-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99d26-121">Header</span></span>|<span data-ttu-id="99d26-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99d26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99d26-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99d26-123">Authorization</span></span>|<span data-ttu-id="99d26-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99d26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99d26-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99d26-125">Accept</span></span>|<span data-ttu-id="99d26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99d26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99d26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99d26-127">Request body</span></span>
<span data-ttu-id="99d26-128">В теле запроса предоставляем представление объекта androidVpnConfiguration в JSON.</span><span class="sxs-lookup"><span data-stu-id="99d26-128">In the request body, supply a JSON representation for the androidVpnConfiguration object.</span></span>

<span data-ttu-id="99d26-129">В следующей таблице показаны свойства, необходимые при создании объекта androidVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="99d26-129">The following table shows the properties that are required when you create the androidVpnConfiguration.</span></span>

|<span data-ttu-id="99d26-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99d26-130">Property</span></span>|<span data-ttu-id="99d26-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99d26-131">Type</span></span>|<span data-ttu-id="99d26-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99d26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99d26-133">id</span><span class="sxs-lookup"><span data-stu-id="99d26-133">id</span></span>|<span data-ttu-id="99d26-134">String</span><span class="sxs-lookup"><span data-stu-id="99d26-134">String</span></span>|<span data-ttu-id="99d26-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99d26-135">Key of the entity.</span></span> <span data-ttu-id="99d26-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99d26-137">lastModifiedDateTime</span></span>|<span data-ttu-id="99d26-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99d26-138">DateTimeOffset</span></span>|<span data-ttu-id="99d26-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="99d26-139">DateTime the object was last modified.</span></span> <span data-ttu-id="99d26-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99d26-141">roleScopeTagIds</span></span>|<span data-ttu-id="99d26-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99d26-142">String collection</span></span>|<span data-ttu-id="99d26-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="99d26-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="99d26-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="99d26-145">supportsScopeTags</span></span>|<span data-ttu-id="99d26-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="99d26-146">Boolean</span></span>|<span data-ttu-id="99d26-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="99d26-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="99d26-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="99d26-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="99d26-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="99d26-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="99d26-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="99d26-150">This property is read-only.</span></span> <span data-ttu-id="99d26-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="99d26-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="99d26-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="99d26-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="99d26-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="99d26-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="99d26-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="99d26-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="99d26-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="99d26-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="99d26-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="99d26-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="99d26-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="99d26-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="99d26-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="99d26-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="99d26-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="99d26-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="99d26-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99d26-164">createdDateTime</span></span>|<span data-ttu-id="99d26-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99d26-165">DateTimeOffset</span></span>|<span data-ttu-id="99d26-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="99d26-166">DateTime the object was created.</span></span> <span data-ttu-id="99d26-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-168">description</span><span class="sxs-lookup"><span data-stu-id="99d26-168">description</span></span>|<span data-ttu-id="99d26-169">String</span><span class="sxs-lookup"><span data-stu-id="99d26-169">String</span></span>|<span data-ttu-id="99d26-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="99d26-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="99d26-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-172">displayName</span><span class="sxs-lookup"><span data-stu-id="99d26-172">displayName</span></span>|<span data-ttu-id="99d26-173">String</span><span class="sxs-lookup"><span data-stu-id="99d26-173">String</span></span>|<span data-ttu-id="99d26-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="99d26-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="99d26-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-176">version</span><span class="sxs-lookup"><span data-stu-id="99d26-176">version</span></span>|<span data-ttu-id="99d26-177">Int32</span><span class="sxs-lookup"><span data-stu-id="99d26-177">Int32</span></span>|<span data-ttu-id="99d26-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="99d26-178">Version of the device configuration.</span></span> <span data-ttu-id="99d26-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99d26-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99d26-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="99d26-180">connectionName</span></span>|<span data-ttu-id="99d26-181">String</span><span class="sxs-lookup"><span data-stu-id="99d26-181">String</span></span>|<span data-ttu-id="99d26-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="99d26-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="99d26-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="99d26-183">connectionType</span></span>|[<span data-ttu-id="99d26-184">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="99d26-184">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="99d26-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="99d26-185">Connection type.</span></span> <span data-ttu-id="99d26-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span><span class="sxs-lookup"><span data-stu-id="99d26-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="99d26-187">role</span><span class="sxs-lookup"><span data-stu-id="99d26-187">role</span></span>|<span data-ttu-id="99d26-188">String</span><span class="sxs-lookup"><span data-stu-id="99d26-188">String</span></span>|<span data-ttu-id="99d26-189">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="99d26-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="99d26-190">realm</span><span class="sxs-lookup"><span data-stu-id="99d26-190">realm</span></span>|<span data-ttu-id="99d26-191">String</span><span class="sxs-lookup"><span data-stu-id="99d26-191">String</span></span>|<span data-ttu-id="99d26-192">Область, когда для типа подключения установлено безопасное пульса.</span><span class="sxs-lookup"><span data-stu-id="99d26-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="99d26-193">серверы</span><span class="sxs-lookup"><span data-stu-id="99d26-193">servers</span></span>|<span data-ttu-id="99d26-194">[Коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="99d26-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="99d26-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="99d26-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="99d26-196">Убедитесь, что конечные пользователи имеют доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="99d26-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="99d26-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="99d26-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="99d26-198">fingerprint</span><span class="sxs-lookup"><span data-stu-id="99d26-198">fingerprint</span></span>|<span data-ttu-id="99d26-199">String</span><span class="sxs-lookup"><span data-stu-id="99d26-199">String</span></span>|<span data-ttu-id="99d26-200">Отпечаток пальца — это строка, которая будет использоваться для проверки доверия VPN-сервера, что применимо только в том случае, если типом подключения является VPN Check Point Vpn.</span><span class="sxs-lookup"><span data-stu-id="99d26-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="99d26-201">customData</span><span class="sxs-lookup"><span data-stu-id="99d26-201">customData</span></span>|<span data-ttu-id="99d26-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="99d26-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="99d26-203">Пользовательские данные, если для типа подключения установлено citrix.</span><span class="sxs-lookup"><span data-stu-id="99d26-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="99d26-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="99d26-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="99d26-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="99d26-205">customKeyValueData</span></span>|<span data-ttu-id="99d26-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="99d26-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="99d26-207">Пользовательские данные, если для типа подключения установлено citrix.</span><span class="sxs-lookup"><span data-stu-id="99d26-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="99d26-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="99d26-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="99d26-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="99d26-209">authenticationMethod</span></span>|[<span data-ttu-id="99d26-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="99d26-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="99d26-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="99d26-211">Authentication method.</span></span> <span data-ttu-id="99d26-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="99d26-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="99d26-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="99d26-213">Response</span></span>
<span data-ttu-id="99d26-214">В случае успеха этот метод возвращает код отклика и объект `201 Created` [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99d26-214">If successful, this method returns a `201 Created` response code and a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99d26-215">Пример</span><span class="sxs-lookup"><span data-stu-id="99d26-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="99d26-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="99d26-216">Request</span></span>
<span data-ttu-id="99d26-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99d26-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1751

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
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
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="99d26-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="99d26-218">Response</span></span>
<span data-ttu-id="99d26-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99d26-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1923

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```




