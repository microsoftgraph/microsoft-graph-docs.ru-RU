---
title: Обновление Андроидворкпрофилевпнконфигуратион
description: Обновление свойств объекта Андроидворкпрофилевпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0456ad3282119d3927eaeb943dec3babb984d51
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949870"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="6c07f-103">Обновление Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6c07f-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="6c07f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c07f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c07f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c07f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c07f-106">Обновление свойств объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6c07f-106">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c07f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c07f-107">Prerequisites</span></span>
<span data-ttu-id="6c07f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c07f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c07f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c07f-110">Permission type</span></span>|<span data-ttu-id="6c07f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c07f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c07f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c07f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c07f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c07f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c07f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c07f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c07f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c07f-115">Not supported.</span></span>|
|<span data-ttu-id="6c07f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c07f-116">Application</span></span>|<span data-ttu-id="6c07f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c07f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c07f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c07f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6c07f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c07f-119">Request headers</span></span>
|<span data-ttu-id="6c07f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c07f-120">Header</span></span>|<span data-ttu-id="6c07f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6c07f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c07f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c07f-122">Authorization</span></span>|<span data-ttu-id="6c07f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c07f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c07f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6c07f-124">Accept</span></span>|<span data-ttu-id="6c07f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c07f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c07f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c07f-126">Request body</span></span>
<span data-ttu-id="6c07f-127">В тексте запроса добавьте представление объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c07f-127">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="6c07f-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-128">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="6c07f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c07f-129">Property</span></span>|<span data-ttu-id="6c07f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6c07f-130">Type</span></span>|<span data-ttu-id="6c07f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6c07f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c07f-132">id</span><span class="sxs-lookup"><span data-stu-id="6c07f-132">id</span></span>|<span data-ttu-id="6c07f-133">String</span><span class="sxs-lookup"><span data-stu-id="6c07f-133">String</span></span>|<span data-ttu-id="6c07f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6c07f-134">Key of the entity.</span></span> <span data-ttu-id="6c07f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c07f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6c07f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c07f-137">DateTimeOffset</span></span>|<span data-ttu-id="6c07f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6c07f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6c07f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c07f-140">roleScopeTagIds</span></span>|<span data-ttu-id="6c07f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6c07f-141">String collection</span></span>|<span data-ttu-id="6c07f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6c07f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c07f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6c07f-144">supportsScopeTags</span></span>|<span data-ttu-id="6c07f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c07f-145">Boolean</span></span>|<span data-ttu-id="6c07f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6c07f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c07f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6c07f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c07f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6c07f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c07f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c07f-149">This property is read-only.</span></span> <span data-ttu-id="6c07f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c07f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6c07f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c07f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6c07f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6c07f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6c07f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c07f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6c07f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c07f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6c07f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6c07f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6c07f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c07f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6c07f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c07f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6c07f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6c07f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6c07f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c07f-163">createdDateTime</span></span>|<span data-ttu-id="6c07f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c07f-164">DateTimeOffset</span></span>|<span data-ttu-id="6c07f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6c07f-165">DateTime the object was created.</span></span> <span data-ttu-id="6c07f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-167">description</span><span class="sxs-lookup"><span data-stu-id="6c07f-167">description</span></span>|<span data-ttu-id="6c07f-168">String</span><span class="sxs-lookup"><span data-stu-id="6c07f-168">String</span></span>|<span data-ttu-id="6c07f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6c07f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c07f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6c07f-171">displayName</span></span>|<span data-ttu-id="6c07f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="6c07f-172">String</span></span>|<span data-ttu-id="6c07f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6c07f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c07f-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-175">version</span><span class="sxs-lookup"><span data-stu-id="6c07f-175">version</span></span>|<span data-ttu-id="6c07f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6c07f-176">Int32</span></span>|<span data-ttu-id="6c07f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6c07f-177">Version of the device configuration.</span></span> <span data-ttu-id="6c07f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c07f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c07f-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="6c07f-179">connectionName</span></span>|<span data-ttu-id="6c07f-180">Строка</span><span class="sxs-lookup"><span data-stu-id="6c07f-180">String</span></span>|<span data-ttu-id="6c07f-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c07f-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="6c07f-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="6c07f-182">connectionType</span></span>|[<span data-ttu-id="6c07f-183">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6c07f-183">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="6c07f-184">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="6c07f-184">Connection type.</span></span> <span data-ttu-id="6c07f-185">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="6c07f-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="6c07f-186">role</span><span class="sxs-lookup"><span data-stu-id="6c07f-186">role</span></span>|<span data-ttu-id="6c07f-187">Строка</span><span class="sxs-lookup"><span data-stu-id="6c07f-187">String</span></span>|<span data-ttu-id="6c07f-188">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="6c07f-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="6c07f-189">область</span><span class="sxs-lookup"><span data-stu-id="6c07f-189">realm</span></span>|<span data-ttu-id="6c07f-190">Строка</span><span class="sxs-lookup"><span data-stu-id="6c07f-190">String</span></span>|<span data-ttu-id="6c07f-191">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="6c07f-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="6c07f-192">серверами</span><span class="sxs-lookup"><span data-stu-id="6c07f-192">servers</span></span>|<span data-ttu-id="6c07f-193">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="6c07f-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6c07f-194">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="6c07f-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="6c07f-195">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="6c07f-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6c07f-196">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6c07f-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6c07f-197">распознавания</span><span class="sxs-lookup"><span data-stu-id="6c07f-197">fingerprint</span></span>|<span data-ttu-id="6c07f-198">Строка</span><span class="sxs-lookup"><span data-stu-id="6c07f-198">String</span></span>|<span data-ttu-id="6c07f-199">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="6c07f-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="6c07f-200">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="6c07f-200">customData</span></span>|<span data-ttu-id="6c07f-201">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6c07f-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="6c07f-202">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="6c07f-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="6c07f-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="6c07f-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="6c07f-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="6c07f-204">customKeyValueData</span></span>|<span data-ttu-id="6c07f-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6c07f-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6c07f-206">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="6c07f-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="6c07f-207">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="6c07f-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="6c07f-208">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6c07f-208">authenticationMethod</span></span>|[<span data-ttu-id="6c07f-209">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="6c07f-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6c07f-210">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6c07f-210">Authentication method.</span></span> <span data-ttu-id="6c07f-211">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6c07f-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="6c07f-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c07f-212">Response</span></span>
<span data-ttu-id="6c07f-213">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c07f-213">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c07f-214">Пример</span><span class="sxs-lookup"><span data-stu-id="6c07f-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c07f-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c07f-215">Request</span></span>
<span data-ttu-id="6c07f-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c07f-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1762

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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="6c07f-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c07f-217">Response</span></span>
<span data-ttu-id="6c07f-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c07f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1934

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
  "authenticationMethod": "usernameAndPassword"
}
```





