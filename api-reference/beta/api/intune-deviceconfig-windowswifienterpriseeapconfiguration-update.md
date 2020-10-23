---
title: Обновление Виндовсвифиентерприсиапконфигуратион
description: Обновление свойств объекта Виндовсвифиентерприсиапконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6522ebf5b487350de83894a839dd7925d743f57
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693313"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="792ca-103">Обновление Виндовсвифиентерприсиапконфигуратион</span><span class="sxs-lookup"><span data-stu-id="792ca-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="792ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="792ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="792ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="792ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="792ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="792ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="792ca-107">Обновление свойств объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="792ca-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="792ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="792ca-108">Prerequisites</span></span>
<span data-ttu-id="792ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="792ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="792ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="792ca-111">Permission type</span></span>|<span data-ttu-id="792ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="792ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="792ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="792ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="792ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="792ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="792ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="792ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="792ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="792ca-116">Not supported.</span></span>|
|<span data-ttu-id="792ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="792ca-117">Application</span></span>|<span data-ttu-id="792ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="792ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="792ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="792ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="792ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="792ca-120">Request headers</span></span>
|<span data-ttu-id="792ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="792ca-121">Header</span></span>|<span data-ttu-id="792ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="792ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="792ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="792ca-123">Authorization</span></span>|<span data-ttu-id="792ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="792ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="792ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="792ca-125">Accept</span></span>|<span data-ttu-id="792ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="792ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="792ca-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="792ca-127">Request body</span></span>
<span data-ttu-id="792ca-128">В тексте запроса добавьте представление объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="792ca-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="792ca-129">В следующей таблице приведены свойства, необходимые при создании [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="792ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="792ca-130">Property</span></span>|<span data-ttu-id="792ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="792ca-131">Type</span></span>|<span data-ttu-id="792ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="792ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="792ca-133">id</span><span class="sxs-lookup"><span data-stu-id="792ca-133">id</span></span>|<span data-ttu-id="792ca-134">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-134">String</span></span>|<span data-ttu-id="792ca-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="792ca-135">Key of the entity.</span></span> <span data-ttu-id="792ca-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="792ca-137">lastModifiedDateTime</span></span>|<span data-ttu-id="792ca-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="792ca-138">DateTimeOffset</span></span>|<span data-ttu-id="792ca-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="792ca-139">DateTime the object was last modified.</span></span> <span data-ttu-id="792ca-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="792ca-141">roleScopeTagIds</span></span>|<span data-ttu-id="792ca-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="792ca-142">String collection</span></span>|<span data-ttu-id="792ca-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="792ca-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="792ca-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="792ca-145">supportsScopeTags</span></span>|<span data-ttu-id="792ca-146">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-146">Boolean</span></span>|<span data-ttu-id="792ca-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="792ca-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="792ca-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="792ca-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="792ca-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="792ca-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="792ca-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="792ca-150">This property is read-only.</span></span> <span data-ttu-id="792ca-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="792ca-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="792ca-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="792ca-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="792ca-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="792ca-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="792ca-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="792ca-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="792ca-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="792ca-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="792ca-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="792ca-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="792ca-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="792ca-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="792ca-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="792ca-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="792ca-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="792ca-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="792ca-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="792ca-164">createdDateTime</span></span>|<span data-ttu-id="792ca-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="792ca-165">DateTimeOffset</span></span>|<span data-ttu-id="792ca-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="792ca-166">DateTime the object was created.</span></span> <span data-ttu-id="792ca-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-168">description</span><span class="sxs-lookup"><span data-stu-id="792ca-168">description</span></span>|<span data-ttu-id="792ca-169">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-169">String</span></span>|<span data-ttu-id="792ca-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="792ca-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="792ca-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-172">displayName</span><span class="sxs-lookup"><span data-stu-id="792ca-172">displayName</span></span>|<span data-ttu-id="792ca-173">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-173">String</span></span>|<span data-ttu-id="792ca-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="792ca-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="792ca-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-176">version</span><span class="sxs-lookup"><span data-stu-id="792ca-176">version</span></span>|<span data-ttu-id="792ca-177">Int32</span><span class="sxs-lookup"><span data-stu-id="792ca-177">Int32</span></span>|<span data-ttu-id="792ca-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="792ca-178">Version of the device configuration.</span></span> <span data-ttu-id="792ca-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="792ca-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="792ca-180">preSharedKey</span></span>|<span data-ttu-id="792ca-181">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-181">String</span></span>|<span data-ttu-id="792ca-182">Это предварительно общий ключ для сети WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="792ca-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="792ca-183">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-184">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="792ca-184">wifiSecurityType</span></span>|[<span data-ttu-id="792ca-185">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="792ca-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="792ca-186">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="792ca-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="792ca-187">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="792ca-188">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="792ca-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="792ca-189">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="792ca-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="792ca-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="792ca-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="792ca-191">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="792ca-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="792ca-192">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="792ca-193">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="792ca-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="792ca-194">SSID</span><span class="sxs-lookup"><span data-stu-id="792ca-194">ssid</span></span>|<span data-ttu-id="792ca-195">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-195">String</span></span>|<span data-ttu-id="792ca-196">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="792ca-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="792ca-197">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-198">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="792ca-198">networkName</span></span>|<span data-ttu-id="792ca-199">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-199">String</span></span>|<span data-ttu-id="792ca-200">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="792ca-200">Specify the network configuration name.</span></span> <span data-ttu-id="792ca-201">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-202">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="792ca-202">connectAutomatically</span></span>|<span data-ttu-id="792ca-203">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-203">Boolean</span></span>|<span data-ttu-id="792ca-204">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="792ca-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="792ca-205">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-206">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="792ca-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="792ca-207">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-207">Boolean</span></span>|<span data-ttu-id="792ca-208">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="792ca-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="792ca-209">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="792ca-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="792ca-210">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-211">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="792ca-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="792ca-212">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-212">Boolean</span></span>|<span data-ttu-id="792ca-213">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="792ca-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="792ca-214">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-215">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="792ca-215">proxySetting</span></span>|[<span data-ttu-id="792ca-216">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="792ca-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="792ca-217">Укажите параметры прокси-сервера для конфигурации Wi-Fi, унаследованной от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="792ca-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="792ca-218">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="792ca-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="792ca-219">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="792ca-219">proxyManualAddress</span></span>|<span data-ttu-id="792ca-220">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-220">String</span></span>|<span data-ttu-id="792ca-221">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="792ca-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="792ca-222">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-223">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="792ca-223">proxyManualPort</span></span>|<span data-ttu-id="792ca-224">Int32</span><span class="sxs-lookup"><span data-stu-id="792ca-224">Int32</span></span>|<span data-ttu-id="792ca-225">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="792ca-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="792ca-226">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-227">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="792ca-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="792ca-228">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-228">String</span></span>|<span data-ttu-id="792ca-229">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="792ca-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="792ca-230">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-231">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="792ca-231">forceFIPSCompliance</span></span>|<span data-ttu-id="792ca-232">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-232">Boolean</span></span>|<span data-ttu-id="792ca-233">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="792ca-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="792ca-234">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="792ca-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="792ca-235">нетворксинглесигнон</span><span class="sxs-lookup"><span data-stu-id="792ca-235">networkSingleSignOn</span></span>|[<span data-ttu-id="792ca-236">нетворксинглесигнонтипе</span><span class="sxs-lookup"><span data-stu-id="792ca-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="792ca-237">Укажите тип единого входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="792ca-237">Specify the network single sign on type.</span></span> <span data-ttu-id="792ca-238">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="792ca-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="792ca-239">максимумаусентикатионтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="792ca-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="792ca-240">Int32</span><span class="sxs-lookup"><span data-stu-id="792ca-240">Int32</span></span>|<span data-ttu-id="792ca-241">Укажите максимальное время ожидания проверки подлинности (в секундах).</span><span class="sxs-lookup"><span data-stu-id="792ca-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="792ca-242">Допустимый диапазон: 1-120</span><span class="sxs-lookup"><span data-stu-id="792ca-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="792ca-243">промптфораддитионалаусентикатионкредентиалс</span><span class="sxs-lookup"><span data-stu-id="792ca-243">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="792ca-244">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-244">Boolean</span></span>|<span data-ttu-id="792ca-245">Укажите, должно ли подключение Wi-Fi запрашивать дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="792ca-245">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="792ca-246">енаблепаирвисемастеркэйкачинг</span><span class="sxs-lookup"><span data-stu-id="792ca-246">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="792ca-247">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-247">Boolean</span></span>|<span data-ttu-id="792ca-248">Укажите, следует ли включить кэширование парных главных ключей в подключении Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="792ca-248">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="792ca-249">максимумпаирвисемастеркэйкачетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="792ca-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="792ca-250">Int32</span><span class="sxs-lookup"><span data-stu-id="792ca-250">Int32</span></span>|<span data-ttu-id="792ca-251">Указать максимальное время кэширования парных главных ключей (в минутах).</span><span class="sxs-lookup"><span data-stu-id="792ca-251">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="792ca-252">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="792ca-252">Valid range: 5-1440</span></span>|
|<span data-ttu-id="792ca-253">максимумнумберофпаирвисемастеркэйсинкаче</span><span class="sxs-lookup"><span data-stu-id="792ca-253">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="792ca-254">Int32</span><span class="sxs-lookup"><span data-stu-id="792ca-254">Int32</span></span>|<span data-ttu-id="792ca-255">Укажите максимальное число парных главных ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="792ca-255">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="792ca-256">Допустимый диапазон: 1-255</span><span class="sxs-lookup"><span data-stu-id="792ca-256">Valid range: 1-255</span></span>|
|<span data-ttu-id="792ca-257">енаблепреаусентикатион</span><span class="sxs-lookup"><span data-stu-id="792ca-257">enablePreAuthentication</span></span>|<span data-ttu-id="792ca-258">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-258">Boolean</span></span>|<span data-ttu-id="792ca-259">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="792ca-259">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="792ca-260">максимумпреаусентикатионаттемптс</span><span class="sxs-lookup"><span data-stu-id="792ca-260">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="792ca-261">Int32</span><span class="sxs-lookup"><span data-stu-id="792ca-261">Int32</span></span>|<span data-ttu-id="792ca-262">Указать максимальное количество попыток перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="792ca-262">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="792ca-263">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="792ca-263">Valid range: 1-16</span></span>|
|<span data-ttu-id="792ca-264">еаптипе</span><span class="sxs-lookup"><span data-stu-id="792ca-264">eapType</span></span>|[<span data-ttu-id="792ca-265">еаптипе</span><span class="sxs-lookup"><span data-stu-id="792ca-265">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="792ca-266">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="792ca-266">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="792ca-267">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="792ca-267">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="792ca-268">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="792ca-268">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="792ca-269">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="792ca-269">trustedServerCertificateNames</span></span>|<span data-ttu-id="792ca-270">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="792ca-270">String collection</span></span>|<span data-ttu-id="792ca-271">Укажите имена сертификатов доверенного сервера.</span><span class="sxs-lookup"><span data-stu-id="792ca-271">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="792ca-272">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="792ca-272">authenticationMethod</span></span>|[<span data-ttu-id="792ca-273">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="792ca-273">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="792ca-274">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="792ca-274">Specify the authentication method.</span></span> <span data-ttu-id="792ca-275">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="792ca-275">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="792ca-276">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="792ca-276">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="792ca-277">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="792ca-277">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="792ca-278">Укажите внутренний протокол проверки подлинности для EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="792ca-278">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="792ca-279">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="792ca-279">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="792ca-280">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="792ca-280">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="792ca-281">Строка</span><span class="sxs-lookup"><span data-stu-id="792ca-281">String</span></span>|<span data-ttu-id="792ca-282">Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="792ca-282">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="792ca-283">рекуирекриптографикбиндинг</span><span class="sxs-lookup"><span data-stu-id="792ca-283">requireCryptographicBinding</span></span>|<span data-ttu-id="792ca-284">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-284">Boolean</span></span>|<span data-ttu-id="792ca-285">Указывает, следует ли включить криптографическую привязку при выборе типа EAP в качестве протокола PEAP.</span><span class="sxs-lookup"><span data-stu-id="792ca-285">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="792ca-286">перформсервервалидатион</span><span class="sxs-lookup"><span data-stu-id="792ca-286">performServerValidation</span></span>|<span data-ttu-id="792ca-287">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-287">Boolean</span></span>|<span data-ttu-id="792ca-288">Укажите, следует ли включить проверку подлинности сервера путем проверки сертификата при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="792ca-288">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="792ca-289">дисаблеусерпромптфорсервервалидатион</span><span class="sxs-lookup"><span data-stu-id="792ca-289">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="792ca-290">Логический</span><span class="sxs-lookup"><span data-stu-id="792ca-290">Boolean</span></span>|<span data-ttu-id="792ca-291">Укажите, следует ли запретить пользователю получать запросы на авторизацию новых серверов для доверенных центров сертификации, когда в качестве протокола PEAP выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="792ca-291">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="792ca-292">Ответ</span><span class="sxs-lookup"><span data-stu-id="792ca-292">Response</span></span>
<span data-ttu-id="792ca-293">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="792ca-293">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="792ca-294">Пример</span><span class="sxs-lookup"><span data-stu-id="792ca-294">Example</span></span>

### <a name="request"></a><span data-ttu-id="792ca-295">Запрос</span><span class="sxs-lookup"><span data-stu-id="792ca-295">Request</span></span>
<span data-ttu-id="792ca-296">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="792ca-296">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2402

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true
}
```

### <a name="response"></a><span data-ttu-id="792ca-297">Отклик</span><span class="sxs-lookup"><span data-stu-id="792ca-297">Response</span></span>
<span data-ttu-id="792ca-p134">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="792ca-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2574

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true
}
```





