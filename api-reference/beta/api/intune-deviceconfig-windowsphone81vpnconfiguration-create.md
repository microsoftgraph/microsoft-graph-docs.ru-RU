---
title: Создание windowsPhone81VpnConfiguration
description: Создание нового объекта windowsPhone81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 287d4a67673fc25bad6829b5d93a66c36d692e6a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532738"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="1faa4-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1faa4-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="1faa4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1faa4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1faa4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1faa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1faa4-106">Создание нового объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1faa4-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1faa4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1faa4-107">Prerequisites</span></span>
<span data-ttu-id="1faa4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1faa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1faa4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1faa4-110">Permission type</span></span>|<span data-ttu-id="1faa4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1faa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1faa4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1faa4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1faa4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1faa4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1faa4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1faa4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1faa4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1faa4-115">Not supported.</span></span>|
|<span data-ttu-id="1faa4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1faa4-116">Application</span></span>|<span data-ttu-id="1faa4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1faa4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1faa4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1faa4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1faa4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1faa4-119">Request headers</span></span>
|<span data-ttu-id="1faa4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1faa4-120">Header</span></span>|<span data-ttu-id="1faa4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1faa4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1faa4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1faa4-122">Authorization</span></span>|<span data-ttu-id="1faa4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1faa4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1faa4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1faa4-124">Accept</span></span>|<span data-ttu-id="1faa4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1faa4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1faa4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1faa4-126">Request body</span></span>
<span data-ttu-id="1faa4-127">В тексте запроса добавьте представление объекта windowsPhone81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1faa4-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="1faa4-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1faa4-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="1faa4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1faa4-129">Property</span></span>|<span data-ttu-id="1faa4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1faa4-130">Type</span></span>|<span data-ttu-id="1faa4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1faa4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1faa4-132">id</span><span class="sxs-lookup"><span data-stu-id="1faa4-132">id</span></span>|<span data-ttu-id="1faa4-133">String</span><span class="sxs-lookup"><span data-stu-id="1faa4-133">String</span></span>|<span data-ttu-id="1faa4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1faa4-134">Key of the entity.</span></span> <span data-ttu-id="1faa4-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1faa4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1faa4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1faa4-137">DateTimeOffset</span></span>|<span data-ttu-id="1faa4-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1faa4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1faa4-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1faa4-140">roleScopeTagIds</span></span>|<span data-ttu-id="1faa4-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1faa4-141">String collection</span></span>|<span data-ttu-id="1faa4-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1faa4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1faa4-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1faa4-144">supportsScopeTags</span></span>|<span data-ttu-id="1faa4-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1faa4-145">Boolean</span></span>|<span data-ttu-id="1faa4-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1faa4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1faa4-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1faa4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1faa4-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1faa4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1faa4-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1faa4-149">This property is read-only.</span></span> <span data-ttu-id="1faa4-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1faa4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1faa4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1faa4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1faa4-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1faa4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1faa4-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1faa4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1faa4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1faa4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1faa4-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1faa4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1faa4-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1faa4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1faa4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1faa4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1faa4-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1faa4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1faa4-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1faa4-163">createdDateTime</span></span>|<span data-ttu-id="1faa4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1faa4-164">DateTimeOffset</span></span>|<span data-ttu-id="1faa4-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1faa4-165">DateTime the object was created.</span></span> <span data-ttu-id="1faa4-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-167">description</span><span class="sxs-lookup"><span data-stu-id="1faa4-167">description</span></span>|<span data-ttu-id="1faa4-168">String</span><span class="sxs-lookup"><span data-stu-id="1faa4-168">String</span></span>|<span data-ttu-id="1faa4-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1faa4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1faa4-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1faa4-171">displayName</span></span>|<span data-ttu-id="1faa4-172">Строка</span><span class="sxs-lookup"><span data-stu-id="1faa4-172">String</span></span>|<span data-ttu-id="1faa4-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1faa4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1faa4-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-175">version</span><span class="sxs-lookup"><span data-stu-id="1faa4-175">version</span></span>|<span data-ttu-id="1faa4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1faa4-176">Int32</span></span>|<span data-ttu-id="1faa4-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1faa4-177">Version of the device configuration.</span></span> <span data-ttu-id="1faa4-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="1faa4-179">connectionName</span></span>|<span data-ttu-id="1faa4-180">String</span><span class="sxs-lookup"><span data-stu-id="1faa4-180">String</span></span>|<span data-ttu-id="1faa4-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1faa4-181">Connection name displayed to the user.</span></span> <span data-ttu-id="1faa4-182">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-183">серверами</span><span class="sxs-lookup"><span data-stu-id="1faa4-183">servers</span></span>|<span data-ttu-id="1faa4-184">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1faa4-185">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="1faa4-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="1faa4-186">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="1faa4-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1faa4-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1faa4-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1faa4-188">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-189">customXml</span><span class="sxs-lookup"><span data-stu-id="1faa4-189">customXml</span></span>|<span data-ttu-id="1faa4-190">Binary</span><span class="sxs-lookup"><span data-stu-id="1faa4-190">Binary</span></span>|<span data-ttu-id="1faa4-191">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="1faa4-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="1faa4-192">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="1faa4-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="1faa4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1faa4-194">Boolean</span></span>|<span data-ttu-id="1faa4-195">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="1faa4-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="1faa4-196">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1faa4-196">This property is read-only.</span></span> <span data-ttu-id="1faa4-197">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-197">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="1faa4-198">connectionType</span></span>|[<span data-ttu-id="1faa4-199">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="1faa4-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="1faa4-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="1faa4-200">Connection type.</span></span> <span data-ttu-id="1faa4-201">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1faa4-201">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="1faa4-202">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="1faa4-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="1faa4-203">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="1faa4-203">loginGroupOrDomain</span></span>|<span data-ttu-id="1faa4-204">String</span><span class="sxs-lookup"><span data-stu-id="1faa4-204">String</span></span>|<span data-ttu-id="1faa4-205">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="1faa4-205">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="1faa4-206">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-206">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-207">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="1faa4-207">enableSplitTunneling</span></span>|<span data-ttu-id="1faa4-208">Логический</span><span class="sxs-lookup"><span data-stu-id="1faa4-208">Boolean</span></span>|<span data-ttu-id="1faa4-209">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="1faa4-209">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="1faa4-210">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-210">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-211">проксисервер</span><span class="sxs-lookup"><span data-stu-id="1faa4-211">proxyServer</span></span>|[<span data-ttu-id="1faa4-212">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1faa4-212">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="1faa4-213">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="1faa4-213">Proxy Server.</span></span> <span data-ttu-id="1faa4-214">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1faa4-214">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1faa4-215">бипассвпнонкомпанивифи</span><span class="sxs-lookup"><span data-stu-id="1faa4-215">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="1faa4-216">Логический</span><span class="sxs-lookup"><span data-stu-id="1faa4-216">Boolean</span></span>|<span data-ttu-id="1faa4-217">Обход VPN в сети Wi-Fi компании.</span><span class="sxs-lookup"><span data-stu-id="1faa4-217">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="1faa4-218">бипассвпнонхомевифи</span><span class="sxs-lookup"><span data-stu-id="1faa4-218">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="1faa4-219">Логический</span><span class="sxs-lookup"><span data-stu-id="1faa4-219">Boolean</span></span>|<span data-ttu-id="1faa4-220">Обход VPN для домашнего Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="1faa4-220">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="1faa4-221">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="1faa4-221">authenticationMethod</span></span>|[<span data-ttu-id="1faa4-222">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="1faa4-222">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="1faa4-223">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1faa4-223">Authentication method.</span></span> <span data-ttu-id="1faa4-224">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="1faa4-224">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="1faa4-225">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="1faa4-225">rememberUserCredentials</span></span>|<span data-ttu-id="1faa4-226">Логический</span><span class="sxs-lookup"><span data-stu-id="1faa4-226">Boolean</span></span>|<span data-ttu-id="1faa4-227">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="1faa4-227">Remember user credentials.</span></span>|
|<span data-ttu-id="1faa4-228">днссуффикссеарчлист</span><span class="sxs-lookup"><span data-stu-id="1faa4-228">dnsSuffixSearchList</span></span>|<span data-ttu-id="1faa4-229">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1faa4-229">String collection</span></span>|<span data-ttu-id="1faa4-230">Список поиска DNS-суффиксов.</span><span class="sxs-lookup"><span data-stu-id="1faa4-230">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="1faa4-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="1faa4-231">Response</span></span>
<span data-ttu-id="1faa4-232">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1faa4-232">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1faa4-233">Пример</span><span class="sxs-lookup"><span data-stu-id="1faa4-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="1faa4-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="1faa4-234">Request</span></span>
<span data-ttu-id="1faa4-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1faa4-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1faa4-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="1faa4-236">Response</span></span>
<span data-ttu-id="1faa4-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1faa4-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```






