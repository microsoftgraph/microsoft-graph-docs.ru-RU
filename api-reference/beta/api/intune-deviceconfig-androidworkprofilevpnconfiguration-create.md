---
title: Создание Андроидворкпрофилевпнконфигуратион
description: Создание нового объекта Андроидворкпрофилевпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5dd302986954d9c9999204b4a89c5f4137c743dd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949898"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="15c21-103">Создание Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="15c21-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="15c21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15c21-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15c21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15c21-106">Создание нового объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15c21-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15c21-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15c21-107">Prerequisites</span></span>
<span data-ttu-id="15c21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15c21-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15c21-110">Permission type</span></span>|<span data-ttu-id="15c21-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15c21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15c21-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15c21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15c21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15c21-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15c21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15c21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c21-115">Not supported.</span></span>|
|<span data-ttu-id="15c21-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15c21-116">Application</span></span>|<span data-ttu-id="15c21-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c21-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15c21-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15c21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15c21-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15c21-119">Request headers</span></span>
|<span data-ttu-id="15c21-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15c21-120">Header</span></span>|<span data-ttu-id="15c21-121">Значение</span><span class="sxs-lookup"><span data-stu-id="15c21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15c21-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15c21-122">Authorization</span></span>|<span data-ttu-id="15c21-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15c21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15c21-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15c21-124">Accept</span></span>|<span data-ttu-id="15c21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15c21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c21-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15c21-126">Request body</span></span>
<span data-ttu-id="15c21-127">В тексте запроса добавьте представление объекта Андроидворкпрофилевпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15c21-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="15c21-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилевпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="15c21-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="15c21-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="15c21-129">Property</span></span>|<span data-ttu-id="15c21-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15c21-130">Type</span></span>|<span data-ttu-id="15c21-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15c21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c21-132">id</span><span class="sxs-lookup"><span data-stu-id="15c21-132">id</span></span>|<span data-ttu-id="15c21-133">String</span><span class="sxs-lookup"><span data-stu-id="15c21-133">String</span></span>|<span data-ttu-id="15c21-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15c21-134">Key of the entity.</span></span> <span data-ttu-id="15c21-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15c21-136">lastModifiedDateTime</span></span>|<span data-ttu-id="15c21-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15c21-137">DateTimeOffset</span></span>|<span data-ttu-id="15c21-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="15c21-138">DateTime the object was last modified.</span></span> <span data-ttu-id="15c21-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15c21-140">roleScopeTagIds</span></span>|<span data-ttu-id="15c21-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="15c21-141">String collection</span></span>|<span data-ttu-id="15c21-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="15c21-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15c21-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="15c21-144">supportsScopeTags</span></span>|<span data-ttu-id="15c21-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="15c21-145">Boolean</span></span>|<span data-ttu-id="15c21-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="15c21-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15c21-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="15c21-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15c21-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="15c21-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15c21-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15c21-149">This property is read-only.</span></span> <span data-ttu-id="15c21-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15c21-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="15c21-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15c21-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="15c21-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15c21-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="15c21-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15c21-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="15c21-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15c21-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="15c21-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15c21-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="15c21-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15c21-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="15c21-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15c21-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="15c21-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15c21-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="15c21-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15c21-163">createdDateTime</span></span>|<span data-ttu-id="15c21-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15c21-164">DateTimeOffset</span></span>|<span data-ttu-id="15c21-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="15c21-165">DateTime the object was created.</span></span> <span data-ttu-id="15c21-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-167">description</span><span class="sxs-lookup"><span data-stu-id="15c21-167">description</span></span>|<span data-ttu-id="15c21-168">String</span><span class="sxs-lookup"><span data-stu-id="15c21-168">String</span></span>|<span data-ttu-id="15c21-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15c21-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15c21-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-171">displayName</span><span class="sxs-lookup"><span data-stu-id="15c21-171">displayName</span></span>|<span data-ttu-id="15c21-172">Строка</span><span class="sxs-lookup"><span data-stu-id="15c21-172">String</span></span>|<span data-ttu-id="15c21-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15c21-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15c21-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-175">version</span><span class="sxs-lookup"><span data-stu-id="15c21-175">version</span></span>|<span data-ttu-id="15c21-176">Int32</span><span class="sxs-lookup"><span data-stu-id="15c21-176">Int32</span></span>|<span data-ttu-id="15c21-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15c21-177">Version of the device configuration.</span></span> <span data-ttu-id="15c21-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15c21-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15c21-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="15c21-179">connectionName</span></span>|<span data-ttu-id="15c21-180">Строка</span><span class="sxs-lookup"><span data-stu-id="15c21-180">String</span></span>|<span data-ttu-id="15c21-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="15c21-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="15c21-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="15c21-182">connectionType</span></span>|[<span data-ttu-id="15c21-183">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="15c21-183">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="15c21-184">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="15c21-184">Connection type.</span></span> <span data-ttu-id="15c21-185">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="15c21-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="15c21-186">role</span><span class="sxs-lookup"><span data-stu-id="15c21-186">role</span></span>|<span data-ttu-id="15c21-187">Строка</span><span class="sxs-lookup"><span data-stu-id="15c21-187">String</span></span>|<span data-ttu-id="15c21-188">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="15c21-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="15c21-189">область</span><span class="sxs-lookup"><span data-stu-id="15c21-189">realm</span></span>|<span data-ttu-id="15c21-190">Строка</span><span class="sxs-lookup"><span data-stu-id="15c21-190">String</span></span>|<span data-ttu-id="15c21-191">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="15c21-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="15c21-192">серверами</span><span class="sxs-lookup"><span data-stu-id="15c21-192">servers</span></span>|<span data-ttu-id="15c21-193">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="15c21-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="15c21-194">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="15c21-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="15c21-195">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="15c21-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="15c21-196">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="15c21-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="15c21-197">распознавания</span><span class="sxs-lookup"><span data-stu-id="15c21-197">fingerprint</span></span>|<span data-ttu-id="15c21-198">Строка</span><span class="sxs-lookup"><span data-stu-id="15c21-198">String</span></span>|<span data-ttu-id="15c21-199">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="15c21-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="15c21-200">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="15c21-200">customData</span></span>|<span data-ttu-id="15c21-201">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="15c21-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="15c21-202">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="15c21-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="15c21-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="15c21-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="15c21-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="15c21-204">customKeyValueData</span></span>|<span data-ttu-id="15c21-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="15c21-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="15c21-206">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="15c21-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="15c21-207">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="15c21-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="15c21-208">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="15c21-208">authenticationMethod</span></span>|[<span data-ttu-id="15c21-209">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="15c21-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="15c21-210">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="15c21-210">Authentication method.</span></span> <span data-ttu-id="15c21-211">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="15c21-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="15c21-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c21-212">Response</span></span>
<span data-ttu-id="15c21-213">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15c21-213">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15c21-214">Пример</span><span class="sxs-lookup"><span data-stu-id="15c21-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="15c21-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="15c21-215">Request</span></span>
<span data-ttu-id="15c21-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15c21-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="15c21-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c21-217">Response</span></span>
<span data-ttu-id="15c21-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15c21-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





