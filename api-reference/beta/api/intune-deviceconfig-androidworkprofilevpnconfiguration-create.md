---
title: Создание Андроидворкпрофилевпнконфигуратион
description: Создание нового объекта Андроидворкпрофилевпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c69e95e1c9a654d29913817101bce6044e81ae35
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123199"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="e4bfb-103">Создание Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4bfb-103">Create androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="e4bfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4bfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4bfb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4bfb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4bfb-107">Создание нового объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4bfb-107">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4bfb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4bfb-108">Prerequisites</span></span>
<span data-ttu-id="e4bfb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e4bfb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bfb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4bfb-111">Permission type</span></span>|<span data-ttu-id="e4bfb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4bfb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4bfb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4bfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4bfb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bfb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4bfb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4bfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4bfb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-116">Not supported.</span></span>|
|<span data-ttu-id="e4bfb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4bfb-117">Application</span></span>|<span data-ttu-id="e4bfb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bfb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4bfb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4bfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e4bfb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4bfb-120">Request headers</span></span>
|<span data-ttu-id="e4bfb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4bfb-121">Header</span></span>|<span data-ttu-id="e4bfb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4bfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4bfb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4bfb-123">Authorization</span></span>|<span data-ttu-id="e4bfb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4bfb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4bfb-125">Accept</span></span>|<span data-ttu-id="e4bfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4bfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4bfb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4bfb-127">Request body</span></span>
<span data-ttu-id="e4bfb-128">В тексте запроса добавьте представление объекта Андроидворкпрофилевпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-128">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="e4bfb-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилевпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-129">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="e4bfb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4bfb-130">Property</span></span>|<span data-ttu-id="e4bfb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4bfb-131">Type</span></span>|<span data-ttu-id="e4bfb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4bfb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4bfb-133">id</span><span class="sxs-lookup"><span data-stu-id="e4bfb-133">id</span></span>|<span data-ttu-id="e4bfb-134">String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-134">String</span></span>|<span data-ttu-id="e4bfb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-135">Key of the entity.</span></span> <span data-ttu-id="e4bfb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4bfb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e4bfb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4bfb-138">DateTimeOffset</span></span>|<span data-ttu-id="e4bfb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e4bfb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4bfb-141">roleScopeTagIds</span></span>|<span data-ttu-id="e4bfb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-142">String collection</span></span>|<span data-ttu-id="e4bfb-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e4bfb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e4bfb-145">supportsScopeTags</span></span>|<span data-ttu-id="e4bfb-146">Логический</span><span class="sxs-lookup"><span data-stu-id="e4bfb-146">Boolean</span></span>|<span data-ttu-id="e4bfb-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e4bfb-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e4bfb-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e4bfb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-150">This property is read-only.</span></span> <span data-ttu-id="e4bfb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e4bfb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e4bfb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e4bfb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e4bfb-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e4bfb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e4bfb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e4bfb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e4bfb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e4bfb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e4bfb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e4bfb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e4bfb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e4bfb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e4bfb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e4bfb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4bfb-164">createdDateTime</span></span>|<span data-ttu-id="e4bfb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4bfb-165">DateTimeOffset</span></span>|<span data-ttu-id="e4bfb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-166">DateTime the object was created.</span></span> <span data-ttu-id="e4bfb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-168">description</span><span class="sxs-lookup"><span data-stu-id="e4bfb-168">description</span></span>|<span data-ttu-id="e4bfb-169">String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-169">String</span></span>|<span data-ttu-id="e4bfb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4bfb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e4bfb-172">displayName</span></span>|<span data-ttu-id="e4bfb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="e4bfb-173">String</span></span>|<span data-ttu-id="e4bfb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4bfb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-176">version</span><span class="sxs-lookup"><span data-stu-id="e4bfb-176">version</span></span>|<span data-ttu-id="e4bfb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e4bfb-177">Int32</span></span>|<span data-ttu-id="e4bfb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-178">Version of the device configuration.</span></span> <span data-ttu-id="e4bfb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4bfb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4bfb-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="e4bfb-180">connectionName</span></span>|<span data-ttu-id="e4bfb-181">String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-181">String</span></span>|<span data-ttu-id="e4bfb-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="e4bfb-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="e4bfb-183">connectionType</span></span>|[<span data-ttu-id="e4bfb-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="e4bfb-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="e4bfb-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-185">Connection type.</span></span> <span data-ttu-id="e4bfb-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="e4bfb-187">role</span><span class="sxs-lookup"><span data-stu-id="e4bfb-187">role</span></span>|<span data-ttu-id="e4bfb-188">String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-188">String</span></span>|<span data-ttu-id="e4bfb-189">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="e4bfb-190">область</span><span class="sxs-lookup"><span data-stu-id="e4bfb-190">realm</span></span>|<span data-ttu-id="e4bfb-191">String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-191">String</span></span>|<span data-ttu-id="e4bfb-192">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="e4bfb-193">серверами</span><span class="sxs-lookup"><span data-stu-id="e4bfb-193">servers</span></span>|<span data-ttu-id="e4bfb-194">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="e4bfb-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="e4bfb-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="e4bfb-196">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="e4bfb-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e4bfb-198">распознавания</span><span class="sxs-lookup"><span data-stu-id="e4bfb-198">fingerprint</span></span>|<span data-ttu-id="e4bfb-199">String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-199">String</span></span>|<span data-ttu-id="e4bfb-200">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="e4bfb-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="e4bfb-201">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="e4bfb-201">customData</span></span>|<span data-ttu-id="e4bfb-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e4bfb-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e4bfb-203">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="e4bfb-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="e4bfb-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e4bfb-205">customKeyValueData</span></span>|<span data-ttu-id="e4bfb-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e4bfb-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e4bfb-207">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="e4bfb-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="e4bfb-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e4bfb-209">authenticationMethod</span></span>|[<span data-ttu-id="e4bfb-210">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e4bfb-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e4bfb-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-211">Authentication method.</span></span> <span data-ttu-id="e4bfb-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="e4bfb-213">проксисервер</span><span class="sxs-lookup"><span data-stu-id="e4bfb-213">proxyServer</span></span>|[<span data-ttu-id="e4bfb-214">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="e4bfb-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="e4bfb-215">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-215">Proxy server.</span></span>|
|<span data-ttu-id="e4bfb-216">таржетедпаккажеидс</span><span class="sxs-lookup"><span data-stu-id="e4bfb-216">targetedPackageIds</span></span>|<span data-ttu-id="e4bfb-217">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e4bfb-217">String collection</span></span>|<span data-ttu-id="e4bfb-218">Идентификаторы целевых пакетов приложений.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="e4bfb-219">Группа</span><span class="sxs-lookup"><span data-stu-id="e4bfb-219">alwaysOn</span></span>|<span data-ttu-id="e4bfb-220">Логический</span><span class="sxs-lookup"><span data-stu-id="e4bfb-220">Boolean</span></span>|<span data-ttu-id="e4bfb-221">Указывает, следует ли включить постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-221">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="e4bfb-222">алвайсонлоккдовн</span><span class="sxs-lookup"><span data-stu-id="e4bfb-222">alwaysOnLockdown</span></span>|<span data-ttu-id="e4bfb-223">Логический</span><span class="sxs-lookup"><span data-stu-id="e4bfb-223">Boolean</span></span>|<span data-ttu-id="e4bfb-224">Если включено постоянное VPN-подключение, независимо от того, следует ли блокировать сетевой трафик при отключении VPN.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-224">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|



## <a name="response"></a><span data-ttu-id="e4bfb-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4bfb-225">Response</span></span>
<span data-ttu-id="e4bfb-226">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4bfb-227">Пример</span><span class="sxs-lookup"><span data-stu-id="e4bfb-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4bfb-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4bfb-228">Request</span></span>
<span data-ttu-id="e4bfb-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2103

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
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```

### <a name="response"></a><span data-ttu-id="e4bfb-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4bfb-230">Response</span></span>
<span data-ttu-id="e4bfb-231">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-231">Here is an example of the response.</span></span> <span data-ttu-id="e4bfb-232">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-232">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e4bfb-233">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e4bfb-233">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2275

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
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```



