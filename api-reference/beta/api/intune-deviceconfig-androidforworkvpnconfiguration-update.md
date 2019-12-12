---
title: Обновление androidForWorkVpnConfiguration
description: Обновление свойств объекта androidForWorkVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d216adca1293546480a9d62d4dd7325dc9472233
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954547"
---
# <a name="update-androidforworkvpnconfiguration"></a><span data-ttu-id="0e731-103">Обновление androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e731-103">Update androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="0e731-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e731-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e731-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e731-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e731-106">Обновление свойств объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0e731-106">Update the properties of a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e731-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e731-107">Prerequisites</span></span>
<span data-ttu-id="0e731-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e731-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e731-110">Permission type</span></span>|<span data-ttu-id="0e731-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e731-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e731-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e731-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e731-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e731-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e731-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e731-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e731-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e731-115">Not supported.</span></span>|
|<span data-ttu-id="0e731-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e731-116">Application</span></span>|<span data-ttu-id="0e731-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e731-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e731-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e731-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0e731-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e731-119">Request headers</span></span>
|<span data-ttu-id="0e731-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e731-120">Header</span></span>|<span data-ttu-id="0e731-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e731-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e731-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e731-122">Authorization</span></span>|<span data-ttu-id="0e731-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e731-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e731-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e731-124">Accept</span></span>|<span data-ttu-id="0e731-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e731-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e731-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e731-126">Request body</span></span>
<span data-ttu-id="0e731-127">В тексте запроса добавьте представление объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e731-127">In the request body, supply a JSON representation for the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

<span data-ttu-id="0e731-128">В следующей таблице приведены свойства, необходимые при создании [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-128">The following table shows the properties that are required when you create the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span></span>

|<span data-ttu-id="0e731-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e731-129">Property</span></span>|<span data-ttu-id="0e731-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e731-130">Type</span></span>|<span data-ttu-id="0e731-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e731-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e731-132">id</span><span class="sxs-lookup"><span data-stu-id="0e731-132">id</span></span>|<span data-ttu-id="0e731-133">String</span><span class="sxs-lookup"><span data-stu-id="0e731-133">String</span></span>|<span data-ttu-id="0e731-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e731-134">Key of the entity.</span></span> <span data-ttu-id="0e731-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e731-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0e731-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e731-137">DateTimeOffset</span></span>|<span data-ttu-id="0e731-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0e731-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0e731-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e731-140">roleScopeTagIds</span></span>|<span data-ttu-id="0e731-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0e731-141">String collection</span></span>|<span data-ttu-id="0e731-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0e731-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e731-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0e731-144">supportsScopeTags</span></span>|<span data-ttu-id="0e731-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e731-145">Boolean</span></span>|<span data-ttu-id="0e731-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0e731-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e731-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0e731-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e731-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0e731-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e731-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e731-149">This property is read-only.</span></span> <span data-ttu-id="0e731-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e731-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0e731-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e731-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0e731-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e731-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0e731-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e731-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0e731-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e731-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0e731-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e731-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0e731-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e731-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0e731-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e731-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0e731-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e731-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0e731-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e731-163">createdDateTime</span></span>|<span data-ttu-id="0e731-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e731-164">DateTimeOffset</span></span>|<span data-ttu-id="0e731-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0e731-165">DateTime the object was created.</span></span> <span data-ttu-id="0e731-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-167">description</span><span class="sxs-lookup"><span data-stu-id="0e731-167">description</span></span>|<span data-ttu-id="0e731-168">String</span><span class="sxs-lookup"><span data-stu-id="0e731-168">String</span></span>|<span data-ttu-id="0e731-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e731-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e731-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0e731-171">displayName</span></span>|<span data-ttu-id="0e731-172">Строка</span><span class="sxs-lookup"><span data-stu-id="0e731-172">String</span></span>|<span data-ttu-id="0e731-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e731-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e731-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-175">version</span><span class="sxs-lookup"><span data-stu-id="0e731-175">version</span></span>|<span data-ttu-id="0e731-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0e731-176">Int32</span></span>|<span data-ttu-id="0e731-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e731-177">Version of the device configuration.</span></span> <span data-ttu-id="0e731-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e731-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e731-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="0e731-179">connectionName</span></span>|<span data-ttu-id="0e731-180">Строка</span><span class="sxs-lookup"><span data-stu-id="0e731-180">String</span></span>|<span data-ttu-id="0e731-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e731-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="0e731-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="0e731-182">connectionType</span></span>|[<span data-ttu-id="0e731-183">Androidforworkvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="0e731-183">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="0e731-184">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="0e731-184">Connection type.</span></span> <span data-ttu-id="0e731-185">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="0e731-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="0e731-186">role</span><span class="sxs-lookup"><span data-stu-id="0e731-186">role</span></span>|<span data-ttu-id="0e731-187">Строка</span><span class="sxs-lookup"><span data-stu-id="0e731-187">String</span></span>|<span data-ttu-id="0e731-188">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="0e731-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="0e731-189">область</span><span class="sxs-lookup"><span data-stu-id="0e731-189">realm</span></span>|<span data-ttu-id="0e731-190">Строка</span><span class="sxs-lookup"><span data-stu-id="0e731-190">String</span></span>|<span data-ttu-id="0e731-191">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="0e731-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="0e731-192">серверами</span><span class="sxs-lookup"><span data-stu-id="0e731-192">servers</span></span>|<span data-ttu-id="0e731-193">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="0e731-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0e731-194">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="0e731-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="0e731-195">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="0e731-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0e731-196">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0e731-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0e731-197">распознавания</span><span class="sxs-lookup"><span data-stu-id="0e731-197">fingerprint</span></span>|<span data-ttu-id="0e731-198">Строка</span><span class="sxs-lookup"><span data-stu-id="0e731-198">String</span></span>|<span data-ttu-id="0e731-199">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="0e731-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="0e731-200">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="0e731-200">customData</span></span>|<span data-ttu-id="0e731-201">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0e731-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0e731-202">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="0e731-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="0e731-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="0e731-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="0e731-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0e731-204">customKeyValueData</span></span>|<span data-ttu-id="0e731-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0e731-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0e731-206">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="0e731-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="0e731-207">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="0e731-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="0e731-208">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="0e731-208">authenticationMethod</span></span>|[<span data-ttu-id="0e731-209">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0e731-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0e731-210">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0e731-210">Authentication method.</span></span> <span data-ttu-id="0e731-211">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0e731-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="0e731-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e731-212">Response</span></span>
<span data-ttu-id="0e731-213">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e731-213">If successful, this method returns a `200 OK` response code and an updated [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e731-214">Пример</span><span class="sxs-lookup"><span data-stu-id="0e731-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e731-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e731-215">Request</span></span>
<span data-ttu-id="0e731-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e731-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1758

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="0e731-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e731-217">Response</span></span>
<span data-ttu-id="0e731-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e731-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1930

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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





