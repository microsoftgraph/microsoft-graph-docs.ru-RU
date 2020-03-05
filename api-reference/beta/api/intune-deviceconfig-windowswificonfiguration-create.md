---
title: Создание Виндовсвификонфигуратион
description: Создание нового объекта Виндовсвификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55e8935c1bc845f770b78b3530a144c55dcb16cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473432"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="db4ef-103">Создание Виндовсвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="db4ef-103">Create windowsWifiConfiguration</span></span>

<span data-ttu-id="db4ef-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db4ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db4ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db4ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db4ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db4ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db4ef-107">Создание нового объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db4ef-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db4ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db4ef-108">Prerequisites</span></span>
<span data-ttu-id="db4ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db4ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db4ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db4ef-111">Permission type</span></span>|<span data-ttu-id="db4ef-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db4ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db4ef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db4ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db4ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db4ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db4ef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db4ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db4ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db4ef-116">Not supported.</span></span>|
|<span data-ttu-id="db4ef-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db4ef-117">Application</span></span>|<span data-ttu-id="db4ef-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db4ef-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db4ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db4ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db4ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="db4ef-120">Request headers</span></span>
|<span data-ttu-id="db4ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db4ef-121">Header</span></span>|<span data-ttu-id="db4ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db4ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db4ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db4ef-123">Authorization</span></span>|<span data-ttu-id="db4ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db4ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db4ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db4ef-125">Accept</span></span>|<span data-ttu-id="db4ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db4ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db4ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db4ef-127">Request body</span></span>
<span data-ttu-id="db4ef-128">В тексте запроса добавьте представление объекта Виндовсвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db4ef-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="db4ef-129">В следующей таблице приведены свойства, необходимые при создании Виндовсвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="db4ef-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="db4ef-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="db4ef-130">Property</span></span>|<span data-ttu-id="db4ef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="db4ef-131">Type</span></span>|<span data-ttu-id="db4ef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="db4ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db4ef-133">id</span><span class="sxs-lookup"><span data-stu-id="db4ef-133">id</span></span>|<span data-ttu-id="db4ef-134">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-134">String</span></span>|<span data-ttu-id="db4ef-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="db4ef-135">Key of the entity.</span></span> <span data-ttu-id="db4ef-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db4ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="db4ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db4ef-138">DateTimeOffset</span></span>|<span data-ttu-id="db4ef-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="db4ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="db4ef-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db4ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="db4ef-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="db4ef-142">String collection</span></span>|<span data-ttu-id="db4ef-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="db4ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db4ef-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="db4ef-145">supportsScopeTags</span></span>|<span data-ttu-id="db4ef-146">Логический</span><span class="sxs-lookup"><span data-stu-id="db4ef-146">Boolean</span></span>|<span data-ttu-id="db4ef-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="db4ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db4ef-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="db4ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db4ef-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="db4ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db4ef-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db4ef-150">This property is read-only.</span></span> <span data-ttu-id="db4ef-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="db4ef-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="db4ef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="db4ef-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="db4ef-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="db4ef-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="db4ef-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="db4ef-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="db4ef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="db4ef-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="db4ef-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="db4ef-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="db4ef-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="db4ef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="db4ef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="db4ef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="db4ef-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="db4ef-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="db4ef-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db4ef-164">createdDateTime</span></span>|<span data-ttu-id="db4ef-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db4ef-165">DateTimeOffset</span></span>|<span data-ttu-id="db4ef-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="db4ef-166">DateTime the object was created.</span></span> <span data-ttu-id="db4ef-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-168">description</span><span class="sxs-lookup"><span data-stu-id="db4ef-168">description</span></span>|<span data-ttu-id="db4ef-169">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-169">String</span></span>|<span data-ttu-id="db4ef-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="db4ef-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db4ef-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-172">displayName</span><span class="sxs-lookup"><span data-stu-id="db4ef-172">displayName</span></span>|<span data-ttu-id="db4ef-173">Строка</span><span class="sxs-lookup"><span data-stu-id="db4ef-173">String</span></span>|<span data-ttu-id="db4ef-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="db4ef-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db4ef-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-176">version</span><span class="sxs-lookup"><span data-stu-id="db4ef-176">version</span></span>|<span data-ttu-id="db4ef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="db4ef-177">Int32</span></span>|<span data-ttu-id="db4ef-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="db4ef-178">Version of the device configuration.</span></span> <span data-ttu-id="db4ef-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db4ef-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db4ef-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="db4ef-180">preSharedKey</span></span>|<span data-ttu-id="db4ef-181">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-181">String</span></span>|<span data-ttu-id="db4ef-182">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="db4ef-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="db4ef-183">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="db4ef-183">wifiSecurityType</span></span>|[<span data-ttu-id="db4ef-184">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="db4ef-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="db4ef-185">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="db4ef-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="db4ef-186">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="db4ef-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="db4ef-187">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="db4ef-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="db4ef-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="db4ef-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="db4ef-189">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="db4ef-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="db4ef-190">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="db4ef-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="db4ef-191">SSID</span><span class="sxs-lookup"><span data-stu-id="db4ef-191">ssid</span></span>|<span data-ttu-id="db4ef-192">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-192">String</span></span>|<span data-ttu-id="db4ef-193">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="db4ef-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="db4ef-194">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="db4ef-194">networkName</span></span>|<span data-ttu-id="db4ef-195">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-195">String</span></span>|<span data-ttu-id="db4ef-196">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="db4ef-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="db4ef-197">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="db4ef-197">connectAutomatically</span></span>|<span data-ttu-id="db4ef-198">Логический</span><span class="sxs-lookup"><span data-stu-id="db4ef-198">Boolean</span></span>|<span data-ttu-id="db4ef-199">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="db4ef-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="db4ef-200">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="db4ef-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="db4ef-201">Логический</span><span class="sxs-lookup"><span data-stu-id="db4ef-201">Boolean</span></span>|<span data-ttu-id="db4ef-202">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="db4ef-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="db4ef-203">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="db4ef-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="db4ef-204">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="db4ef-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="db4ef-205">Логический</span><span class="sxs-lookup"><span data-stu-id="db4ef-205">Boolean</span></span>|<span data-ttu-id="db4ef-206">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="db4ef-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="db4ef-207">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="db4ef-207">proxySetting</span></span>|[<span data-ttu-id="db4ef-208">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="db4ef-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="db4ef-209">Укажите параметры прокси-сервера для конфигурации Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="db4ef-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="db4ef-210">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="db4ef-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="db4ef-211">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="db4ef-211">proxyManualAddress</span></span>|<span data-ttu-id="db4ef-212">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-212">String</span></span>|<span data-ttu-id="db4ef-213">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="db4ef-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="db4ef-214">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="db4ef-214">proxyManualPort</span></span>|<span data-ttu-id="db4ef-215">Int32</span><span class="sxs-lookup"><span data-stu-id="db4ef-215">Int32</span></span>|<span data-ttu-id="db4ef-216">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="db4ef-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="db4ef-217">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="db4ef-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="db4ef-218">String</span><span class="sxs-lookup"><span data-stu-id="db4ef-218">String</span></span>|<span data-ttu-id="db4ef-219">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="db4ef-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="db4ef-220">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="db4ef-220">forceFIPSCompliance</span></span>|<span data-ttu-id="db4ef-221">Логический</span><span class="sxs-lookup"><span data-stu-id="db4ef-221">Boolean</span></span>|<span data-ttu-id="db4ef-222">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="db4ef-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="db4ef-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="db4ef-223">Response</span></span>
<span data-ttu-id="db4ef-224">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db4ef-224">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db4ef-225">Пример</span><span class="sxs-lookup"><span data-stu-id="db4ef-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="db4ef-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="db4ef-226">Request</span></span>
<span data-ttu-id="db4ef-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db4ef-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db4ef-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="db4ef-228">Response</span></span>
<span data-ttu-id="db4ef-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db4ef-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





