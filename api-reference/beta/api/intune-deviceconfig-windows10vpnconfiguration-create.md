---
title: Создание windows10VpnConfiguration
description: Создание нового объекта windows10VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bdc0ae8261061fac4fd0e63dfb3bb2a4f3901f85
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314296"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="8577f-103">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8577f-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="8577f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8577f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8577f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8577f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8577f-106">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8577f-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8577f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8577f-107">Prerequisites</span></span>
<span data-ttu-id="8577f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8577f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8577f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8577f-110">Permission type</span></span>|<span data-ttu-id="8577f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8577f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8577f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8577f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8577f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8577f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8577f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8577f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8577f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8577f-115">Not supported.</span></span>|
|<span data-ttu-id="8577f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8577f-116">Application</span></span>|<span data-ttu-id="8577f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8577f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8577f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8577f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8577f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8577f-119">Request headers</span></span>
|<span data-ttu-id="8577f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8577f-120">Header</span></span>|<span data-ttu-id="8577f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8577f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8577f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8577f-122">Authorization</span></span>|<span data-ttu-id="8577f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8577f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8577f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8577f-124">Accept</span></span>|<span data-ttu-id="8577f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8577f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8577f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8577f-126">Request body</span></span>
<span data-ttu-id="8577f-127">В тексте запроса добавьте представление объекта windows10VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8577f-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="8577f-128">В следующей таблице приведены свойства, необходимые при создании windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8577f-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="8577f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8577f-129">Property</span></span>|<span data-ttu-id="8577f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8577f-130">Type</span></span>|<span data-ttu-id="8577f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8577f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8577f-132">id</span><span class="sxs-lookup"><span data-stu-id="8577f-132">id</span></span>|<span data-ttu-id="8577f-133">String</span><span class="sxs-lookup"><span data-stu-id="8577f-133">String</span></span>|<span data-ttu-id="8577f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8577f-134">Key of the entity.</span></span> <span data-ttu-id="8577f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8577f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8577f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8577f-137">DateTimeOffset</span></span>|<span data-ttu-id="8577f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8577f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8577f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8577f-140">roleScopeTagIds</span></span>|<span data-ttu-id="8577f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8577f-141">String collection</span></span>|<span data-ttu-id="8577f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8577f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8577f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8577f-144">supportsScopeTags</span></span>|<span data-ttu-id="8577f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-145">Boolean</span></span>|<span data-ttu-id="8577f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8577f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8577f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8577f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8577f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8577f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8577f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8577f-149">This property is read-only.</span></span> <span data-ttu-id="8577f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8577f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8577f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8577f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8577f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8577f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8577f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8577f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8577f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8577f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8577f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8577f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8577f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="8577f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8577f-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="8577f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8577f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8577f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8577f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8577f-163">createdDateTime</span></span>|<span data-ttu-id="8577f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8577f-164">DateTimeOffset</span></span>|<span data-ttu-id="8577f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8577f-165">DateTime the object was created.</span></span> <span data-ttu-id="8577f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-167">description</span><span class="sxs-lookup"><span data-stu-id="8577f-167">description</span></span>|<span data-ttu-id="8577f-168">String</span><span class="sxs-lookup"><span data-stu-id="8577f-168">String</span></span>|<span data-ttu-id="8577f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8577f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8577f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8577f-171">displayName</span></span>|<span data-ttu-id="8577f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8577f-172">String</span></span>|<span data-ttu-id="8577f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8577f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8577f-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-175">version</span><span class="sxs-lookup"><span data-stu-id="8577f-175">version</span></span>|<span data-ttu-id="8577f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8577f-176">Int32</span></span>|<span data-ttu-id="8577f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8577f-177">Version of the device configuration.</span></span> <span data-ttu-id="8577f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8577f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="8577f-179">connectionName</span></span>|<span data-ttu-id="8577f-180">String</span><span class="sxs-lookup"><span data-stu-id="8577f-180">String</span></span>|<span data-ttu-id="8577f-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8577f-181">Connection name displayed to the user.</span></span> <span data-ttu-id="8577f-182">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-183">серверами</span><span class="sxs-lookup"><span data-stu-id="8577f-183">servers</span></span>|<span data-ttu-id="8577f-184">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="8577f-185">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="8577f-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="8577f-186">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="8577f-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="8577f-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8577f-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8577f-188">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-189">customXml</span><span class="sxs-lookup"><span data-stu-id="8577f-189">customXml</span></span>|<span data-ttu-id="8577f-190">Binary</span><span class="sxs-lookup"><span data-stu-id="8577f-190">Binary</span></span>|<span data-ttu-id="8577f-191">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="8577f-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="8577f-192">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8577f-193">профилетаржет</span><span class="sxs-lookup"><span data-stu-id="8577f-193">profileTarget</span></span>|[<span data-ttu-id="8577f-194">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="8577f-194">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="8577f-195">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="8577f-195">Profile target type.</span></span> <span data-ttu-id="8577f-196">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="8577f-196">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="8577f-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="8577f-197">connectionType</span></span>|[<span data-ttu-id="8577f-198">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="8577f-198">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="8577f-199">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="8577f-199">Connection type.</span></span> <span data-ttu-id="8577f-200">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="8577f-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="8577f-201">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="8577f-201">enableSplitTunneling</span></span>|<span data-ttu-id="8577f-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-202">Boolean</span></span>|<span data-ttu-id="8577f-203">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="8577f-203">Enable split tunneling.</span></span>|
|<span data-ttu-id="8577f-204">енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="8577f-204">enableAlwaysOn</span></span>|<span data-ttu-id="8577f-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-205">Boolean</span></span>|<span data-ttu-id="8577f-206">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="8577f-206">Enable Always On mode.</span></span>|
|<span data-ttu-id="8577f-207">енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="8577f-207">enableDeviceTunnel</span></span>|<span data-ttu-id="8577f-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-208">Boolean</span></span>|<span data-ttu-id="8577f-209">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="8577f-209">Enable device tunnel.</span></span>|
|<span data-ttu-id="8577f-210">енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="8577f-210">enableDnsRegistration</span></span>|<span data-ttu-id="8577f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-211">Boolean</span></span>|<span data-ttu-id="8577f-212">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="8577f-212">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="8577f-213">днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="8577f-213">dnsSuffixes</span></span>|<span data-ttu-id="8577f-214">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8577f-214">String collection</span></span>|<span data-ttu-id="8577f-215">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="8577f-215">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="8577f-216">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="8577f-216">authenticationMethod</span></span>|[<span data-ttu-id="8577f-217">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8577f-217">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="8577f-218">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8577f-218">Authentication method.</span></span> <span data-ttu-id="8577f-219">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="8577f-219">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="8577f-220">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="8577f-220">rememberUserCredentials</span></span>|<span data-ttu-id="8577f-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-221">Boolean</span></span>|<span data-ttu-id="8577f-222">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="8577f-222">Remember user credentials.</span></span>|
|<span data-ttu-id="8577f-223">енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="8577f-223">enableConditionalAccess</span></span>|<span data-ttu-id="8577f-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-224">Boolean</span></span>|<span data-ttu-id="8577f-225">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="8577f-225">Enable conditional access.</span></span>|
|<span data-ttu-id="8577f-226">енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="8577f-226">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="8577f-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-227">Boolean</span></span>|<span data-ttu-id="8577f-228">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="8577f-228">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="8577f-229">синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="8577f-229">singleSignOnEku</span></span>|[<span data-ttu-id="8577f-230">екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="8577f-230">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="8577f-231">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="8577f-231">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="8577f-232">синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="8577f-232">singleSignOnIssuerHash</span></span>|<span data-ttu-id="8577f-233">String</span><span class="sxs-lookup"><span data-stu-id="8577f-233">String</span></span>|<span data-ttu-id="8577f-234">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="8577f-234">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="8577f-235">еапксмл</span><span class="sxs-lookup"><span data-stu-id="8577f-235">eapXml</span></span>|<span data-ttu-id="8577f-236">Binary</span><span class="sxs-lookup"><span data-stu-id="8577f-236">Binary</span></span>|<span data-ttu-id="8577f-237">XML-файл протокола расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="8577f-237">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="8577f-238">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="8577f-238">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="8577f-239">проксисервер</span><span class="sxs-lookup"><span data-stu-id="8577f-239">proxyServer</span></span>|[<span data-ttu-id="8577f-240">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="8577f-240">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="8577f-241">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="8577f-241">Proxy Server.</span></span>|
|<span data-ttu-id="8577f-242">ассоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="8577f-242">associatedApps</span></span>|<span data-ttu-id="8577f-243">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-243">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="8577f-244">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="8577f-244">Associated Apps.</span></span> <span data-ttu-id="8577f-245">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8577f-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8577f-246">онляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="8577f-246">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="8577f-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="8577f-247">Boolean</span></span>|<span data-ttu-id="8577f-248">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="8577f-248">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="8577f-249">виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="8577f-249">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="8577f-250">String</span><span class="sxs-lookup"><span data-stu-id="8577f-250">String</span></span>|<span data-ttu-id="8577f-251">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="8577f-251">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="8577f-252">траффикрулес</span><span class="sxs-lookup"><span data-stu-id="8577f-252">trafficRules</span></span>|<span data-ttu-id="8577f-253">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-253">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="8577f-254">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="8577f-254">Traffic rules.</span></span> <span data-ttu-id="8577f-255">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8577f-255">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8577f-256">сылает</span><span class="sxs-lookup"><span data-stu-id="8577f-256">routes</span></span>|<span data-ttu-id="8577f-257">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-257">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="8577f-258">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="8577f-258">Routes (optional for third-party providers).</span></span> <span data-ttu-id="8577f-259">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8577f-259">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8577f-260">днсрулес</span><span class="sxs-lookup"><span data-stu-id="8577f-260">dnsRules</span></span>|<span data-ttu-id="8577f-261">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="8577f-261">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="8577f-262">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="8577f-262">DNS rules.</span></span> <span data-ttu-id="8577f-263">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8577f-263">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8577f-264">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="8577f-264">trustedNetworkDomains</span></span>|<span data-ttu-id="8577f-265">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8577f-265">String collection</span></span>|<span data-ttu-id="8577f-266">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="8577f-266">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="8577f-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="8577f-267">Response</span></span>
<span data-ttu-id="8577f-268">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8577f-268">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8577f-269">Пример</span><span class="sxs-lookup"><span data-stu-id="8577f-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="8577f-270">Запрос</span><span class="sxs-lookup"><span data-stu-id="8577f-270">Request</span></span>
<span data-ttu-id="8577f-271">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8577f-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4160

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8577f-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="8577f-272">Response</span></span>
<span data-ttu-id="8577f-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8577f-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4332

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```






