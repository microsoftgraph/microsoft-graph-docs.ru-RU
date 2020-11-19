---
title: Создание Андроидворкпрофилевпнконфигуратион
description: Создание нового объекта Андроидворкпрофилевпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0728c8f7d0f29cbacd3f92ac961944337b7fbf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206590"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="2462b-103">Создание Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2462b-103">Create androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="2462b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2462b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2462b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2462b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2462b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2462b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2462b-107">Создание нового объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2462b-107">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2462b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2462b-108">Prerequisites</span></span>
<span data-ttu-id="2462b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2462b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2462b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2462b-111">Permission type</span></span>|<span data-ttu-id="2462b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2462b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2462b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2462b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2462b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2462b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2462b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2462b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2462b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2462b-116">Not supported.</span></span>|
|<span data-ttu-id="2462b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2462b-117">Application</span></span>|<span data-ttu-id="2462b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2462b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2462b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2462b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2462b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2462b-120">Request headers</span></span>
|<span data-ttu-id="2462b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2462b-121">Header</span></span>|<span data-ttu-id="2462b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2462b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2462b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2462b-123">Authorization</span></span>|<span data-ttu-id="2462b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2462b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2462b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2462b-125">Accept</span></span>|<span data-ttu-id="2462b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2462b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2462b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2462b-127">Request body</span></span>
<span data-ttu-id="2462b-128">В тексте запроса добавьте представление объекта Андроидворкпрофилевпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2462b-128">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="2462b-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилевпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="2462b-129">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="2462b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2462b-130">Property</span></span>|<span data-ttu-id="2462b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2462b-131">Type</span></span>|<span data-ttu-id="2462b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2462b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2462b-133">id</span><span class="sxs-lookup"><span data-stu-id="2462b-133">id</span></span>|<span data-ttu-id="2462b-134">String</span><span class="sxs-lookup"><span data-stu-id="2462b-134">String</span></span>|<span data-ttu-id="2462b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2462b-135">Key of the entity.</span></span> <span data-ttu-id="2462b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2462b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2462b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2462b-138">DateTimeOffset</span></span>|<span data-ttu-id="2462b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2462b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2462b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2462b-141">roleScopeTagIds</span></span>|<span data-ttu-id="2462b-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2462b-142">String collection</span></span>|<span data-ttu-id="2462b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2462b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2462b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2462b-145">supportsScopeTags</span></span>|<span data-ttu-id="2462b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2462b-146">Boolean</span></span>|<span data-ttu-id="2462b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2462b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2462b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2462b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2462b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2462b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2462b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2462b-150">This property is read-only.</span></span> <span data-ttu-id="2462b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2462b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2462b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2462b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2462b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2462b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2462b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2462b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2462b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2462b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2462b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2462b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2462b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2462b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2462b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2462b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2462b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2462b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2462b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2462b-164">createdDateTime</span></span>|<span data-ttu-id="2462b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2462b-165">DateTimeOffset</span></span>|<span data-ttu-id="2462b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2462b-166">DateTime the object was created.</span></span> <span data-ttu-id="2462b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-168">description</span><span class="sxs-lookup"><span data-stu-id="2462b-168">description</span></span>|<span data-ttu-id="2462b-169">String</span><span class="sxs-lookup"><span data-stu-id="2462b-169">String</span></span>|<span data-ttu-id="2462b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2462b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2462b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2462b-172">displayName</span></span>|<span data-ttu-id="2462b-173">String</span><span class="sxs-lookup"><span data-stu-id="2462b-173">String</span></span>|<span data-ttu-id="2462b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2462b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2462b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-176">version</span><span class="sxs-lookup"><span data-stu-id="2462b-176">version</span></span>|<span data-ttu-id="2462b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2462b-177">Int32</span></span>|<span data-ttu-id="2462b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2462b-178">Version of the device configuration.</span></span> <span data-ttu-id="2462b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2462b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2462b-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="2462b-180">connectionName</span></span>|<span data-ttu-id="2462b-181">String</span><span class="sxs-lookup"><span data-stu-id="2462b-181">String</span></span>|<span data-ttu-id="2462b-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2462b-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="2462b-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="2462b-183">connectionType</span></span>|[<span data-ttu-id="2462b-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2462b-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="2462b-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="2462b-185">Connection type.</span></span> <span data-ttu-id="2462b-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`.</span><span class="sxs-lookup"><span data-stu-id="2462b-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="2462b-187">role</span><span class="sxs-lookup"><span data-stu-id="2462b-187">role</span></span>|<span data-ttu-id="2462b-188">String</span><span class="sxs-lookup"><span data-stu-id="2462b-188">String</span></span>|<span data-ttu-id="2462b-189">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="2462b-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="2462b-190">область</span><span class="sxs-lookup"><span data-stu-id="2462b-190">realm</span></span>|<span data-ttu-id="2462b-191">String</span><span class="sxs-lookup"><span data-stu-id="2462b-191">String</span></span>|<span data-ttu-id="2462b-192">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="2462b-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="2462b-193">серверами</span><span class="sxs-lookup"><span data-stu-id="2462b-193">servers</span></span>|<span data-ttu-id="2462b-194">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="2462b-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="2462b-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="2462b-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="2462b-196">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="2462b-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="2462b-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2462b-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2462b-198">распознавания</span><span class="sxs-lookup"><span data-stu-id="2462b-198">fingerprint</span></span>|<span data-ttu-id="2462b-199">String</span><span class="sxs-lookup"><span data-stu-id="2462b-199">String</span></span>|<span data-ttu-id="2462b-200">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="2462b-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="2462b-201">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="2462b-201">customData</span></span>|<span data-ttu-id="2462b-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2462b-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2462b-203">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="2462b-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="2462b-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="2462b-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="2462b-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2462b-205">customKeyValueData</span></span>|<span data-ttu-id="2462b-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2462b-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2462b-207">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="2462b-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="2462b-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="2462b-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="2462b-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="2462b-209">authenticationMethod</span></span>|[<span data-ttu-id="2462b-210">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2462b-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2462b-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2462b-211">Authentication method.</span></span> <span data-ttu-id="2462b-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="2462b-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="2462b-213">проксисервер</span><span class="sxs-lookup"><span data-stu-id="2462b-213">proxyServer</span></span>|[<span data-ttu-id="2462b-214">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="2462b-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2462b-215">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="2462b-215">Proxy server.</span></span>|
|<span data-ttu-id="2462b-216">таржетедпаккажеидс</span><span class="sxs-lookup"><span data-stu-id="2462b-216">targetedPackageIds</span></span>|<span data-ttu-id="2462b-217">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2462b-217">String collection</span></span>|<span data-ttu-id="2462b-218">Идентификаторы целевых пакетов приложений.</span><span class="sxs-lookup"><span data-stu-id="2462b-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="2462b-219">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2462b-219">targetedMobileApps</span></span>|<span data-ttu-id="2462b-220">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2462b-220">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2462b-221">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="2462b-221">Targeted mobile apps.</span></span> <span data-ttu-id="2462b-222">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2462b-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2462b-223">Группа</span><span class="sxs-lookup"><span data-stu-id="2462b-223">alwaysOn</span></span>|<span data-ttu-id="2462b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="2462b-224">Boolean</span></span>|<span data-ttu-id="2462b-225">Указывает, следует ли включить постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="2462b-225">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="2462b-226">алвайсонлоккдовн</span><span class="sxs-lookup"><span data-stu-id="2462b-226">alwaysOnLockdown</span></span>|<span data-ttu-id="2462b-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="2462b-227">Boolean</span></span>|<span data-ttu-id="2462b-228">Если включено постоянное VPN-подключение, независимо от того, следует ли блокировать сетевой трафик при отключении VPN.</span><span class="sxs-lookup"><span data-stu-id="2462b-228">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="2462b-229">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="2462b-229">microsoftTunnelSiteId</span></span>|<span data-ttu-id="2462b-230">String</span><span class="sxs-lookup"><span data-stu-id="2462b-230">String</span></span>|<span data-ttu-id="2462b-231">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="2462b-231">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="2462b-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="2462b-232">Response</span></span>
<span data-ttu-id="2462b-233">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2462b-233">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2462b-234">Пример</span><span class="sxs-lookup"><span data-stu-id="2462b-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="2462b-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="2462b-235">Request</span></span>
<span data-ttu-id="2462b-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2462b-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2422

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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
  "authenticationMethod": "usernameAndPassword",
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="2462b-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="2462b-237">Response</span></span>
<span data-ttu-id="2462b-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2462b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2594

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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
  "authenticationMethod": "usernameAndPassword",
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




