---
title: Создание windows81VpnConfiguration
description: Создание нового объекта windows81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 849f59a462849420758b343fe5043bc46a5c18ff
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186997"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="faeff-103">Создание windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faeff-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="faeff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faeff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faeff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faeff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faeff-106">Создание нового объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="faeff-106">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faeff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="faeff-107">Prerequisites</span></span>
<span data-ttu-id="faeff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faeff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faeff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faeff-110">Permission type</span></span>|<span data-ttu-id="faeff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="faeff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faeff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faeff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faeff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faeff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faeff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faeff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faeff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faeff-115">Not supported.</span></span>|
|<span data-ttu-id="faeff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faeff-116">Application</span></span>|<span data-ttu-id="faeff-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faeff-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="faeff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faeff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="faeff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faeff-119">Request headers</span></span>
|<span data-ttu-id="faeff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faeff-120">Header</span></span>|<span data-ttu-id="faeff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="faeff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faeff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faeff-122">Authorization</span></span>|<span data-ttu-id="faeff-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faeff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faeff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="faeff-124">Accept</span></span>|<span data-ttu-id="faeff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faeff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faeff-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="faeff-126">Request body</span></span>
<span data-ttu-id="faeff-127">В тексте запроса добавьте представление объекта windows81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="faeff-127">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="faeff-128">В следующей таблице приведены свойства, необходимые при создании windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="faeff-128">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="faeff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="faeff-129">Property</span></span>|<span data-ttu-id="faeff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="faeff-130">Type</span></span>|<span data-ttu-id="faeff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="faeff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faeff-132">id</span><span class="sxs-lookup"><span data-stu-id="faeff-132">id</span></span>|<span data-ttu-id="faeff-133">String</span><span class="sxs-lookup"><span data-stu-id="faeff-133">String</span></span>|<span data-ttu-id="faeff-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="faeff-134">Key of the entity.</span></span> <span data-ttu-id="faeff-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faeff-136">lastModifiedDateTime</span></span>|<span data-ttu-id="faeff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faeff-137">DateTimeOffset</span></span>|<span data-ttu-id="faeff-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="faeff-138">DateTime the object was last modified.</span></span> <span data-ttu-id="faeff-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="faeff-140">roleScopeTagIds</span></span>|<span data-ttu-id="faeff-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="faeff-141">String collection</span></span>|<span data-ttu-id="faeff-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="faeff-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="faeff-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="faeff-144">supportsScopeTags</span></span>|<span data-ttu-id="faeff-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="faeff-145">Boolean</span></span>|<span data-ttu-id="faeff-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="faeff-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="faeff-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="faeff-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="faeff-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="faeff-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="faeff-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeff-149">This property is read-only.</span></span> <span data-ttu-id="faeff-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="faeff-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="faeff-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="faeff-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="faeff-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="faeff-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="faeff-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="faeff-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="faeff-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="faeff-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="faeff-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="faeff-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="faeff-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="faeff-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="faeff-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="faeff-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="faeff-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="faeff-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="faeff-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faeff-163">createdDateTime</span></span>|<span data-ttu-id="faeff-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faeff-164">DateTimeOffset</span></span>|<span data-ttu-id="faeff-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="faeff-165">DateTime the object was created.</span></span> <span data-ttu-id="faeff-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-167">description</span><span class="sxs-lookup"><span data-stu-id="faeff-167">description</span></span>|<span data-ttu-id="faeff-168">String</span><span class="sxs-lookup"><span data-stu-id="faeff-168">String</span></span>|<span data-ttu-id="faeff-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="faeff-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="faeff-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-171">displayName</span><span class="sxs-lookup"><span data-stu-id="faeff-171">displayName</span></span>|<span data-ttu-id="faeff-172">Строка</span><span class="sxs-lookup"><span data-stu-id="faeff-172">String</span></span>|<span data-ttu-id="faeff-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="faeff-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="faeff-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-175">version</span><span class="sxs-lookup"><span data-stu-id="faeff-175">version</span></span>|<span data-ttu-id="faeff-176">Int32</span><span class="sxs-lookup"><span data-stu-id="faeff-176">Int32</span></span>|<span data-ttu-id="faeff-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="faeff-177">Version of the device configuration.</span></span> <span data-ttu-id="faeff-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faeff-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="faeff-179">connectionName</span></span>|<span data-ttu-id="faeff-180">String.</span><span class="sxs-lookup"><span data-stu-id="faeff-180">String</span></span>|<span data-ttu-id="faeff-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="faeff-181">Connection name displayed to the user.</span></span> <span data-ttu-id="faeff-182">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faeff-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-183">серверами</span><span class="sxs-lookup"><span data-stu-id="faeff-183">servers</span></span>|<span data-ttu-id="faeff-184">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="faeff-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="faeff-185">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="faeff-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="faeff-186">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="faeff-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="faeff-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="faeff-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="faeff-188">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faeff-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-189">customXml</span><span class="sxs-lookup"><span data-stu-id="faeff-189">customXml</span></span>|<span data-ttu-id="faeff-190">Binary</span><span class="sxs-lookup"><span data-stu-id="faeff-190">Binary</span></span>|<span data-ttu-id="faeff-191">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="faeff-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="faeff-192">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faeff-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="faeff-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="faeff-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="faeff-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="faeff-194">Boolean</span></span>|<span data-ttu-id="faeff-195">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="faeff-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="faeff-196">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faeff-196">This property is read-only.</span></span>|
|<span data-ttu-id="faeff-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="faeff-197">connectionType</span></span>|[<span data-ttu-id="faeff-198">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="faeff-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="faeff-199">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="faeff-199">Connection type.</span></span> <span data-ttu-id="faeff-200">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="faeff-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="faeff-201">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="faeff-201">loginGroupOrDomain</span></span>|<span data-ttu-id="faeff-202">String.</span><span class="sxs-lookup"><span data-stu-id="faeff-202">String</span></span>|<span data-ttu-id="faeff-203">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="faeff-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="faeff-204">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="faeff-204">enableSplitTunneling</span></span>|<span data-ttu-id="faeff-205">Boolean.</span><span class="sxs-lookup"><span data-stu-id="faeff-205">Boolean</span></span>|<span data-ttu-id="faeff-206">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="faeff-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="faeff-207">проксисервер</span><span class="sxs-lookup"><span data-stu-id="faeff-207">proxyServer</span></span>|[<span data-ttu-id="faeff-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="faeff-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="faeff-209">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="faeff-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="faeff-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="faeff-210">Response</span></span>
<span data-ttu-id="faeff-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="faeff-211">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faeff-212">Пример</span><span class="sxs-lookup"><span data-stu-id="faeff-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="faeff-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="faeff-213">Request</span></span>
<span data-ttu-id="faeff-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="faeff-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="faeff-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="faeff-215">Response</span></span>
<span data-ttu-id="faeff-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="faeff-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




