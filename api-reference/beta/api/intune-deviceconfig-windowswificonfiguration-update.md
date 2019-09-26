---
title: Обновление Виндовсвификонфигуратион
description: Обновление свойств объекта Виндовсвификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2085c35f967fba84a3b459c77156eaa5611dc33d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181331"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="4b5cb-103">Обновление Виндовсвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="4b5cb-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="4b5cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b5cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b5cb-106">Обновление свойств объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4b5cb-106">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b5cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b5cb-107">Prerequisites</span></span>
<span data-ttu-id="4b5cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b5cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b5cb-110">Permission type</span></span>|<span data-ttu-id="4b5cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b5cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b5cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b5cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b5cb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5cb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b5cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b5cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b5cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-115">Not supported.</span></span>|
|<span data-ttu-id="4b5cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b5cb-116">Application</span></span>|<span data-ttu-id="4b5cb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5cb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b5cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b5cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4b5cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b5cb-119">Request headers</span></span>
|<span data-ttu-id="4b5cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b5cb-120">Header</span></span>|<span data-ttu-id="4b5cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b5cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b5cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b5cb-122">Authorization</span></span>|<span data-ttu-id="4b5cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b5cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b5cb-124">Accept</span></span>|<span data-ttu-id="4b5cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b5cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5cb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b5cb-126">Request body</span></span>
<span data-ttu-id="4b5cb-127">В тексте запроса добавьте представление объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-127">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="4b5cb-128">В следующей таблице приведены свойства, необходимые при создании [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-128">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="4b5cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b5cb-129">Property</span></span>|<span data-ttu-id="4b5cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b5cb-130">Type</span></span>|<span data-ttu-id="4b5cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b5cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b5cb-132">id</span><span class="sxs-lookup"><span data-stu-id="4b5cb-132">id</span></span>|<span data-ttu-id="4b5cb-133">String</span><span class="sxs-lookup"><span data-stu-id="4b5cb-133">String</span></span>|<span data-ttu-id="4b5cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-134">Key of the entity.</span></span> <span data-ttu-id="4b5cb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5cb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4b5cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5cb-137">DateTimeOffset</span></span>|<span data-ttu-id="4b5cb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4b5cb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b5cb-140">roleScopeTagIds</span></span>|<span data-ttu-id="4b5cb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4b5cb-141">String collection</span></span>|<span data-ttu-id="4b5cb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b5cb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4b5cb-144">supportsScopeTags</span></span>|<span data-ttu-id="4b5cb-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-145">Boolean</span></span>|<span data-ttu-id="4b5cb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b5cb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b5cb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b5cb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-149">This property is read-only.</span></span> <span data-ttu-id="4b5cb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b5cb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4b5cb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b5cb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4b5cb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4b5cb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b5cb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4b5cb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b5cb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4b5cb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4b5cb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4b5cb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4b5cb-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4b5cb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4b5cb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4b5cb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5cb-163">createdDateTime</span></span>|<span data-ttu-id="4b5cb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5cb-164">DateTimeOffset</span></span>|<span data-ttu-id="4b5cb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-165">DateTime the object was created.</span></span> <span data-ttu-id="4b5cb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-167">description</span><span class="sxs-lookup"><span data-stu-id="4b5cb-167">description</span></span>|<span data-ttu-id="4b5cb-168">String</span><span class="sxs-lookup"><span data-stu-id="4b5cb-168">String</span></span>|<span data-ttu-id="4b5cb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b5cb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4b5cb-171">displayName</span></span>|<span data-ttu-id="4b5cb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4b5cb-172">String</span></span>|<span data-ttu-id="4b5cb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b5cb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-175">version</span><span class="sxs-lookup"><span data-stu-id="4b5cb-175">version</span></span>|<span data-ttu-id="4b5cb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4b5cb-176">Int32</span></span>|<span data-ttu-id="4b5cb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-177">Version of the device configuration.</span></span> <span data-ttu-id="4b5cb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b5cb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b5cb-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="4b5cb-179">preSharedKey</span></span>|<span data-ttu-id="4b5cb-180">String.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-180">String</span></span>|<span data-ttu-id="4b5cb-181">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="4b5cb-182">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="4b5cb-182">wifiSecurityType</span></span>|[<span data-ttu-id="4b5cb-183">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="4b5cb-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="4b5cb-184">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-184">Specify the Wifi Security Type.</span></span> <span data-ttu-id="4b5cb-185">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="4b5cb-186">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="4b5cb-186">meteredConnectionLimit</span></span>|[<span data-ttu-id="4b5cb-187">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="4b5cb-187">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="4b5cb-188">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-188">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="4b5cb-189">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-189">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="4b5cb-190">SSID</span><span class="sxs-lookup"><span data-stu-id="4b5cb-190">ssid</span></span>|<span data-ttu-id="4b5cb-191">String.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-191">String</span></span>|<span data-ttu-id="4b5cb-192">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-192">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="4b5cb-193">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="4b5cb-193">networkName</span></span>|<span data-ttu-id="4b5cb-194">String.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-194">String</span></span>|<span data-ttu-id="4b5cb-195">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-195">Specify the network configuration name.</span></span>|
|<span data-ttu-id="4b5cb-196">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="4b5cb-196">connectAutomatically</span></span>|<span data-ttu-id="4b5cb-197">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-197">Boolean</span></span>|<span data-ttu-id="4b5cb-198">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-198">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="4b5cb-199">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="4b5cb-199">connectToPreferredNetwork</span></span>|<span data-ttu-id="4b5cb-200">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-200">Boolean</span></span>|<span data-ttu-id="4b5cb-201">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-201">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="4b5cb-202">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-202">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="4b5cb-203">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="4b5cb-203">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="4b5cb-204">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-204">Boolean</span></span>|<span data-ttu-id="4b5cb-205">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-205">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="4b5cb-206">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="4b5cb-206">proxySetting</span></span>|[<span data-ttu-id="4b5cb-207">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="4b5cb-207">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="4b5cb-208">Укажите параметры прокси-сервера для конфигурации Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-208">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="4b5cb-209">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-209">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="4b5cb-210">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="4b5cb-210">proxyManualAddress</span></span>|<span data-ttu-id="4b5cb-211">String.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-211">String</span></span>|<span data-ttu-id="4b5cb-212">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-212">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="4b5cb-213">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="4b5cb-213">proxyManualPort</span></span>|<span data-ttu-id="4b5cb-214">Int32</span><span class="sxs-lookup"><span data-stu-id="4b5cb-214">Int32</span></span>|<span data-ttu-id="4b5cb-215">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-215">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="4b5cb-216">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="4b5cb-216">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="4b5cb-217">String.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-217">String</span></span>|<span data-ttu-id="4b5cb-218">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-218">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="4b5cb-219">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="4b5cb-219">forceFIPSCompliance</span></span>|<span data-ttu-id="4b5cb-220">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-220">Boolean</span></span>|<span data-ttu-id="4b5cb-221">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-221">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="4b5cb-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b5cb-222">Response</span></span>
<span data-ttu-id="4b5cb-223">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-223">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b5cb-224">Пример</span><span class="sxs-lookup"><span data-stu-id="4b5cb-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b5cb-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b5cb-225">Request</span></span>
<span data-ttu-id="4b5cb-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="4b5cb-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b5cb-227">Response</span></span>
<span data-ttu-id="4b5cb-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b5cb-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1731

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```




