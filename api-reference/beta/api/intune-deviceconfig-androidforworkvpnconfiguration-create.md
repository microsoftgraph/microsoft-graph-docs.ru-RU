---
title: Создание androidForWorkVpnConfiguration
description: Создание нового объекта androidForWorkVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55ea637d205e7c5302c47139831e8a66f27d95e4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43345347"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="b649f-103">Создание androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b649f-103">Create androidForWorkVpnConfiguration</span></span>

<span data-ttu-id="b649f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b649f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b649f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b649f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b649f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b649f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b649f-107">Создание нового объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b649f-107">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b649f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b649f-108">Prerequisites</span></span>
<span data-ttu-id="b649f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b649f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b649f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b649f-111">Permission type</span></span>|<span data-ttu-id="b649f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b649f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b649f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b649f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b649f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b649f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b649f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b649f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b649f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b649f-116">Not supported.</span></span>|
|<span data-ttu-id="b649f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b649f-117">Application</span></span>|<span data-ttu-id="b649f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b649f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b649f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b649f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b649f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b649f-120">Request headers</span></span>
|<span data-ttu-id="b649f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b649f-121">Header</span></span>|<span data-ttu-id="b649f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b649f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b649f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b649f-123">Authorization</span></span>|<span data-ttu-id="b649f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b649f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b649f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b649f-125">Accept</span></span>|<span data-ttu-id="b649f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b649f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b649f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b649f-127">Request body</span></span>
<span data-ttu-id="b649f-128">В тексте запроса добавьте представление объекта androidForWorkVpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b649f-128">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="b649f-129">В следующей таблице приведены свойства, необходимые при создании androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b649f-129">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="b649f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b649f-130">Property</span></span>|<span data-ttu-id="b649f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b649f-131">Type</span></span>|<span data-ttu-id="b649f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b649f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b649f-133">id</span><span class="sxs-lookup"><span data-stu-id="b649f-133">id</span></span>|<span data-ttu-id="b649f-134">String</span><span class="sxs-lookup"><span data-stu-id="b649f-134">String</span></span>|<span data-ttu-id="b649f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b649f-135">Key of the entity.</span></span> <span data-ttu-id="b649f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b649f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b649f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b649f-138">DateTimeOffset</span></span>|<span data-ttu-id="b649f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b649f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b649f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b649f-141">roleScopeTagIds</span></span>|<span data-ttu-id="b649f-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b649f-142">String collection</span></span>|<span data-ttu-id="b649f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b649f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b649f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b649f-145">supportsScopeTags</span></span>|<span data-ttu-id="b649f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b649f-146">Boolean</span></span>|<span data-ttu-id="b649f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b649f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b649f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b649f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b649f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b649f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b649f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b649f-150">This property is read-only.</span></span> <span data-ttu-id="b649f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b649f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b649f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b649f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b649f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b649f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b649f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b649f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b649f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b649f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b649f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b649f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b649f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b649f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b649f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b649f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b649f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b649f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b649f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b649f-164">createdDateTime</span></span>|<span data-ttu-id="b649f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b649f-165">DateTimeOffset</span></span>|<span data-ttu-id="b649f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b649f-166">DateTime the object was created.</span></span> <span data-ttu-id="b649f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-168">description</span><span class="sxs-lookup"><span data-stu-id="b649f-168">description</span></span>|<span data-ttu-id="b649f-169">String</span><span class="sxs-lookup"><span data-stu-id="b649f-169">String</span></span>|<span data-ttu-id="b649f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b649f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b649f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b649f-172">displayName</span></span>|<span data-ttu-id="b649f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b649f-173">String</span></span>|<span data-ttu-id="b649f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b649f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b649f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-176">version</span><span class="sxs-lookup"><span data-stu-id="b649f-176">version</span></span>|<span data-ttu-id="b649f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b649f-177">Int32</span></span>|<span data-ttu-id="b649f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b649f-178">Version of the device configuration.</span></span> <span data-ttu-id="b649f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b649f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b649f-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="b649f-180">connectionName</span></span>|<span data-ttu-id="b649f-181">String</span><span class="sxs-lookup"><span data-stu-id="b649f-181">String</span></span>|<span data-ttu-id="b649f-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b649f-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="b649f-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="b649f-183">connectionType</span></span>|[<span data-ttu-id="b649f-184">Androidforworkvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="b649f-184">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="b649f-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="b649f-185">Connection type.</span></span> <span data-ttu-id="b649f-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="b649f-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="b649f-187">role</span><span class="sxs-lookup"><span data-stu-id="b649f-187">role</span></span>|<span data-ttu-id="b649f-188">String</span><span class="sxs-lookup"><span data-stu-id="b649f-188">String</span></span>|<span data-ttu-id="b649f-189">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="b649f-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b649f-190">область</span><span class="sxs-lookup"><span data-stu-id="b649f-190">realm</span></span>|<span data-ttu-id="b649f-191">String</span><span class="sxs-lookup"><span data-stu-id="b649f-191">String</span></span>|<span data-ttu-id="b649f-192">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="b649f-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b649f-193">серверами</span><span class="sxs-lookup"><span data-stu-id="b649f-193">servers</span></span>|<span data-ttu-id="b649f-194">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="b649f-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b649f-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="b649f-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="b649f-196">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="b649f-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b649f-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b649f-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b649f-198">распознавания</span><span class="sxs-lookup"><span data-stu-id="b649f-198">fingerprint</span></span>|<span data-ttu-id="b649f-199">String</span><span class="sxs-lookup"><span data-stu-id="b649f-199">String</span></span>|<span data-ttu-id="b649f-200">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="b649f-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="b649f-201">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="b649f-201">customData</span></span>|<span data-ttu-id="b649f-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b649f-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b649f-203">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="b649f-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b649f-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="b649f-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b649f-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b649f-205">customKeyValueData</span></span>|<span data-ttu-id="b649f-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b649f-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b649f-207">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="b649f-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b649f-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="b649f-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b649f-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="b649f-209">authenticationMethod</span></span>|[<span data-ttu-id="b649f-210">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b649f-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b649f-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b649f-211">Authentication method.</span></span> <span data-ttu-id="b649f-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b649f-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="b649f-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="b649f-213">Response</span></span>
<span data-ttu-id="b649f-214">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b649f-214">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b649f-215">Пример</span><span class="sxs-lookup"><span data-stu-id="b649f-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="b649f-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="b649f-216">Request</span></span>
<span data-ttu-id="b649f-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b649f-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="b649f-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="b649f-218">Response</span></span>
<span data-ttu-id="b649f-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b649f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



