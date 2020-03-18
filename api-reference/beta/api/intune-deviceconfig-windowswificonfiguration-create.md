---
title: Создание Виндовсвификонфигуратион
description: Создание нового объекта Виндовсвификонфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e64e18b1de4505680ea22393ed3665a492375866
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42732071"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="6a9c2-103">Создание Виндовсвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="6a9c2-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="6a9c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a9c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a9c2-106">Создание нового объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6a9c2-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a9c2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a9c2-107">Prerequisites</span></span>
<span data-ttu-id="6a9c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a9c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a9c2-110">Permission type</span></span>|<span data-ttu-id="6a9c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a9c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a9c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a9c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a9c2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9c2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a9c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a9c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a9c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-115">Not supported.</span></span>|
|<span data-ttu-id="6a9c2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a9c2-116">Application</span></span>|<span data-ttu-id="6a9c2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9c2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a9c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a9c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6a9c2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a9c2-119">Request headers</span></span>
|<span data-ttu-id="6a9c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a9c2-120">Header</span></span>|<span data-ttu-id="6a9c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6a9c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a9c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a9c2-122">Authorization</span></span>|<span data-ttu-id="6a9c2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a9c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6a9c2-124">Accept</span></span>|<span data-ttu-id="6a9c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a9c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a9c2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a9c2-126">Request body</span></span>
<span data-ttu-id="6a9c2-127">В тексте запроса добавьте представление объекта Виндовсвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="6a9c2-128">В следующей таблице приведены свойства, необходимые при создании Виндовсвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="6a9c2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a9c2-129">Property</span></span>|<span data-ttu-id="6a9c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6a9c2-130">Type</span></span>|<span data-ttu-id="6a9c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6a9c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a9c2-132">id</span><span class="sxs-lookup"><span data-stu-id="6a9c2-132">id</span></span>|<span data-ttu-id="6a9c2-133">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-133">String</span></span>|<span data-ttu-id="6a9c2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-134">Key of the entity.</span></span> <span data-ttu-id="6a9c2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a9c2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6a9c2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a9c2-137">DateTimeOffset</span></span>|<span data-ttu-id="6a9c2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6a9c2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a9c2-140">roleScopeTagIds</span></span>|<span data-ttu-id="6a9c2-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-141">String collection</span></span>|<span data-ttu-id="6a9c2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6a9c2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6a9c2-144">supportsScopeTags</span></span>|<span data-ttu-id="6a9c2-145">Логический</span><span class="sxs-lookup"><span data-stu-id="6a9c2-145">Boolean</span></span>|<span data-ttu-id="6a9c2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6a9c2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6a9c2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6a9c2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-149">This property is read-only.</span></span> <span data-ttu-id="6a9c2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6a9c2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6a9c2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6a9c2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6a9c2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6a9c2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6a9c2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6a9c2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6a9c2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6a9c2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6a9c2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6a9c2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6a9c2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6a9c2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6a9c2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6a9c2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a9c2-163">createdDateTime</span></span>|<span data-ttu-id="6a9c2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a9c2-164">DateTimeOffset</span></span>|<span data-ttu-id="6a9c2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-165">DateTime the object was created.</span></span> <span data-ttu-id="6a9c2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-167">description</span><span class="sxs-lookup"><span data-stu-id="6a9c2-167">description</span></span>|<span data-ttu-id="6a9c2-168">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-168">String</span></span>|<span data-ttu-id="6a9c2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a9c2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6a9c2-171">displayName</span></span>|<span data-ttu-id="6a9c2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="6a9c2-172">String</span></span>|<span data-ttu-id="6a9c2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a9c2-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-175">version</span><span class="sxs-lookup"><span data-stu-id="6a9c2-175">version</span></span>|<span data-ttu-id="6a9c2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6a9c2-176">Int32</span></span>|<span data-ttu-id="6a9c2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-177">Version of the device configuration.</span></span> <span data-ttu-id="6a9c2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6a9c2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9c2-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="6a9c2-179">preSharedKey</span></span>|<span data-ttu-id="6a9c2-180">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-180">String</span></span>|<span data-ttu-id="6a9c2-181">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="6a9c2-182">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="6a9c2-182">wifiSecurityType</span></span>|[<span data-ttu-id="6a9c2-183">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="6a9c2-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="6a9c2-184">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-184">Specify the Wifi Security Type.</span></span> <span data-ttu-id="6a9c2-185">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="6a9c2-186">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="6a9c2-186">meteredConnectionLimit</span></span>|[<span data-ttu-id="6a9c2-187">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="6a9c2-187">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="6a9c2-188">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-188">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="6a9c2-189">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-189">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="6a9c2-190">SSID</span><span class="sxs-lookup"><span data-stu-id="6a9c2-190">ssid</span></span>|<span data-ttu-id="6a9c2-191">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-191">String</span></span>|<span data-ttu-id="6a9c2-192">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-192">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="6a9c2-193">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="6a9c2-193">networkName</span></span>|<span data-ttu-id="6a9c2-194">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-194">String</span></span>|<span data-ttu-id="6a9c2-195">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-195">Specify the network configuration name.</span></span>|
|<span data-ttu-id="6a9c2-196">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="6a9c2-196">connectAutomatically</span></span>|<span data-ttu-id="6a9c2-197">Логический</span><span class="sxs-lookup"><span data-stu-id="6a9c2-197">Boolean</span></span>|<span data-ttu-id="6a9c2-198">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-198">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="6a9c2-199">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="6a9c2-199">connectToPreferredNetwork</span></span>|<span data-ttu-id="6a9c2-200">Логический</span><span class="sxs-lookup"><span data-stu-id="6a9c2-200">Boolean</span></span>|<span data-ttu-id="6a9c2-201">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-201">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="6a9c2-202">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-202">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="6a9c2-203">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="6a9c2-203">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6a9c2-204">Логический</span><span class="sxs-lookup"><span data-stu-id="6a9c2-204">Boolean</span></span>|<span data-ttu-id="6a9c2-205">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-205">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="6a9c2-206">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="6a9c2-206">proxySetting</span></span>|[<span data-ttu-id="6a9c2-207">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="6a9c2-207">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="6a9c2-208">Укажите параметры прокси-сервера для конфигурации Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-208">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="6a9c2-209">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-209">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="6a9c2-210">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="6a9c2-210">proxyManualAddress</span></span>|<span data-ttu-id="6a9c2-211">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-211">String</span></span>|<span data-ttu-id="6a9c2-212">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-212">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="6a9c2-213">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="6a9c2-213">proxyManualPort</span></span>|<span data-ttu-id="6a9c2-214">Int32</span><span class="sxs-lookup"><span data-stu-id="6a9c2-214">Int32</span></span>|<span data-ttu-id="6a9c2-215">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-215">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="6a9c2-216">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="6a9c2-216">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="6a9c2-217">String</span><span class="sxs-lookup"><span data-stu-id="6a9c2-217">String</span></span>|<span data-ttu-id="6a9c2-218">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-218">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="6a9c2-219">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="6a9c2-219">forceFIPSCompliance</span></span>|<span data-ttu-id="6a9c2-220">Логический</span><span class="sxs-lookup"><span data-stu-id="6a9c2-220">Boolean</span></span>|<span data-ttu-id="6a9c2-221">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-221">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="6a9c2-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a9c2-222">Response</span></span>
<span data-ttu-id="6a9c2-223">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-223">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a9c2-224">Пример</span><span class="sxs-lookup"><span data-stu-id="6a9c2-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a9c2-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a9c2-225">Request</span></span>
<span data-ttu-id="6a9c2-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6a9c2-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a9c2-227">Response</span></span>
<span data-ttu-id="6a9c2-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a9c2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




