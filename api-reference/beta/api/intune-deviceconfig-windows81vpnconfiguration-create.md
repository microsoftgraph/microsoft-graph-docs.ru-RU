---
title: Создание windows81VpnConfiguration
description: Создание нового объекта windows81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00dc8f4b8456299ec3f8c012e41a3e83d97e3591
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723506"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="17799-103">Создание windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="17799-103">Create windows81VpnConfiguration</span></span>

<span data-ttu-id="17799-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17799-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17799-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17799-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17799-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17799-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17799-107">Создание нового объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="17799-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17799-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17799-108">Prerequisites</span></span>
<span data-ttu-id="17799-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17799-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17799-111">Permission type</span></span>|<span data-ttu-id="17799-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17799-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17799-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17799-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17799-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17799-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17799-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17799-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17799-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17799-116">Not supported.</span></span>|
|<span data-ttu-id="17799-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17799-117">Application</span></span>|<span data-ttu-id="17799-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17799-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17799-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17799-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="17799-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17799-120">Request headers</span></span>
|<span data-ttu-id="17799-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17799-121">Header</span></span>|<span data-ttu-id="17799-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17799-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17799-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17799-123">Authorization</span></span>|<span data-ttu-id="17799-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17799-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17799-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17799-125">Accept</span></span>|<span data-ttu-id="17799-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17799-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17799-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17799-127">Request body</span></span>
<span data-ttu-id="17799-128">В тексте запроса добавьте представление объекта windows81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17799-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="17799-129">В следующей таблице приведены свойства, необходимые при создании windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="17799-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="17799-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17799-130">Property</span></span>|<span data-ttu-id="17799-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17799-131">Type</span></span>|<span data-ttu-id="17799-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17799-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17799-133">id</span><span class="sxs-lookup"><span data-stu-id="17799-133">id</span></span>|<span data-ttu-id="17799-134">Строка</span><span class="sxs-lookup"><span data-stu-id="17799-134">String</span></span>|<span data-ttu-id="17799-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17799-135">Key of the entity.</span></span> <span data-ttu-id="17799-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17799-137">lastModifiedDateTime</span></span>|<span data-ttu-id="17799-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17799-138">DateTimeOffset</span></span>|<span data-ttu-id="17799-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="17799-139">DateTime the object was last modified.</span></span> <span data-ttu-id="17799-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17799-141">roleScopeTagIds</span></span>|<span data-ttu-id="17799-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="17799-142">String collection</span></span>|<span data-ttu-id="17799-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="17799-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17799-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="17799-145">supportsScopeTags</span></span>|<span data-ttu-id="17799-146">Логический</span><span class="sxs-lookup"><span data-stu-id="17799-146">Boolean</span></span>|<span data-ttu-id="17799-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="17799-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17799-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="17799-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17799-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="17799-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17799-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17799-150">This property is read-only.</span></span> <span data-ttu-id="17799-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17799-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="17799-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17799-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="17799-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="17799-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="17799-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17799-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="17799-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17799-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="17799-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="17799-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="17799-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17799-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="17799-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17799-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="17799-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="17799-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="17799-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17799-164">createdDateTime</span></span>|<span data-ttu-id="17799-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17799-165">DateTimeOffset</span></span>|<span data-ttu-id="17799-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="17799-166">DateTime the object was created.</span></span> <span data-ttu-id="17799-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-168">description</span><span class="sxs-lookup"><span data-stu-id="17799-168">description</span></span>|<span data-ttu-id="17799-169">Строка</span><span class="sxs-lookup"><span data-stu-id="17799-169">String</span></span>|<span data-ttu-id="17799-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17799-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17799-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-172">displayName</span><span class="sxs-lookup"><span data-stu-id="17799-172">displayName</span></span>|<span data-ttu-id="17799-173">Строка</span><span class="sxs-lookup"><span data-stu-id="17799-173">String</span></span>|<span data-ttu-id="17799-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17799-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17799-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-176">version</span><span class="sxs-lookup"><span data-stu-id="17799-176">version</span></span>|<span data-ttu-id="17799-177">Int32</span><span class="sxs-lookup"><span data-stu-id="17799-177">Int32</span></span>|<span data-ttu-id="17799-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17799-178">Version of the device configuration.</span></span> <span data-ttu-id="17799-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17799-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17799-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="17799-180">connectionName</span></span>|<span data-ttu-id="17799-181">Строка</span><span class="sxs-lookup"><span data-stu-id="17799-181">String</span></span>|<span data-ttu-id="17799-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="17799-182">Connection name displayed to the user.</span></span> <span data-ttu-id="17799-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17799-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="17799-184">серверами</span><span class="sxs-lookup"><span data-stu-id="17799-184">servers</span></span>|<span data-ttu-id="17799-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="17799-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="17799-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="17799-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="17799-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="17799-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="17799-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="17799-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="17799-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17799-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="17799-190">customXml</span><span class="sxs-lookup"><span data-stu-id="17799-190">customXml</span></span>|<span data-ttu-id="17799-191">Binary</span><span class="sxs-lookup"><span data-stu-id="17799-191">Binary</span></span>|<span data-ttu-id="17799-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="17799-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="17799-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17799-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="17799-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="17799-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="17799-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="17799-195">Boolean</span></span>|<span data-ttu-id="17799-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="17799-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="17799-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17799-197">This property is read-only.</span></span>|
|<span data-ttu-id="17799-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="17799-198">connectionType</span></span>|[<span data-ttu-id="17799-199">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="17799-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="17799-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="17799-200">Connection type.</span></span> <span data-ttu-id="17799-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="17799-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="17799-202">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="17799-202">loginGroupOrDomain</span></span>|<span data-ttu-id="17799-203">Строка</span><span class="sxs-lookup"><span data-stu-id="17799-203">String</span></span>|<span data-ttu-id="17799-204">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="17799-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="17799-205">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="17799-205">enableSplitTunneling</span></span>|<span data-ttu-id="17799-206">Логический</span><span class="sxs-lookup"><span data-stu-id="17799-206">Boolean</span></span>|<span data-ttu-id="17799-207">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="17799-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="17799-208">проксисервер</span><span class="sxs-lookup"><span data-stu-id="17799-208">proxyServer</span></span>|[<span data-ttu-id="17799-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="17799-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="17799-210">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="17799-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="17799-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="17799-211">Response</span></span>
<span data-ttu-id="17799-212">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17799-212">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17799-213">Пример</span><span class="sxs-lookup"><span data-stu-id="17799-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="17799-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="17799-214">Request</span></span>
<span data-ttu-id="17799-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17799-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17799-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="17799-216">Response</span></span>
<span data-ttu-id="17799-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17799-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





