---
title: Создание windows81VpnConfiguration
description: Создание нового объекта windows81VpnConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9d8d848b1861aa34365fe8b440442558193ebd0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42736533"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="90f16-103">Создание windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="90f16-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="90f16-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90f16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90f16-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90f16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90f16-106">Создание нового объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="90f16-106">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90f16-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90f16-107">Prerequisites</span></span>
<span data-ttu-id="90f16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90f16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90f16-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90f16-110">Permission type</span></span>|<span data-ttu-id="90f16-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90f16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90f16-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90f16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90f16-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f16-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90f16-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90f16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90f16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90f16-115">Not supported.</span></span>|
|<span data-ttu-id="90f16-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="90f16-116">Application</span></span>|<span data-ttu-id="90f16-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90f16-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90f16-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90f16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90f16-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90f16-119">Request headers</span></span>
|<span data-ttu-id="90f16-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90f16-120">Header</span></span>|<span data-ttu-id="90f16-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90f16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90f16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90f16-122">Authorization</span></span>|<span data-ttu-id="90f16-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90f16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90f16-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90f16-124">Accept</span></span>|<span data-ttu-id="90f16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90f16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90f16-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90f16-126">Request body</span></span>
<span data-ttu-id="90f16-127">В тексте запроса добавьте представление объекта windows81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90f16-127">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="90f16-128">В следующей таблице приведены свойства, необходимые при создании windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="90f16-128">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="90f16-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="90f16-129">Property</span></span>|<span data-ttu-id="90f16-130">Тип</span><span class="sxs-lookup"><span data-stu-id="90f16-130">Type</span></span>|<span data-ttu-id="90f16-131">Описание</span><span class="sxs-lookup"><span data-stu-id="90f16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90f16-132">id</span><span class="sxs-lookup"><span data-stu-id="90f16-132">id</span></span>|<span data-ttu-id="90f16-133">String</span><span class="sxs-lookup"><span data-stu-id="90f16-133">String</span></span>|<span data-ttu-id="90f16-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90f16-134">Key of the entity.</span></span> <span data-ttu-id="90f16-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90f16-136">lastModifiedDateTime</span></span>|<span data-ttu-id="90f16-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90f16-137">DateTimeOffset</span></span>|<span data-ttu-id="90f16-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="90f16-138">DateTime the object was last modified.</span></span> <span data-ttu-id="90f16-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90f16-140">roleScopeTagIds</span></span>|<span data-ttu-id="90f16-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90f16-141">String collection</span></span>|<span data-ttu-id="90f16-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="90f16-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="90f16-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="90f16-144">supportsScopeTags</span></span>|<span data-ttu-id="90f16-145">Логический</span><span class="sxs-lookup"><span data-stu-id="90f16-145">Boolean</span></span>|<span data-ttu-id="90f16-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="90f16-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="90f16-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="90f16-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="90f16-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="90f16-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="90f16-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90f16-149">This property is read-only.</span></span> <span data-ttu-id="90f16-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90f16-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="90f16-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90f16-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="90f16-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="90f16-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="90f16-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90f16-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="90f16-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90f16-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="90f16-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="90f16-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="90f16-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90f16-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="90f16-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90f16-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="90f16-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="90f16-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="90f16-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90f16-163">createdDateTime</span></span>|<span data-ttu-id="90f16-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90f16-164">DateTimeOffset</span></span>|<span data-ttu-id="90f16-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="90f16-165">DateTime the object was created.</span></span> <span data-ttu-id="90f16-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-167">description</span><span class="sxs-lookup"><span data-stu-id="90f16-167">description</span></span>|<span data-ttu-id="90f16-168">String</span><span class="sxs-lookup"><span data-stu-id="90f16-168">String</span></span>|<span data-ttu-id="90f16-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90f16-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90f16-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-171">displayName</span><span class="sxs-lookup"><span data-stu-id="90f16-171">displayName</span></span>|<span data-ttu-id="90f16-172">Строка</span><span class="sxs-lookup"><span data-stu-id="90f16-172">String</span></span>|<span data-ttu-id="90f16-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90f16-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90f16-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-175">version</span><span class="sxs-lookup"><span data-stu-id="90f16-175">version</span></span>|<span data-ttu-id="90f16-176">Int32</span><span class="sxs-lookup"><span data-stu-id="90f16-176">Int32</span></span>|<span data-ttu-id="90f16-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90f16-177">Version of the device configuration.</span></span> <span data-ttu-id="90f16-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90f16-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="90f16-179">connectionName</span></span>|<span data-ttu-id="90f16-180">String</span><span class="sxs-lookup"><span data-stu-id="90f16-180">String</span></span>|<span data-ttu-id="90f16-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="90f16-181">Connection name displayed to the user.</span></span> <span data-ttu-id="90f16-182">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90f16-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-183">серверами</span><span class="sxs-lookup"><span data-stu-id="90f16-183">servers</span></span>|<span data-ttu-id="90f16-184">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="90f16-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="90f16-185">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="90f16-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="90f16-186">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="90f16-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="90f16-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="90f16-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="90f16-188">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90f16-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-189">customXml</span><span class="sxs-lookup"><span data-stu-id="90f16-189">customXml</span></span>|<span data-ttu-id="90f16-190">Binary</span><span class="sxs-lookup"><span data-stu-id="90f16-190">Binary</span></span>|<span data-ttu-id="90f16-191">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="90f16-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="90f16-192">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90f16-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="90f16-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="90f16-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="90f16-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="90f16-194">Boolean</span></span>|<span data-ttu-id="90f16-195">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="90f16-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="90f16-196">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90f16-196">This property is read-only.</span></span>|
|<span data-ttu-id="90f16-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="90f16-197">connectionType</span></span>|[<span data-ttu-id="90f16-198">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="90f16-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="90f16-199">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="90f16-199">Connection type.</span></span> <span data-ttu-id="90f16-200">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="90f16-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="90f16-201">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="90f16-201">loginGroupOrDomain</span></span>|<span data-ttu-id="90f16-202">String</span><span class="sxs-lookup"><span data-stu-id="90f16-202">String</span></span>|<span data-ttu-id="90f16-203">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="90f16-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="90f16-204">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="90f16-204">enableSplitTunneling</span></span>|<span data-ttu-id="90f16-205">Логический</span><span class="sxs-lookup"><span data-stu-id="90f16-205">Boolean</span></span>|<span data-ttu-id="90f16-206">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="90f16-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="90f16-207">проксисервер</span><span class="sxs-lookup"><span data-stu-id="90f16-207">proxyServer</span></span>|[<span data-ttu-id="90f16-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="90f16-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="90f16-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="90f16-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="90f16-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="90f16-210">Response</span></span>
<span data-ttu-id="90f16-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90f16-211">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90f16-212">Пример</span><span class="sxs-lookup"><span data-stu-id="90f16-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="90f16-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="90f16-213">Request</span></span>
<span data-ttu-id="90f16-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90f16-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="90f16-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="90f16-215">Response</span></span>
<span data-ttu-id="90f16-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90f16-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




