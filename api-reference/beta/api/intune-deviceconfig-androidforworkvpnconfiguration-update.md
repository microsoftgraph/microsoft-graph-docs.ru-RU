---
title: Обновление androidForWorkVpnConfiguration
description: Обновление свойств объекта AndroidForWorkVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e7531c4934c92d885f66c575491e1e2030def37f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138150"
---
# <a name="update-androidforworkvpnconfiguration"></a><span data-ttu-id="3e7ec-103">Обновление androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e7ec-103">Update androidForWorkVpnConfiguration</span></span>

<span data-ttu-id="3e7ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e7ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e7ec-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e7ec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e7ec-107">Обновление свойств объекта [AndroidForWorkVpnConfiguration.](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-107">Update the properties of a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e7ec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e7ec-108">Prerequisites</span></span>
<span data-ttu-id="3e7ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e7ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7ec-111">Permission type</span></span>|<span data-ttu-id="3e7ec-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e7ec-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e7ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e7ec-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e7ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-116">Not supported.</span></span>|
|<span data-ttu-id="3e7ec-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e7ec-117">Application</span></span>|<span data-ttu-id="3e7ec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7ec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e7ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e7ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3e7ec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e7ec-120">Request headers</span></span>
|<span data-ttu-id="3e7ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e7ec-121">Header</span></span>|<span data-ttu-id="3e7ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e7ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e7ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e7ec-123">Authorization</span></span>|<span data-ttu-id="3e7ec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e7ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e7ec-125">Accept</span></span>|<span data-ttu-id="3e7ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e7ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e7ec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e7ec-127">Request body</span></span>
<span data-ttu-id="3e7ec-128">В теле запроса предоставляем представление JSON для [объекта AndroidForWorkVpnConfiguration.](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-128">In the request body, supply a JSON representation for the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

<span data-ttu-id="3e7ec-129">В следующей таблице показаны свойства, необходимые при создании [androidForWorkVpnConfiguration.](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-129">The following table shows the properties that are required when you create the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span></span>

|<span data-ttu-id="3e7ec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e7ec-130">Property</span></span>|<span data-ttu-id="3e7ec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7ec-131">Type</span></span>|<span data-ttu-id="3e7ec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e7ec-133">id</span><span class="sxs-lookup"><span data-stu-id="3e7ec-133">id</span></span>|<span data-ttu-id="3e7ec-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-134">String</span></span>|<span data-ttu-id="3e7ec-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-135">Key of the entity.</span></span> <span data-ttu-id="3e7ec-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7ec-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3e7ec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7ec-138">DateTimeOffset</span></span>|<span data-ttu-id="3e7ec-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3e7ec-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e7ec-141">roleScopeTagIds</span></span>|<span data-ttu-id="3e7ec-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e7ec-142">String collection</span></span>|<span data-ttu-id="3e7ec-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3e7ec-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3e7ec-145">supportsScopeTags</span></span>|<span data-ttu-id="3e7ec-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e7ec-146">Boolean</span></span>|<span data-ttu-id="3e7ec-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3e7ec-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3e7ec-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3e7ec-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-150">This property is read-only.</span></span> <span data-ttu-id="3e7ec-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3e7ec-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3e7ec-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3e7ec-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3e7ec-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3e7ec-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3e7ec-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3e7ec-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3e7ec-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3e7ec-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3e7ec-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3e7ec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3e7ec-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3e7ec-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3e7ec-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3e7ec-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7ec-164">createdDateTime</span></span>|<span data-ttu-id="3e7ec-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7ec-165">DateTimeOffset</span></span>|<span data-ttu-id="3e7ec-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-166">DateTime the object was created.</span></span> <span data-ttu-id="3e7ec-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-168">description</span><span class="sxs-lookup"><span data-stu-id="3e7ec-168">description</span></span>|<span data-ttu-id="3e7ec-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-169">String</span></span>|<span data-ttu-id="3e7ec-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e7ec-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3e7ec-172">displayName</span></span>|<span data-ttu-id="3e7ec-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-173">String</span></span>|<span data-ttu-id="3e7ec-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e7ec-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-176">version</span><span class="sxs-lookup"><span data-stu-id="3e7ec-176">version</span></span>|<span data-ttu-id="3e7ec-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7ec-177">Int32</span></span>|<span data-ttu-id="3e7ec-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-178">Version of the device configuration.</span></span> <span data-ttu-id="3e7ec-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e7ec-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e7ec-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="3e7ec-180">connectionName</span></span>|<span data-ttu-id="3e7ec-181">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-181">String</span></span>|<span data-ttu-id="3e7ec-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="3e7ec-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="3e7ec-183">connectionType</span></span>|[<span data-ttu-id="3e7ec-184">AndroidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3e7ec-184">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="3e7ec-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-185">Connection type.</span></span> <span data-ttu-id="3e7ec-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="3e7ec-187">role</span><span class="sxs-lookup"><span data-stu-id="3e7ec-187">role</span></span>|<span data-ttu-id="3e7ec-188">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-188">String</span></span>|<span data-ttu-id="3e7ec-189">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="3e7ec-190">realm</span><span class="sxs-lookup"><span data-stu-id="3e7ec-190">realm</span></span>|<span data-ttu-id="3e7ec-191">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-191">String</span></span>|<span data-ttu-id="3e7ec-192">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="3e7ec-193">серверы</span><span class="sxs-lookup"><span data-stu-id="3e7ec-193">servers</span></span>|<span data-ttu-id="3e7ec-194">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3e7ec-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="3e7ec-196">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3e7ec-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3e7ec-198">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="3e7ec-198">fingerprint</span></span>|<span data-ttu-id="3e7ec-199">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7ec-199">String</span></span>|<span data-ttu-id="3e7ec-200">Отпечатки пальцев — это строка, которая будет использоваться для проверки доверия к VPN-серверу, которая применяется только в том случае, если тип подключения — VPN Check Point Capsule.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="3e7ec-201">customData</span><span class="sxs-lookup"><span data-stu-id="3e7ec-201">customData</span></span>|<span data-ttu-id="3e7ec-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="3e7ec-203">Настраиваемые данные при наборе типа подключения к Citrix.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="3e7ec-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="3e7ec-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="3e7ec-205">customKeyValueData</span></span>|<span data-ttu-id="3e7ec-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3e7ec-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3e7ec-207">Настраиваемые данные при наборе типа подключения к Citrix.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="3e7ec-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="3e7ec-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3e7ec-209">authenticationMethod</span></span>|[<span data-ttu-id="3e7ec-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3e7ec-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3e7ec-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-211">Authentication method.</span></span> <span data-ttu-id="3e7ec-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="3e7ec-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7ec-213">Response</span></span>
<span data-ttu-id="3e7ec-214">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-214">If successful, this method returns a `200 OK` response code and an updated [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e7ec-215">Пример</span><span class="sxs-lookup"><span data-stu-id="3e7ec-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e7ec-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e7ec-216">Request</span></span>
<span data-ttu-id="3e7ec-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e7ec-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7ec-218">Response</span></span>
<span data-ttu-id="3e7ec-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e7ec-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




