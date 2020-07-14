---
title: Создание Андроидвпнконфигуратион
description: Создание нового объекта Андроидвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd029e83a7b7e0ebe8677774273edb393ccf2cc1
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123269"
---
# <a name="create-androidvpnconfiguration"></a><span data-ttu-id="f23e2-103">Создание Андроидвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f23e2-103">Create androidVpnConfiguration</span></span>

<span data-ttu-id="f23e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f23e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f23e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f23e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f23e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23e2-107">Создание нового объекта [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f23e2-107">Create a new [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f23e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f23e2-108">Prerequisites</span></span>
<span data-ttu-id="f23e2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f23e2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f23e2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23e2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f23e2-111">Permission type</span></span>|<span data-ttu-id="f23e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f23e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f23e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f23e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f23e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f23e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f23e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f23e2-116">Not supported.</span></span>|
|<span data-ttu-id="f23e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f23e2-117">Application</span></span>|<span data-ttu-id="f23e2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23e2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f23e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f23e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f23e2-120">Request headers</span></span>
|<span data-ttu-id="f23e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f23e2-121">Header</span></span>|<span data-ttu-id="f23e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f23e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f23e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f23e2-123">Authorization</span></span>|<span data-ttu-id="f23e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f23e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f23e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f23e2-125">Accept</span></span>|<span data-ttu-id="f23e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f23e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f23e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f23e2-127">Request body</span></span>
<span data-ttu-id="f23e2-128">В тексте запроса добавьте представление объекта Андроидвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f23e2-128">In the request body, supply a JSON representation for the androidVpnConfiguration object.</span></span>

<span data-ttu-id="f23e2-129">В следующей таблице приведены свойства, необходимые при создании Андроидвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f23e2-129">The following table shows the properties that are required when you create the androidVpnConfiguration.</span></span>

|<span data-ttu-id="f23e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f23e2-130">Property</span></span>|<span data-ttu-id="f23e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f23e2-131">Type</span></span>|<span data-ttu-id="f23e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f23e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23e2-133">id</span><span class="sxs-lookup"><span data-stu-id="f23e2-133">id</span></span>|<span data-ttu-id="f23e2-134">String</span><span class="sxs-lookup"><span data-stu-id="f23e2-134">String</span></span>|<span data-ttu-id="f23e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f23e2-135">Key of the entity.</span></span> <span data-ttu-id="f23e2-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f23e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f23e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23e2-138">DateTimeOffset</span></span>|<span data-ttu-id="f23e2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f23e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f23e2-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f23e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="f23e2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f23e2-142">String collection</span></span>|<span data-ttu-id="f23e2-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f23e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f23e2-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f23e2-145">supportsScopeTags</span></span>|<span data-ttu-id="f23e2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f23e2-146">Boolean</span></span>|<span data-ttu-id="f23e2-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f23e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f23e2-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f23e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f23e2-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f23e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f23e2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f23e2-150">This property is read-only.</span></span> <span data-ttu-id="f23e2-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f23e2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f23e2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f23e2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f23e2-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f23e2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f23e2-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f23e2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f23e2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f23e2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f23e2-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f23e2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f23e2-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f23e2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f23e2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f23e2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f23e2-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f23e2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f23e2-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f23e2-164">createdDateTime</span></span>|<span data-ttu-id="f23e2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f23e2-165">DateTimeOffset</span></span>|<span data-ttu-id="f23e2-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f23e2-166">DateTime the object was created.</span></span> <span data-ttu-id="f23e2-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-168">description</span><span class="sxs-lookup"><span data-stu-id="f23e2-168">description</span></span>|<span data-ttu-id="f23e2-169">String</span><span class="sxs-lookup"><span data-stu-id="f23e2-169">String</span></span>|<span data-ttu-id="f23e2-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f23e2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f23e2-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f23e2-172">displayName</span></span>|<span data-ttu-id="f23e2-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f23e2-173">String</span></span>|<span data-ttu-id="f23e2-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f23e2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f23e2-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-176">version</span><span class="sxs-lookup"><span data-stu-id="f23e2-176">version</span></span>|<span data-ttu-id="f23e2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f23e2-177">Int32</span></span>|<span data-ttu-id="f23e2-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f23e2-178">Version of the device configuration.</span></span> <span data-ttu-id="f23e2-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f23e2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f23e2-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="f23e2-180">connectionName</span></span>|<span data-ttu-id="f23e2-181">String</span><span class="sxs-lookup"><span data-stu-id="f23e2-181">String</span></span>|<span data-ttu-id="f23e2-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f23e2-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="f23e2-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="f23e2-183">connectionType</span></span>|[<span data-ttu-id="f23e2-184">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="f23e2-184">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="f23e2-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f23e2-185">Connection type.</span></span> <span data-ttu-id="f23e2-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`.</span><span class="sxs-lookup"><span data-stu-id="f23e2-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="f23e2-187">role</span><span class="sxs-lookup"><span data-stu-id="f23e2-187">role</span></span>|<span data-ttu-id="f23e2-188">String</span><span class="sxs-lookup"><span data-stu-id="f23e2-188">String</span></span>|<span data-ttu-id="f23e2-189">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="f23e2-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="f23e2-190">область</span><span class="sxs-lookup"><span data-stu-id="f23e2-190">realm</span></span>|<span data-ttu-id="f23e2-191">String</span><span class="sxs-lookup"><span data-stu-id="f23e2-191">String</span></span>|<span data-ttu-id="f23e2-192">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="f23e2-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="f23e2-193">серверами</span><span class="sxs-lookup"><span data-stu-id="f23e2-193">servers</span></span>|<span data-ttu-id="f23e2-194">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="f23e2-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f23e2-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="f23e2-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="f23e2-196">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="f23e2-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f23e2-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f23e2-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f23e2-198">распознавания</span><span class="sxs-lookup"><span data-stu-id="f23e2-198">fingerprint</span></span>|<span data-ttu-id="f23e2-199">String</span><span class="sxs-lookup"><span data-stu-id="f23e2-199">String</span></span>|<span data-ttu-id="f23e2-200">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="f23e2-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="f23e2-201">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="f23e2-201">customData</span></span>|<span data-ttu-id="f23e2-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f23e2-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f23e2-203">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="f23e2-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="f23e2-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f23e2-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="f23e2-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f23e2-205">customKeyValueData</span></span>|<span data-ttu-id="f23e2-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f23e2-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f23e2-207">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="f23e2-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="f23e2-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="f23e2-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="f23e2-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f23e2-209">authenticationMethod</span></span>|[<span data-ttu-id="f23e2-210">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f23e2-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f23e2-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f23e2-211">Authentication method.</span></span> <span data-ttu-id="f23e2-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="f23e2-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="f23e2-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="f23e2-213">Response</span></span>
<span data-ttu-id="f23e2-214">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f23e2-214">If successful, this method returns a `201 Created` response code and a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23e2-215">Пример</span><span class="sxs-lookup"><span data-stu-id="f23e2-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="f23e2-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="f23e2-216">Request</span></span>
<span data-ttu-id="f23e2-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f23e2-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f23e2-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="f23e2-218">Response</span></span>
<span data-ttu-id="f23e2-219">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f23e2-219">Here is an example of the response.</span></span> <span data-ttu-id="f23e2-220">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f23e2-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f23e2-221">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f23e2-221">All of the properties will be returned from an actual call.</span></span>
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



