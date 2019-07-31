---
title: Обновление windows81VpnConfiguration
description: Обновление свойств объекта windows81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14e253bc1d78d4c00191a3c19e52aa24ee85fb5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977022"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="788fb-103">Обновление windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="788fb-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="788fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="788fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="788fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="788fb-106">Обновление свойств объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="788fb-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="788fb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="788fb-107">Prerequisites</span></span>
<span data-ttu-id="788fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="788fb-110">Permission type</span></span>|<span data-ttu-id="788fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="788fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="788fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="788fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="788fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="788fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="788fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="788fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="788fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788fb-115">Not supported.</span></span>|
|<span data-ttu-id="788fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="788fb-116">Application</span></span>|<span data-ttu-id="788fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="788fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="788fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="788fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="788fb-119">Request headers</span></span>
|<span data-ttu-id="788fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="788fb-120">Header</span></span>|<span data-ttu-id="788fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="788fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="788fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="788fb-122">Authorization</span></span>|<span data-ttu-id="788fb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="788fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="788fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="788fb-124">Accept</span></span>|<span data-ttu-id="788fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="788fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="788fb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="788fb-126">Request body</span></span>
<span data-ttu-id="788fb-127">В тексте запроса добавьте представление объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="788fb-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="788fb-128">В следующей таблице приведены свойства, необходимые при создании [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="788fb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="788fb-129">Property</span></span>|<span data-ttu-id="788fb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="788fb-130">Type</span></span>|<span data-ttu-id="788fb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="788fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="788fb-132">id</span><span class="sxs-lookup"><span data-stu-id="788fb-132">id</span></span>|<span data-ttu-id="788fb-133">String</span><span class="sxs-lookup"><span data-stu-id="788fb-133">String</span></span>|<span data-ttu-id="788fb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="788fb-134">Key of the entity.</span></span> <span data-ttu-id="788fb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="788fb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="788fb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="788fb-137">DateTimeOffset</span></span>|<span data-ttu-id="788fb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="788fb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="788fb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="788fb-140">roleScopeTagIds</span></span>|<span data-ttu-id="788fb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="788fb-141">String collection</span></span>|<span data-ttu-id="788fb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="788fb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="788fb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="788fb-144">supportsScopeTags</span></span>|<span data-ttu-id="788fb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="788fb-145">Boolean</span></span>|<span data-ttu-id="788fb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="788fb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="788fb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="788fb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="788fb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="788fb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="788fb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="788fb-149">This property is read-only.</span></span> <span data-ttu-id="788fb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="788fb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="788fb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="788fb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="788fb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="788fb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="788fb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="788fb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="788fb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="788fb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="788fb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="788fb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="788fb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="788fb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="788fb-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="788fb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="788fb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="788fb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="788fb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="788fb-163">createdDateTime</span></span>|<span data-ttu-id="788fb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="788fb-164">DateTimeOffset</span></span>|<span data-ttu-id="788fb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="788fb-165">DateTime the object was created.</span></span> <span data-ttu-id="788fb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-167">description</span><span class="sxs-lookup"><span data-stu-id="788fb-167">description</span></span>|<span data-ttu-id="788fb-168">String</span><span class="sxs-lookup"><span data-stu-id="788fb-168">String</span></span>|<span data-ttu-id="788fb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="788fb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="788fb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="788fb-171">displayName</span></span>|<span data-ttu-id="788fb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="788fb-172">String</span></span>|<span data-ttu-id="788fb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="788fb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="788fb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-175">version</span><span class="sxs-lookup"><span data-stu-id="788fb-175">version</span></span>|<span data-ttu-id="788fb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="788fb-176">Int32</span></span>|<span data-ttu-id="788fb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="788fb-177">Version of the device configuration.</span></span> <span data-ttu-id="788fb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="788fb-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-179">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="788fb-179">connectionName</span></span>|<span data-ttu-id="788fb-180">String</span><span class="sxs-lookup"><span data-stu-id="788fb-180">String</span></span>|<span data-ttu-id="788fb-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="788fb-181">Connection name displayed to the user.</span></span> <span data-ttu-id="788fb-182">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="788fb-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-183">серверами</span><span class="sxs-lookup"><span data-stu-id="788fb-183">servers</span></span>|<span data-ttu-id="788fb-184">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="788fb-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="788fb-185">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="788fb-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="788fb-186">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="788fb-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="788fb-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="788fb-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="788fb-188">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="788fb-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-189">customXml</span><span class="sxs-lookup"><span data-stu-id="788fb-189">customXml</span></span>|<span data-ttu-id="788fb-190">Binary</span><span class="sxs-lookup"><span data-stu-id="788fb-190">Binary</span></span>|<span data-ttu-id="788fb-191">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="788fb-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="788fb-192">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="788fb-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="788fb-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="788fb-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="788fb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="788fb-194">Boolean</span></span>|<span data-ttu-id="788fb-195">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="788fb-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="788fb-196">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="788fb-196">This property is read-only.</span></span>|
|<span data-ttu-id="788fb-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="788fb-197">connectionType</span></span>|[<span data-ttu-id="788fb-198">Виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="788fb-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="788fb-199">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="788fb-199">Connection type.</span></span> <span data-ttu-id="788fb-200">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="788fb-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="788fb-201">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="788fb-201">loginGroupOrDomain</span></span>|<span data-ttu-id="788fb-202">String</span><span class="sxs-lookup"><span data-stu-id="788fb-202">String</span></span>|<span data-ttu-id="788fb-203">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="788fb-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="788fb-204">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="788fb-204">enableSplitTunneling</span></span>|<span data-ttu-id="788fb-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="788fb-205">Boolean</span></span>|<span data-ttu-id="788fb-206">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="788fb-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="788fb-207">проксисервер</span><span class="sxs-lookup"><span data-stu-id="788fb-207">proxyServer</span></span>|[<span data-ttu-id="788fb-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="788fb-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="788fb-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="788fb-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="788fb-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="788fb-210">Response</span></span>
<span data-ttu-id="788fb-211">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="788fb-211">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="788fb-212">Пример</span><span class="sxs-lookup"><span data-stu-id="788fb-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="788fb-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="788fb-213">Request</span></span>
<span data-ttu-id="788fb-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788fb-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="788fb-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="788fb-215">Response</span></span>
<span data-ttu-id="788fb-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="788fb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





