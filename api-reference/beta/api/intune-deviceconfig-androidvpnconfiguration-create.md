---
title: Создание androidVpnConfiguration
description: Создайте новый объект androidVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eef270f2c97f0e566c36f5e5206c1e05714bce83
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137674"
---
# <a name="create-androidvpnconfiguration"></a><span data-ttu-id="717d5-103">Создание androidVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="717d5-103">Create androidVpnConfiguration</span></span>

<span data-ttu-id="717d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="717d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="717d5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="717d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="717d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="717d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="717d5-107">Создайте новый [объект androidVpnConfiguration.](../resources/intune-deviceconfig-androidvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="717d5-107">Create a new [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="717d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="717d5-108">Prerequisites</span></span>
<span data-ttu-id="717d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="717d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="717d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="717d5-111">Permission type</span></span>|<span data-ttu-id="717d5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="717d5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="717d5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="717d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="717d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="717d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="717d5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="717d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="717d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="717d5-116">Not supported.</span></span>|
|<span data-ttu-id="717d5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="717d5-117">Application</span></span>|<span data-ttu-id="717d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="717d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="717d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="717d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="717d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="717d5-120">Request headers</span></span>
|<span data-ttu-id="717d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="717d5-121">Header</span></span>|<span data-ttu-id="717d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="717d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="717d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="717d5-123">Authorization</span></span>|<span data-ttu-id="717d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="717d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="717d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="717d5-125">Accept</span></span>|<span data-ttu-id="717d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="717d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="717d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="717d5-127">Request body</span></span>
<span data-ttu-id="717d5-128">В теле запроса предоставляем представление JSON для объекта AndroidVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="717d5-128">In the request body, supply a JSON representation for the androidVpnConfiguration object.</span></span>

<span data-ttu-id="717d5-129">В следующей таблице показаны свойства, необходимые при создании androidVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="717d5-129">The following table shows the properties that are required when you create the androidVpnConfiguration.</span></span>

|<span data-ttu-id="717d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="717d5-130">Property</span></span>|<span data-ttu-id="717d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="717d5-131">Type</span></span>|<span data-ttu-id="717d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="717d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="717d5-133">id</span><span class="sxs-lookup"><span data-stu-id="717d5-133">id</span></span>|<span data-ttu-id="717d5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-134">String</span></span>|<span data-ttu-id="717d5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="717d5-135">Key of the entity.</span></span> <span data-ttu-id="717d5-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="717d5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="717d5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="717d5-138">DateTimeOffset</span></span>|<span data-ttu-id="717d5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="717d5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="717d5-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="717d5-141">roleScopeTagIds</span></span>|<span data-ttu-id="717d5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="717d5-142">String collection</span></span>|<span data-ttu-id="717d5-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="717d5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="717d5-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="717d5-145">supportsScopeTags</span></span>|<span data-ttu-id="717d5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="717d5-146">Boolean</span></span>|<span data-ttu-id="717d5-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="717d5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="717d5-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="717d5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="717d5-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="717d5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="717d5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="717d5-150">This property is read-only.</span></span> <span data-ttu-id="717d5-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="717d5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="717d5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="717d5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="717d5-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="717d5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="717d5-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="717d5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="717d5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="717d5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="717d5-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="717d5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="717d5-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="717d5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="717d5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="717d5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="717d5-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="717d5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="717d5-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="717d5-164">createdDateTime</span></span>|<span data-ttu-id="717d5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="717d5-165">DateTimeOffset</span></span>|<span data-ttu-id="717d5-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="717d5-166">DateTime the object was created.</span></span> <span data-ttu-id="717d5-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-168">description</span><span class="sxs-lookup"><span data-stu-id="717d5-168">description</span></span>|<span data-ttu-id="717d5-169">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-169">String</span></span>|<span data-ttu-id="717d5-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="717d5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="717d5-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="717d5-172">displayName</span></span>|<span data-ttu-id="717d5-173">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-173">String</span></span>|<span data-ttu-id="717d5-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="717d5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="717d5-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-176">version</span><span class="sxs-lookup"><span data-stu-id="717d5-176">version</span></span>|<span data-ttu-id="717d5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="717d5-177">Int32</span></span>|<span data-ttu-id="717d5-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="717d5-178">Version of the device configuration.</span></span> <span data-ttu-id="717d5-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="717d5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="717d5-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="717d5-180">connectionName</span></span>|<span data-ttu-id="717d5-181">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-181">String</span></span>|<span data-ttu-id="717d5-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="717d5-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="717d5-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="717d5-183">connectionType</span></span>|[<span data-ttu-id="717d5-184">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="717d5-184">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="717d5-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="717d5-185">Connection type.</span></span> <span data-ttu-id="717d5-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span><span class="sxs-lookup"><span data-stu-id="717d5-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="717d5-187">role</span><span class="sxs-lookup"><span data-stu-id="717d5-187">role</span></span>|<span data-ttu-id="717d5-188">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-188">String</span></span>|<span data-ttu-id="717d5-189">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="717d5-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="717d5-190">realm</span><span class="sxs-lookup"><span data-stu-id="717d5-190">realm</span></span>|<span data-ttu-id="717d5-191">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-191">String</span></span>|<span data-ttu-id="717d5-192">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="717d5-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="717d5-193">серверы</span><span class="sxs-lookup"><span data-stu-id="717d5-193">servers</span></span>|<span data-ttu-id="717d5-194">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="717d5-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="717d5-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="717d5-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="717d5-196">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="717d5-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="717d5-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="717d5-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="717d5-198">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="717d5-198">fingerprint</span></span>|<span data-ttu-id="717d5-199">Строка</span><span class="sxs-lookup"><span data-stu-id="717d5-199">String</span></span>|<span data-ttu-id="717d5-200">Отпечатки пальцев — это строка, которая будет использоваться для проверки доверия к VPN-серверу, которая применяется только в том случае, если тип подключения — VPN Check Point Capsule.</span><span class="sxs-lookup"><span data-stu-id="717d5-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="717d5-201">customData</span><span class="sxs-lookup"><span data-stu-id="717d5-201">customData</span></span>|<span data-ttu-id="717d5-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="717d5-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="717d5-203">Настраиваемые данные при наборе типа подключения к Citrix.</span><span class="sxs-lookup"><span data-stu-id="717d5-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="717d5-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="717d5-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="717d5-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="717d5-205">customKeyValueData</span></span>|<span data-ttu-id="717d5-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="717d5-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="717d5-207">Настраиваемые данные при наборе типа подключения к Citrix.</span><span class="sxs-lookup"><span data-stu-id="717d5-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="717d5-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="717d5-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="717d5-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="717d5-209">authenticationMethod</span></span>|[<span data-ttu-id="717d5-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="717d5-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="717d5-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="717d5-211">Authentication method.</span></span> <span data-ttu-id="717d5-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="717d5-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="717d5-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="717d5-213">Response</span></span>
<span data-ttu-id="717d5-214">В случае успеха этот метод возвращает код отклика и `201 Created` [объект androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="717d5-214">If successful, this method returns a `201 Created` response code and a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="717d5-215">Пример</span><span class="sxs-lookup"><span data-stu-id="717d5-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="717d5-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="717d5-216">Request</span></span>
<span data-ttu-id="717d5-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="717d5-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="717d5-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="717d5-218">Response</span></span>
<span data-ttu-id="717d5-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="717d5-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




