---
title: Создание windows10VpnConfiguration
description: Создание нового объекта windows10VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b29e09613b5d82ca3c24bc030472d8fed53df6fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980640"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="9f3ec-103">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f3ec-103">Create windows10VpnConfiguration</span></span>

<span data-ttu-id="9f3ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f3ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f3ec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f3ec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f3ec-107">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9f3ec-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f3ec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f3ec-108">Prerequisites</span></span>
<span data-ttu-id="9f3ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f3ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f3ec-111">Permission type</span></span>|<span data-ttu-id="9f3ec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f3ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f3ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f3ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f3ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f3ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-116">Not supported.</span></span>|
|<span data-ttu-id="9f3ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f3ec-117">Application</span></span>|<span data-ttu-id="9f3ec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f3ec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f3ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f3ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9f3ec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f3ec-120">Request headers</span></span>
|<span data-ttu-id="9f3ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f3ec-121">Header</span></span>|<span data-ttu-id="9f3ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f3ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f3ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f3ec-123">Authorization</span></span>|<span data-ttu-id="9f3ec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f3ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f3ec-125">Accept</span></span>|<span data-ttu-id="9f3ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f3ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f3ec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f3ec-127">Request body</span></span>
<span data-ttu-id="9f3ec-128">В тексте запроса добавьте представление объекта windows10VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="9f3ec-129">В следующей таблице приведены свойства, необходимые при создании windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="9f3ec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f3ec-130">Property</span></span>|<span data-ttu-id="9f3ec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f3ec-131">Type</span></span>|<span data-ttu-id="9f3ec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f3ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f3ec-133">id</span><span class="sxs-lookup"><span data-stu-id="9f3ec-133">id</span></span>|<span data-ttu-id="9f3ec-134">String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-134">String</span></span>|<span data-ttu-id="9f3ec-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-135">Key of the entity.</span></span> <span data-ttu-id="9f3ec-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f3ec-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9f3ec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f3ec-138">DateTimeOffset</span></span>|<span data-ttu-id="9f3ec-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9f3ec-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f3ec-141">roleScopeTagIds</span></span>|<span data-ttu-id="9f3ec-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-142">String collection</span></span>|<span data-ttu-id="9f3ec-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f3ec-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9f3ec-145">supportsScopeTags</span></span>|<span data-ttu-id="9f3ec-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-146">Boolean</span></span>|<span data-ttu-id="9f3ec-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f3ec-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f3ec-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f3ec-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-150">This property is read-only.</span></span> <span data-ttu-id="9f3ec-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f3ec-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9f3ec-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f3ec-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9f3ec-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9f3ec-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f3ec-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9f3ec-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f3ec-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9f3ec-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9f3ec-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f3ec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9f3ec-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f3ec-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9f3ec-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9f3ec-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f3ec-164">createdDateTime</span></span>|<span data-ttu-id="9f3ec-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f3ec-165">DateTimeOffset</span></span>|<span data-ttu-id="9f3ec-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-166">DateTime the object was created.</span></span> <span data-ttu-id="9f3ec-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-168">description</span><span class="sxs-lookup"><span data-stu-id="9f3ec-168">description</span></span>|<span data-ttu-id="9f3ec-169">String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-169">String</span></span>|<span data-ttu-id="9f3ec-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f3ec-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9f3ec-172">displayName</span></span>|<span data-ttu-id="9f3ec-173">String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-173">String</span></span>|<span data-ttu-id="9f3ec-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f3ec-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-176">version</span><span class="sxs-lookup"><span data-stu-id="9f3ec-176">version</span></span>|<span data-ttu-id="9f3ec-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9f3ec-177">Int32</span></span>|<span data-ttu-id="9f3ec-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-178">Version of the device configuration.</span></span> <span data-ttu-id="9f3ec-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="9f3ec-180">connectionName</span></span>|<span data-ttu-id="9f3ec-181">String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-181">String</span></span>|<span data-ttu-id="9f3ec-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-182">Connection name displayed to the user.</span></span> <span data-ttu-id="9f3ec-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-184">серверами</span><span class="sxs-lookup"><span data-stu-id="9f3ec-184">servers</span></span>|<span data-ttu-id="9f3ec-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9f3ec-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="9f3ec-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9f3ec-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9f3ec-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-190">customXml</span><span class="sxs-lookup"><span data-stu-id="9f3ec-190">customXml</span></span>|<span data-ttu-id="9f3ec-191">Binary</span><span class="sxs-lookup"><span data-stu-id="9f3ec-191">Binary</span></span>|<span data-ttu-id="9f3ec-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="9f3ec-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9f3ec-194">профилетаржет</span><span class="sxs-lookup"><span data-stu-id="9f3ec-194">profileTarget</span></span>|[<span data-ttu-id="9f3ec-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="9f3ec-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="9f3ec-196">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-196">Profile target type.</span></span> <span data-ttu-id="9f3ec-197">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="9f3ec-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="9f3ec-198">connectionType</span></span>|[<span data-ttu-id="9f3ec-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9f3ec-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="9f3ec-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-200">Connection type.</span></span> <span data-ttu-id="9f3ec-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="9f3ec-202">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="9f3ec-202">enableSplitTunneling</span></span>|<span data-ttu-id="9f3ec-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-203">Boolean</span></span>|<span data-ttu-id="9f3ec-204">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="9f3ec-205">енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="9f3ec-205">enableAlwaysOn</span></span>|<span data-ttu-id="9f3ec-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-206">Boolean</span></span>|<span data-ttu-id="9f3ec-207">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="9f3ec-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="9f3ec-208">енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="9f3ec-208">enableDeviceTunnel</span></span>|<span data-ttu-id="9f3ec-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-209">Boolean</span></span>|<span data-ttu-id="9f3ec-210">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="9f3ec-211">енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="9f3ec-211">enableDnsRegistration</span></span>|<span data-ttu-id="9f3ec-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-212">Boolean</span></span>|<span data-ttu-id="9f3ec-213">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="9f3ec-214">днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="9f3ec-214">dnsSuffixes</span></span>|<span data-ttu-id="9f3ec-215">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-215">String collection</span></span>|<span data-ttu-id="9f3ec-216">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="9f3ec-217">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="9f3ec-217">authenticationMethod</span></span>|[<span data-ttu-id="9f3ec-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9f3ec-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="9f3ec-219">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-219">Authentication method.</span></span> <span data-ttu-id="9f3ec-220">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9f3ec-221">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="9f3ec-221">rememberUserCredentials</span></span>|<span data-ttu-id="9f3ec-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-222">Boolean</span></span>|<span data-ttu-id="9f3ec-223">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-223">Remember user credentials.</span></span>|
|<span data-ttu-id="9f3ec-224">енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="9f3ec-224">enableConditionalAccess</span></span>|<span data-ttu-id="9f3ec-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-225">Boolean</span></span>|<span data-ttu-id="9f3ec-226">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-226">Enable conditional access.</span></span>|
|<span data-ttu-id="9f3ec-227">енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="9f3ec-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="9f3ec-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-228">Boolean</span></span>|<span data-ttu-id="9f3ec-229">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="9f3ec-230">синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="9f3ec-230">singleSignOnEku</span></span>|[<span data-ttu-id="9f3ec-231">екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="9f3ec-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="9f3ec-232">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="9f3ec-233">синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="9f3ec-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="9f3ec-234">String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-234">String</span></span>|<span data-ttu-id="9f3ec-235">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="9f3ec-236">еапксмл</span><span class="sxs-lookup"><span data-stu-id="9f3ec-236">eapXml</span></span>|<span data-ttu-id="9f3ec-237">Binary</span><span class="sxs-lookup"><span data-stu-id="9f3ec-237">Binary</span></span>|<span data-ttu-id="9f3ec-238">XML-файл протокола расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="9f3ec-239">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="9f3ec-240">проксисервер</span><span class="sxs-lookup"><span data-stu-id="9f3ec-240">proxyServer</span></span>|[<span data-ttu-id="9f3ec-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9f3ec-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="9f3ec-242">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-242">Proxy Server.</span></span>|
|<span data-ttu-id="9f3ec-243">ассоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="9f3ec-243">associatedApps</span></span>|<span data-ttu-id="9f3ec-244">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="9f3ec-245">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-245">Associated Apps.</span></span> <span data-ttu-id="9f3ec-246">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9f3ec-247">онляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="9f3ec-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="9f3ec-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f3ec-248">Boolean</span></span>|<span data-ttu-id="9f3ec-249">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="9f3ec-250">виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="9f3ec-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="9f3ec-251">String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-251">String</span></span>|<span data-ttu-id="9f3ec-252">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="9f3ec-253">траффикрулес</span><span class="sxs-lookup"><span data-stu-id="9f3ec-253">trafficRules</span></span>|<span data-ttu-id="9f3ec-254">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="9f3ec-255">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-255">Traffic rules.</span></span> <span data-ttu-id="9f3ec-256">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="9f3ec-257">сылает</span><span class="sxs-lookup"><span data-stu-id="9f3ec-257">routes</span></span>|<span data-ttu-id="9f3ec-258">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="9f3ec-259">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="9f3ec-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="9f3ec-260">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="9f3ec-261">днсрулес</span><span class="sxs-lookup"><span data-stu-id="9f3ec-261">dnsRules</span></span>|<span data-ttu-id="9f3ec-262">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="9f3ec-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="9f3ec-263">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-263">DNS rules.</span></span> <span data-ttu-id="9f3ec-264">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="9f3ec-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="9f3ec-265">trustedNetworkDomains</span></span>|<span data-ttu-id="9f3ec-266">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f3ec-266">String collection</span></span>|<span data-ttu-id="9f3ec-267">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="9f3ec-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="9f3ec-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="9f3ec-268">cryptographySuite</span></span>|[<span data-ttu-id="9f3ec-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="9f3ec-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="9f3ec-270">Параметры безопасности комплекта шифрования для VPN-подключения по протоколу IKEv2 в Windows10 и более поздних версий</span><span class="sxs-lookup"><span data-stu-id="9f3ec-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="9f3ec-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f3ec-271">Response</span></span>
<span data-ttu-id="9f3ec-272">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-272">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f3ec-273">Пример</span><span class="sxs-lookup"><span data-stu-id="9f3ec-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f3ec-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f3ec-274">Request</span></span>
<span data-ttu-id="9f3ec-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4463

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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```

### <a name="response"></a><span data-ttu-id="9f3ec-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f3ec-276">Response</span></span>
<span data-ttu-id="9f3ec-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f3ec-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4635

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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```






