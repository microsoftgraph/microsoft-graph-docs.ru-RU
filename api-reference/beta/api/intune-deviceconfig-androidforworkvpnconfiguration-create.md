---
title: Создание androidForWorkVpnConfiguration
description: Создание нового объекта androidForWorkVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 864a12fd53a825ccaf9c0f8f942a505f3bad70cd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534528"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="18a86-103">Создание androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="18a86-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="18a86-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a86-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18a86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a86-106">Создание нового объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="18a86-106">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18a86-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18a86-107">Prerequisites</span></span>
<span data-ttu-id="18a86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18a86-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18a86-110">Permission type</span></span>|<span data-ttu-id="18a86-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18a86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18a86-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18a86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18a86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18a86-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18a86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18a86-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a86-115">Not supported.</span></span>|
|<span data-ttu-id="18a86-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="18a86-116">Application</span></span>|<span data-ttu-id="18a86-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a86-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18a86-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18a86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18a86-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18a86-119">Request headers</span></span>
|<span data-ttu-id="18a86-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18a86-120">Header</span></span>|<span data-ttu-id="18a86-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18a86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18a86-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18a86-122">Authorization</span></span>|<span data-ttu-id="18a86-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18a86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18a86-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18a86-124">Accept</span></span>|<span data-ttu-id="18a86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18a86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18a86-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18a86-126">Request body</span></span>
<span data-ttu-id="18a86-127">В тексте запроса добавьте представление объекта androidForWorkVpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18a86-127">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="18a86-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="18a86-128">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="18a86-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18a86-129">Property</span></span>|<span data-ttu-id="18a86-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18a86-130">Type</span></span>|<span data-ttu-id="18a86-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18a86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a86-132">id</span><span class="sxs-lookup"><span data-stu-id="18a86-132">id</span></span>|<span data-ttu-id="18a86-133">String</span><span class="sxs-lookup"><span data-stu-id="18a86-133">String</span></span>|<span data-ttu-id="18a86-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="18a86-134">Key of the entity.</span></span> <span data-ttu-id="18a86-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a86-136">lastModifiedDateTime</span></span>|<span data-ttu-id="18a86-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a86-137">DateTimeOffset</span></span>|<span data-ttu-id="18a86-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="18a86-138">DateTime the object was last modified.</span></span> <span data-ttu-id="18a86-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18a86-140">roleScopeTagIds</span></span>|<span data-ttu-id="18a86-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18a86-141">String collection</span></span>|<span data-ttu-id="18a86-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="18a86-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18a86-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="18a86-144">supportsScopeTags</span></span>|<span data-ttu-id="18a86-145">Логический</span><span class="sxs-lookup"><span data-stu-id="18a86-145">Boolean</span></span>|<span data-ttu-id="18a86-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="18a86-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18a86-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="18a86-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18a86-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="18a86-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18a86-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18a86-149">This property is read-only.</span></span> <span data-ttu-id="18a86-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18a86-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="18a86-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18a86-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="18a86-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="18a86-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="18a86-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18a86-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="18a86-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18a86-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="18a86-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="18a86-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="18a86-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18a86-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="18a86-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18a86-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="18a86-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="18a86-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="18a86-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18a86-163">createdDateTime</span></span>|<span data-ttu-id="18a86-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a86-164">DateTimeOffset</span></span>|<span data-ttu-id="18a86-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="18a86-165">DateTime the object was created.</span></span> <span data-ttu-id="18a86-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-167">description</span><span class="sxs-lookup"><span data-stu-id="18a86-167">description</span></span>|<span data-ttu-id="18a86-168">String</span><span class="sxs-lookup"><span data-stu-id="18a86-168">String</span></span>|<span data-ttu-id="18a86-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18a86-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18a86-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-171">displayName</span><span class="sxs-lookup"><span data-stu-id="18a86-171">displayName</span></span>|<span data-ttu-id="18a86-172">Строка</span><span class="sxs-lookup"><span data-stu-id="18a86-172">String</span></span>|<span data-ttu-id="18a86-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18a86-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18a86-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-175">version</span><span class="sxs-lookup"><span data-stu-id="18a86-175">version</span></span>|<span data-ttu-id="18a86-176">Int32</span><span class="sxs-lookup"><span data-stu-id="18a86-176">Int32</span></span>|<span data-ttu-id="18a86-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18a86-177">Version of the device configuration.</span></span> <span data-ttu-id="18a86-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a86-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a86-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="18a86-179">connectionName</span></span>|<span data-ttu-id="18a86-180">String</span><span class="sxs-lookup"><span data-stu-id="18a86-180">String</span></span>|<span data-ttu-id="18a86-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="18a86-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="18a86-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="18a86-182">connectionType</span></span>|[<span data-ttu-id="18a86-183">Androidforworkvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="18a86-183">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="18a86-184">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="18a86-184">Connection type.</span></span> <span data-ttu-id="18a86-185">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="18a86-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="18a86-186">role</span><span class="sxs-lookup"><span data-stu-id="18a86-186">role</span></span>|<span data-ttu-id="18a86-187">String</span><span class="sxs-lookup"><span data-stu-id="18a86-187">String</span></span>|<span data-ttu-id="18a86-188">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="18a86-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="18a86-189">область</span><span class="sxs-lookup"><span data-stu-id="18a86-189">realm</span></span>|<span data-ttu-id="18a86-190">String</span><span class="sxs-lookup"><span data-stu-id="18a86-190">String</span></span>|<span data-ttu-id="18a86-191">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="18a86-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="18a86-192">серверами</span><span class="sxs-lookup"><span data-stu-id="18a86-192">servers</span></span>|<span data-ttu-id="18a86-193">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="18a86-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="18a86-194">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="18a86-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="18a86-195">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="18a86-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="18a86-196">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="18a86-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="18a86-197">распознавания</span><span class="sxs-lookup"><span data-stu-id="18a86-197">fingerprint</span></span>|<span data-ttu-id="18a86-198">String</span><span class="sxs-lookup"><span data-stu-id="18a86-198">String</span></span>|<span data-ttu-id="18a86-199">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="18a86-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="18a86-200">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="18a86-200">customData</span></span>|<span data-ttu-id="18a86-201">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="18a86-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="18a86-202">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="18a86-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="18a86-203">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="18a86-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="18a86-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="18a86-204">customKeyValueData</span></span>|<span data-ttu-id="18a86-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="18a86-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="18a86-206">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="18a86-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="18a86-207">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="18a86-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="18a86-208">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="18a86-208">authenticationMethod</span></span>|[<span data-ttu-id="18a86-209">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="18a86-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="18a86-210">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="18a86-210">Authentication method.</span></span> <span data-ttu-id="18a86-211">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="18a86-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="18a86-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="18a86-212">Response</span></span>
<span data-ttu-id="18a86-213">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18a86-213">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a86-214">Пример</span><span class="sxs-lookup"><span data-stu-id="18a86-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="18a86-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="18a86-215">Request</span></span>
<span data-ttu-id="18a86-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18a86-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18a86-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="18a86-217">Response</span></span>
<span data-ttu-id="18a86-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18a86-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






