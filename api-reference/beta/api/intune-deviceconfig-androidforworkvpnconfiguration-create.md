---
title: Создание androidForWorkVpnConfiguration
description: Создайте новый объект AndroidForWorkVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e6061004519c86b25ae8aa3794e5c02f56ff810
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138220"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="12f77-103">Создание androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="12f77-103">Create androidForWorkVpnConfiguration</span></span>

<span data-ttu-id="12f77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12f77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12f77-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12f77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12f77-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12f77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12f77-107">Создайте новый [объект AndroidForWorkVpnConfiguration.](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12f77-107">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12f77-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12f77-108">Prerequisites</span></span>
<span data-ttu-id="12f77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f77-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12f77-111">Permission type</span></span>|<span data-ttu-id="12f77-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12f77-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12f77-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12f77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12f77-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f77-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12f77-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12f77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12f77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12f77-116">Not supported.</span></span>|
|<span data-ttu-id="12f77-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="12f77-117">Application</span></span>|<span data-ttu-id="12f77-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f77-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12f77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12f77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12f77-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12f77-120">Request headers</span></span>
|<span data-ttu-id="12f77-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12f77-121">Header</span></span>|<span data-ttu-id="12f77-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12f77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12f77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f77-123">Authorization</span></span>|<span data-ttu-id="12f77-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12f77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12f77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12f77-125">Accept</span></span>|<span data-ttu-id="12f77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12f77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12f77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12f77-127">Request body</span></span>
<span data-ttu-id="12f77-128">В теле запроса предоставляем представление JSON для объекта AndroidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="12f77-128">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="12f77-129">В следующей таблице показаны свойства, необходимые при создании androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="12f77-129">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="12f77-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12f77-130">Property</span></span>|<span data-ttu-id="12f77-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12f77-131">Type</span></span>|<span data-ttu-id="12f77-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12f77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f77-133">id</span><span class="sxs-lookup"><span data-stu-id="12f77-133">id</span></span>|<span data-ttu-id="12f77-134">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-134">String</span></span>|<span data-ttu-id="12f77-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12f77-135">Key of the entity.</span></span> <span data-ttu-id="12f77-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12f77-137">lastModifiedDateTime</span></span>|<span data-ttu-id="12f77-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f77-138">DateTimeOffset</span></span>|<span data-ttu-id="12f77-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="12f77-139">DateTime the object was last modified.</span></span> <span data-ttu-id="12f77-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12f77-141">roleScopeTagIds</span></span>|<span data-ttu-id="12f77-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="12f77-142">String collection</span></span>|<span data-ttu-id="12f77-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="12f77-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12f77-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="12f77-145">supportsScopeTags</span></span>|<span data-ttu-id="12f77-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="12f77-146">Boolean</span></span>|<span data-ttu-id="12f77-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="12f77-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12f77-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="12f77-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12f77-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="12f77-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12f77-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12f77-150">This property is read-only.</span></span> <span data-ttu-id="12f77-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12f77-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12f77-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12f77-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12f77-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12f77-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12f77-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12f77-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12f77-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12f77-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12f77-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12f77-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12f77-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12f77-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12f77-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12f77-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12f77-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12f77-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12f77-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12f77-164">createdDateTime</span></span>|<span data-ttu-id="12f77-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f77-165">DateTimeOffset</span></span>|<span data-ttu-id="12f77-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="12f77-166">DateTime the object was created.</span></span> <span data-ttu-id="12f77-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-168">description</span><span class="sxs-lookup"><span data-stu-id="12f77-168">description</span></span>|<span data-ttu-id="12f77-169">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-169">String</span></span>|<span data-ttu-id="12f77-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12f77-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12f77-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-172">displayName</span><span class="sxs-lookup"><span data-stu-id="12f77-172">displayName</span></span>|<span data-ttu-id="12f77-173">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-173">String</span></span>|<span data-ttu-id="12f77-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12f77-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12f77-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-176">version</span><span class="sxs-lookup"><span data-stu-id="12f77-176">version</span></span>|<span data-ttu-id="12f77-177">Int32</span><span class="sxs-lookup"><span data-stu-id="12f77-177">Int32</span></span>|<span data-ttu-id="12f77-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12f77-178">Version of the device configuration.</span></span> <span data-ttu-id="12f77-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12f77-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12f77-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="12f77-180">connectionName</span></span>|<span data-ttu-id="12f77-181">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-181">String</span></span>|<span data-ttu-id="12f77-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="12f77-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="12f77-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="12f77-183">connectionType</span></span>|[<span data-ttu-id="12f77-184">AndroidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="12f77-184">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="12f77-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="12f77-185">Connection type.</span></span> <span data-ttu-id="12f77-186">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="12f77-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="12f77-187">role</span><span class="sxs-lookup"><span data-stu-id="12f77-187">role</span></span>|<span data-ttu-id="12f77-188">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-188">String</span></span>|<span data-ttu-id="12f77-189">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="12f77-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="12f77-190">realm</span><span class="sxs-lookup"><span data-stu-id="12f77-190">realm</span></span>|<span data-ttu-id="12f77-191">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-191">String</span></span>|<span data-ttu-id="12f77-192">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="12f77-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="12f77-193">серверы</span><span class="sxs-lookup"><span data-stu-id="12f77-193">servers</span></span>|<span data-ttu-id="12f77-194">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="12f77-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="12f77-195">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="12f77-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="12f77-196">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="12f77-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="12f77-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="12f77-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="12f77-198">отпечаток пальца</span><span class="sxs-lookup"><span data-stu-id="12f77-198">fingerprint</span></span>|<span data-ttu-id="12f77-199">Строка</span><span class="sxs-lookup"><span data-stu-id="12f77-199">String</span></span>|<span data-ttu-id="12f77-200">Отпечатки пальцев — это строка, которая будет использоваться для проверки доверия к VPN-серверу, которая применяется только в том случае, если тип подключения — VPN Check Point Capsule.</span><span class="sxs-lookup"><span data-stu-id="12f77-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="12f77-201">customData</span><span class="sxs-lookup"><span data-stu-id="12f77-201">customData</span></span>|<span data-ttu-id="12f77-202">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="12f77-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="12f77-203">Настраиваемые данные при наборе типа подключения к Citrix.</span><span class="sxs-lookup"><span data-stu-id="12f77-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="12f77-204">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="12f77-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="12f77-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="12f77-205">customKeyValueData</span></span>|<span data-ttu-id="12f77-206">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="12f77-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="12f77-207">Настраиваемые данные при наборе типа подключения к Citrix.</span><span class="sxs-lookup"><span data-stu-id="12f77-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="12f77-208">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="12f77-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="12f77-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="12f77-209">authenticationMethod</span></span>|[<span data-ttu-id="12f77-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="12f77-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="12f77-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="12f77-211">Authentication method.</span></span> <span data-ttu-id="12f77-212">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="12f77-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="12f77-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="12f77-213">Response</span></span>
<span data-ttu-id="12f77-214">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12f77-214">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f77-215">Пример</span><span class="sxs-lookup"><span data-stu-id="12f77-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="12f77-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="12f77-216">Request</span></span>
<span data-ttu-id="12f77-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12f77-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12f77-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="12f77-218">Response</span></span>
<span data-ttu-id="12f77-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12f77-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




