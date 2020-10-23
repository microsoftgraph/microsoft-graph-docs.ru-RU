---
title: Обновление windows81VpnConfiguration
description: Обновление свойств объекта windows81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: affb0642a71c2eac8546964f5fc0e97af6d9e2d1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723478"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="a9d15-103">Обновление windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9d15-103">Update windows81VpnConfiguration</span></span>

<span data-ttu-id="a9d15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9d15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9d15-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9d15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9d15-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9d15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9d15-107">Обновление свойств объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a9d15-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9d15-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9d15-108">Prerequisites</span></span>
<span data-ttu-id="a9d15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9d15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9d15-111">Permission type</span></span>|<span data-ttu-id="a9d15-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9d15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9d15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9d15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9d15-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9d15-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9d15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9d15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9d15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9d15-116">Not supported.</span></span>|
|<span data-ttu-id="a9d15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9d15-117">Application</span></span>|<span data-ttu-id="a9d15-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9d15-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9d15-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9d15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a9d15-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9d15-120">Request headers</span></span>
|<span data-ttu-id="a9d15-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9d15-121">Header</span></span>|<span data-ttu-id="a9d15-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9d15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9d15-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9d15-123">Authorization</span></span>|<span data-ttu-id="a9d15-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9d15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9d15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9d15-125">Accept</span></span>|<span data-ttu-id="a9d15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9d15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9d15-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9d15-127">Request body</span></span>
<span data-ttu-id="a9d15-128">В тексте запроса добавьте представление объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d15-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="a9d15-129">В следующей таблице приведены свойства, необходимые при создании [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="a9d15-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9d15-130">Property</span></span>|<span data-ttu-id="a9d15-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9d15-131">Type</span></span>|<span data-ttu-id="a9d15-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9d15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9d15-133">id</span><span class="sxs-lookup"><span data-stu-id="a9d15-133">id</span></span>|<span data-ttu-id="a9d15-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d15-134">String</span></span>|<span data-ttu-id="a9d15-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9d15-135">Key of the entity.</span></span> <span data-ttu-id="a9d15-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d15-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a9d15-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d15-138">DateTimeOffset</span></span>|<span data-ttu-id="a9d15-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a9d15-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a9d15-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9d15-141">roleScopeTagIds</span></span>|<span data-ttu-id="a9d15-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a9d15-142">String collection</span></span>|<span data-ttu-id="a9d15-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a9d15-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9d15-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a9d15-145">supportsScopeTags</span></span>|<span data-ttu-id="a9d15-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d15-146">Boolean</span></span>|<span data-ttu-id="a9d15-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a9d15-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9d15-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a9d15-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9d15-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a9d15-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9d15-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9d15-150">This property is read-only.</span></span> <span data-ttu-id="a9d15-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a9d15-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a9d15-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a9d15-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a9d15-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a9d15-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a9d15-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a9d15-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a9d15-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a9d15-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a9d15-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a9d15-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a9d15-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a9d15-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a9d15-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a9d15-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a9d15-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a9d15-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a9d15-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d15-164">createdDateTime</span></span>|<span data-ttu-id="a9d15-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d15-165">DateTimeOffset</span></span>|<span data-ttu-id="a9d15-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a9d15-166">DateTime the object was created.</span></span> <span data-ttu-id="a9d15-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-168">description</span><span class="sxs-lookup"><span data-stu-id="a9d15-168">description</span></span>|<span data-ttu-id="a9d15-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d15-169">String</span></span>|<span data-ttu-id="a9d15-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9d15-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9d15-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a9d15-172">displayName</span></span>|<span data-ttu-id="a9d15-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d15-173">String</span></span>|<span data-ttu-id="a9d15-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9d15-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9d15-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-176">version</span><span class="sxs-lookup"><span data-stu-id="a9d15-176">version</span></span>|<span data-ttu-id="a9d15-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a9d15-177">Int32</span></span>|<span data-ttu-id="a9d15-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9d15-178">Version of the device configuration.</span></span> <span data-ttu-id="a9d15-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9d15-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="a9d15-180">connectionName</span></span>|<span data-ttu-id="a9d15-181">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d15-181">String</span></span>|<span data-ttu-id="a9d15-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a9d15-182">Connection name displayed to the user.</span></span> <span data-ttu-id="a9d15-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9d15-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-184">серверами</span><span class="sxs-lookup"><span data-stu-id="a9d15-184">servers</span></span>|<span data-ttu-id="a9d15-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="a9d15-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="a9d15-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="a9d15-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="a9d15-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="a9d15-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="a9d15-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a9d15-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a9d15-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9d15-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-190">customXml</span><span class="sxs-lookup"><span data-stu-id="a9d15-190">customXml</span></span>|<span data-ttu-id="a9d15-191">Binary</span><span class="sxs-lookup"><span data-stu-id="a9d15-191">Binary</span></span>|<span data-ttu-id="a9d15-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="a9d15-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="a9d15-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9d15-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a9d15-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="a9d15-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="a9d15-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d15-195">Boolean</span></span>|<span data-ttu-id="a9d15-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="a9d15-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="a9d15-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9d15-197">This property is read-only.</span></span>|
|<span data-ttu-id="a9d15-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="a9d15-198">connectionType</span></span>|[<span data-ttu-id="a9d15-199">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="a9d15-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="a9d15-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="a9d15-200">Connection type.</span></span> <span data-ttu-id="a9d15-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="a9d15-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="a9d15-202">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="a9d15-202">loginGroupOrDomain</span></span>|<span data-ttu-id="a9d15-203">Строка</span><span class="sxs-lookup"><span data-stu-id="a9d15-203">String</span></span>|<span data-ttu-id="a9d15-204">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="a9d15-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a9d15-205">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="a9d15-205">enableSplitTunneling</span></span>|<span data-ttu-id="a9d15-206">Логический</span><span class="sxs-lookup"><span data-stu-id="a9d15-206">Boolean</span></span>|<span data-ttu-id="a9d15-207">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="a9d15-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="a9d15-208">проксисервер</span><span class="sxs-lookup"><span data-stu-id="a9d15-208">proxyServer</span></span>|[<span data-ttu-id="a9d15-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a9d15-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="a9d15-210">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="a9d15-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="a9d15-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9d15-211">Response</span></span>
<span data-ttu-id="a9d15-212">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9d15-212">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9d15-213">Пример</span><span class="sxs-lookup"><span data-stu-id="a9d15-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9d15-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9d15-214">Request</span></span>
<span data-ttu-id="a9d15-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9d15-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="a9d15-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9d15-216">Response</span></span>
<span data-ttu-id="a9d15-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9d15-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```





