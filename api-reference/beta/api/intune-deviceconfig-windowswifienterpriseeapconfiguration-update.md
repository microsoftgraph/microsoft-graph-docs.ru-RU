---
title: Обновление Виндовсвифиентерприсиапконфигуратион
description: Обновление свойств объекта Виндовсвифиентерприсиапконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed2afd7f75ebdec5aa334096e0e3e211daab0a94
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311296"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="e414d-103">Обновление Виндовсвифиентерприсиапконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e414d-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="e414d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e414d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e414d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e414d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e414d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e414d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e414d-107">Обновление свойств объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e414d-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e414d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e414d-108">Prerequisites</span></span>
<span data-ttu-id="e414d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e414d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e414d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e414d-111">Permission type</span></span>|<span data-ttu-id="e414d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e414d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e414d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e414d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e414d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e414d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e414d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e414d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e414d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e414d-116">Not supported.</span></span>|
|<span data-ttu-id="e414d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e414d-117">Application</span></span>|<span data-ttu-id="e414d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e414d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e414d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e414d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e414d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e414d-120">Request headers</span></span>
|<span data-ttu-id="e414d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e414d-121">Header</span></span>|<span data-ttu-id="e414d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e414d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e414d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e414d-123">Authorization</span></span>|<span data-ttu-id="e414d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e414d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e414d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e414d-125">Accept</span></span>|<span data-ttu-id="e414d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e414d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e414d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e414d-127">Request body</span></span>
<span data-ttu-id="e414d-128">В тексте запроса добавьте представление объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e414d-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="e414d-129">В следующей таблице приведены свойства, необходимые при создании [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="e414d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e414d-130">Property</span></span>|<span data-ttu-id="e414d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e414d-131">Type</span></span>|<span data-ttu-id="e414d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e414d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e414d-133">id</span><span class="sxs-lookup"><span data-stu-id="e414d-133">id</span></span>|<span data-ttu-id="e414d-134">String</span><span class="sxs-lookup"><span data-stu-id="e414d-134">String</span></span>|<span data-ttu-id="e414d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e414d-135">Key of the entity.</span></span> <span data-ttu-id="e414d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e414d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e414d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e414d-138">DateTimeOffset</span></span>|<span data-ttu-id="e414d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e414d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e414d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e414d-141">roleScopeTagIds</span></span>|<span data-ttu-id="e414d-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e414d-142">String collection</span></span>|<span data-ttu-id="e414d-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e414d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e414d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e414d-145">supportsScopeTags</span></span>|<span data-ttu-id="e414d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-146">Boolean</span></span>|<span data-ttu-id="e414d-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e414d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e414d-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e414d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e414d-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e414d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e414d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e414d-150">This property is read-only.</span></span> <span data-ttu-id="e414d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e414d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e414d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e414d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e414d-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e414d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e414d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e414d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e414d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e414d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e414d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e414d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e414d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e414d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e414d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e414d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e414d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e414d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e414d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e414d-164">createdDateTime</span></span>|<span data-ttu-id="e414d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e414d-165">DateTimeOffset</span></span>|<span data-ttu-id="e414d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e414d-166">DateTime the object was created.</span></span> <span data-ttu-id="e414d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-168">description</span><span class="sxs-lookup"><span data-stu-id="e414d-168">description</span></span>|<span data-ttu-id="e414d-169">String</span><span class="sxs-lookup"><span data-stu-id="e414d-169">String</span></span>|<span data-ttu-id="e414d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e414d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e414d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e414d-172">displayName</span></span>|<span data-ttu-id="e414d-173">String</span><span class="sxs-lookup"><span data-stu-id="e414d-173">String</span></span>|<span data-ttu-id="e414d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e414d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e414d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-176">version</span><span class="sxs-lookup"><span data-stu-id="e414d-176">version</span></span>|<span data-ttu-id="e414d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-177">Int32</span></span>|<span data-ttu-id="e414d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e414d-178">Version of the device configuration.</span></span> <span data-ttu-id="e414d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e414d-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e414d-180">preSharedKey</span></span>|<span data-ttu-id="e414d-181">String</span><span class="sxs-lookup"><span data-stu-id="e414d-181">String</span></span>|<span data-ttu-id="e414d-182">Это предварительно общий ключ для сети WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e414d-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="e414d-183">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-184">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="e414d-184">wifiSecurityType</span></span>|[<span data-ttu-id="e414d-185">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="e414d-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e414d-186">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e414d-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="e414d-187">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e414d-188">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="e414d-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e414d-189">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="e414d-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="e414d-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="e414d-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="e414d-191">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="e414d-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="e414d-192">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e414d-193">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="e414d-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="e414d-194">SSID</span><span class="sxs-lookup"><span data-stu-id="e414d-194">ssid</span></span>|<span data-ttu-id="e414d-195">String</span><span class="sxs-lookup"><span data-stu-id="e414d-195">String</span></span>|<span data-ttu-id="e414d-196">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="e414d-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="e414d-197">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-198">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="e414d-198">networkName</span></span>|<span data-ttu-id="e414d-199">String</span><span class="sxs-lookup"><span data-stu-id="e414d-199">String</span></span>|<span data-ttu-id="e414d-200">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="e414d-200">Specify the network configuration name.</span></span> <span data-ttu-id="e414d-201">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-202">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="e414d-202">connectAutomatically</span></span>|<span data-ttu-id="e414d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-203">Boolean</span></span>|<span data-ttu-id="e414d-204">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="e414d-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="e414d-205">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-206">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="e414d-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="e414d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-207">Boolean</span></span>|<span data-ttu-id="e414d-208">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="e414d-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="e414d-209">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="e414d-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="e414d-210">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-211">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="e414d-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e414d-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-212">Boolean</span></span>|<span data-ttu-id="e414d-213">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="e414d-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="e414d-214">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-215">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="e414d-215">proxySetting</span></span>|[<span data-ttu-id="e414d-216">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="e414d-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e414d-217">Укажите параметры прокси-сервера для конфигурации Wi-Fi, унаследованной от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e414d-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e414d-218">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="e414d-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e414d-219">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="e414d-219">proxyManualAddress</span></span>|<span data-ttu-id="e414d-220">String</span><span class="sxs-lookup"><span data-stu-id="e414d-220">String</span></span>|<span data-ttu-id="e414d-221">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="e414d-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="e414d-222">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-223">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="e414d-223">proxyManualPort</span></span>|<span data-ttu-id="e414d-224">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-224">Int32</span></span>|<span data-ttu-id="e414d-225">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="e414d-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="e414d-226">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-227">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="e414d-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e414d-228">String</span><span class="sxs-lookup"><span data-stu-id="e414d-228">String</span></span>|<span data-ttu-id="e414d-229">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="e414d-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="e414d-230">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-231">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="e414d-231">forceFIPSCompliance</span></span>|<span data-ttu-id="e414d-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-232">Boolean</span></span>|<span data-ttu-id="e414d-233">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="e414d-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="e414d-234">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e414d-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e414d-235">нетворксинглесигнон</span><span class="sxs-lookup"><span data-stu-id="e414d-235">networkSingleSignOn</span></span>|[<span data-ttu-id="e414d-236">нетворксинглесигнонтипе</span><span class="sxs-lookup"><span data-stu-id="e414d-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="e414d-237">Укажите тип единого входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="e414d-237">Specify the network single sign on type.</span></span> <span data-ttu-id="e414d-238">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="e414d-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="e414d-239">максимумаусентикатионтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="e414d-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="e414d-240">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-240">Int32</span></span>|<span data-ttu-id="e414d-241">Укажите максимальное время ожидания проверки подлинности (в секундах).</span><span class="sxs-lookup"><span data-stu-id="e414d-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="e414d-242">Допустимый диапазон: 1-120</span><span class="sxs-lookup"><span data-stu-id="e414d-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="e414d-243">усербаседвиртуаллан</span><span class="sxs-lookup"><span data-stu-id="e414d-243">userBasedVirtualLan</span></span>|<span data-ttu-id="e414d-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-244">Boolean</span></span>|<span data-ttu-id="e414d-245">Укажите, следует ли изменить виртуальную локальную сеть, используемую устройством на основе учетных данных пользователя.</span><span class="sxs-lookup"><span data-stu-id="e414d-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="e414d-246">Невозможно использовать, если для Нетворксинглесигнонтипе задано значение Disabled.</span><span class="sxs-lookup"><span data-stu-id="e414d-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="e414d-247">промптфораддитионалаусентикатионкредентиалс</span><span class="sxs-lookup"><span data-stu-id="e414d-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="e414d-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-248">Boolean</span></span>|<span data-ttu-id="e414d-249">Укажите, должно ли подключение Wi-Fi запрашивать дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e414d-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="e414d-250">енаблепаирвисемастеркэйкачинг</span><span class="sxs-lookup"><span data-stu-id="e414d-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="e414d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-251">Boolean</span></span>|<span data-ttu-id="e414d-252">Укажите, следует ли включить кэширование парных главных ключей в подключении Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e414d-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="e414d-253">максимумпаирвисемастеркэйкачетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="e414d-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="e414d-254">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-254">Int32</span></span>|<span data-ttu-id="e414d-255">Указать максимальное время кэширования парных главных ключей (в минутах).</span><span class="sxs-lookup"><span data-stu-id="e414d-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="e414d-256">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="e414d-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="e414d-257">максимумнумберофпаирвисемастеркэйсинкаче</span><span class="sxs-lookup"><span data-stu-id="e414d-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="e414d-258">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-258">Int32</span></span>|<span data-ttu-id="e414d-259">Укажите максимальное число парных главных ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="e414d-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="e414d-260">Допустимый диапазон: 1-255</span><span class="sxs-lookup"><span data-stu-id="e414d-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="e414d-261">енаблепреаусентикатион</span><span class="sxs-lookup"><span data-stu-id="e414d-261">enablePreAuthentication</span></span>|<span data-ttu-id="e414d-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-262">Boolean</span></span>|<span data-ttu-id="e414d-263">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="e414d-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="e414d-264">максимумпреаусентикатионаттемптс</span><span class="sxs-lookup"><span data-stu-id="e414d-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="e414d-265">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-265">Int32</span></span>|<span data-ttu-id="e414d-266">Указать максимальное количество попыток перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="e414d-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="e414d-267">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="e414d-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="e414d-268">еаптипе</span><span class="sxs-lookup"><span data-stu-id="e414d-268">eapType</span></span>|[<span data-ttu-id="e414d-269">еаптипе</span><span class="sxs-lookup"><span data-stu-id="e414d-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="e414d-270">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="e414d-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="e414d-271">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="e414d-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="e414d-272">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="e414d-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="e414d-273">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="e414d-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="e414d-274">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e414d-274">String collection</span></span>|<span data-ttu-id="e414d-275">Укажите имена сертификатов доверенного сервера.</span><span class="sxs-lookup"><span data-stu-id="e414d-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="e414d-276">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e414d-276">authenticationMethod</span></span>|[<span data-ttu-id="e414d-277">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e414d-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="e414d-278">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e414d-278">Specify the authentication method.</span></span> <span data-ttu-id="e414d-279">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e414d-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e414d-280">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="e414d-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="e414d-281">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="e414d-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="e414d-282">Укажите внутренний протокол проверки подлинности для EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="e414d-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="e414d-283">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="e414d-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="e414d-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="e414d-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="e414d-285">String</span><span class="sxs-lookup"><span data-stu-id="e414d-285">String</span></span>|<span data-ttu-id="e414d-286">Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="e414d-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="e414d-287">рекуирекриптографикбиндинг</span><span class="sxs-lookup"><span data-stu-id="e414d-287">requireCryptographicBinding</span></span>|<span data-ttu-id="e414d-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-288">Boolean</span></span>|<span data-ttu-id="e414d-289">Указывает, следует ли включить криптографическую привязку при выборе типа EAP в качестве протокола PEAP.</span><span class="sxs-lookup"><span data-stu-id="e414d-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="e414d-290">перформсервервалидатион</span><span class="sxs-lookup"><span data-stu-id="e414d-290">performServerValidation</span></span>|<span data-ttu-id="e414d-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-291">Boolean</span></span>|<span data-ttu-id="e414d-292">Укажите, следует ли включить проверку подлинности сервера путем проверки сертификата при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="e414d-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="e414d-293">дисаблеусерпромптфорсервервалидатион</span><span class="sxs-lookup"><span data-stu-id="e414d-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="e414d-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-294">Boolean</span></span>|<span data-ttu-id="e414d-295">Укажите, следует ли запретить пользователю получать запросы на авторизацию новых серверов для доверенных центров сертификации, когда в качестве протокола PEAP выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="e414d-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="e414d-296">аусентикатионпериодинсекондс</span><span class="sxs-lookup"><span data-stu-id="e414d-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="e414d-297">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-297">Int32</span></span>|<span data-ttu-id="e414d-298">Укажите количество секунд, в течение которого клиент будет ждать после попытки проверки подлинности перед отказом.</span><span class="sxs-lookup"><span data-stu-id="e414d-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="e414d-299">Допустимый диапазон 1-3600.</span><span class="sxs-lookup"><span data-stu-id="e414d-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="e414d-300">аусентикатионретриделайпериодинсекондс</span><span class="sxs-lookup"><span data-stu-id="e414d-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="e414d-301">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-301">Int32</span></span>|<span data-ttu-id="e414d-302">Укажите количество секунд между неудачной проверкой подлинности и следующей попыткой проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e414d-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="e414d-303">Допустимый диапазон 1-3600.</span><span class="sxs-lookup"><span data-stu-id="e414d-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="e414d-304">еаполстартпериодинсекондс</span><span class="sxs-lookup"><span data-stu-id="e414d-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="e414d-305">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-305">Int32</span></span>|<span data-ttu-id="e414d-306">Укажите время ожидания перед отправкой сообщения о запуске EAPOL (Extensible Authentication Protocol over LAN) в секундах.</span><span class="sxs-lookup"><span data-stu-id="e414d-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="e414d-307">Допустимый диапазон 1-3600.</span><span class="sxs-lookup"><span data-stu-id="e414d-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="e414d-308">максимумеаполстартмессажес</span><span class="sxs-lookup"><span data-stu-id="e414d-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="e414d-309">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-309">Int32</span></span>|<span data-ttu-id="e414d-310">Укажите максимальное число сообщений о запуске для отправки с помощью EAPOL (протокол расширенной проверки подлинности по локальной сети) перед возвращением отказа.</span><span class="sxs-lookup"><span data-stu-id="e414d-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="e414d-311">Допустимый диапазон 1-100.</span><span class="sxs-lookup"><span data-stu-id="e414d-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="e414d-312">максимумаусентикатионфаилурес</span><span class="sxs-lookup"><span data-stu-id="e414d-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="e414d-313">Int32</span><span class="sxs-lookup"><span data-stu-id="e414d-313">Int32</span></span>|<span data-ttu-id="e414d-314">Указывает максимальное количество сбоев проверки подлинности, разрешенных для набора учетных данных.</span><span class="sxs-lookup"><span data-stu-id="e414d-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="e414d-315">Допустимый диапазон 1-100.</span><span class="sxs-lookup"><span data-stu-id="e414d-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="e414d-316">качекредентиалс</span><span class="sxs-lookup"><span data-stu-id="e414d-316">cacheCredentials</span></span>|<span data-ttu-id="e414d-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="e414d-317">Boolean</span></span>|<span data-ttu-id="e414d-318">Укажите, следует ли кэшировать учетные данные пользователя на устройстве, чтобы пользователям не нужно было вводить их каждый раз при каждом подключении.</span><span class="sxs-lookup"><span data-stu-id="e414d-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="e414d-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="e414d-319">authenticationType</span></span>|[<span data-ttu-id="e414d-320">вифиаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="e414d-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="e414d-321">Укажите, следует ли проверять подлинность пользователя, устройства, либо использовать гостевую проверку подлинности (None).</span><span class="sxs-lookup"><span data-stu-id="e414d-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="e414d-322">Если вы используете проверку подлинности с помощью сертификата, убедитесь, что тип сертификата соответствует типу проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e414d-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="e414d-323">Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="e414d-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="e414d-324">Отклик</span><span class="sxs-lookup"><span data-stu-id="e414d-324">Response</span></span>
<span data-ttu-id="e414d-325">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e414d-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e414d-326">Пример</span><span class="sxs-lookup"><span data-stu-id="e414d-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="e414d-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="e414d-327">Request</span></span>
<span data-ttu-id="e414d-328">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e414d-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2695

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
  "userBasedVirtualLan": true,
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
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```

### <a name="response"></a><span data-ttu-id="e414d-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="e414d-329">Response</span></span>
<span data-ttu-id="e414d-p141">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e414d-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2867

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
  "userBasedVirtualLan": true,
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
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```




