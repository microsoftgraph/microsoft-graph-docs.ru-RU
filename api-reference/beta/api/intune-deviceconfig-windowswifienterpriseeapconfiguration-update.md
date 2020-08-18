---
title: Обновление Виндовсвифиентерприсиапконфигуратион
description: Обновление свойств объекта Виндовсвифиентерприсиапконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0119e99ea7bf14b6177134157d9fd9b9008bb8b
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790352"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="f7fe4-103">Обновление Виндовсвифиентерприсиапконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f7fe4-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="f7fe4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7fe4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7fe4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7fe4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7fe4-107">Обновление свойств объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7fe4-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7fe4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7fe4-108">Prerequisites</span></span>
<span data-ttu-id="f7fe4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fe4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7fe4-111">Permission type</span></span>|<span data-ttu-id="f7fe4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7fe4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fe4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7fe4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7fe4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-116">Not supported.</span></span>|
|<span data-ttu-id="f7fe4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f7fe4-117">Application</span></span>|<span data-ttu-id="f7fe4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fe4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7fe4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7fe4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7fe4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7fe4-120">Request headers</span></span>
|<span data-ttu-id="f7fe4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7fe4-121">Header</span></span>|<span data-ttu-id="f7fe4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7fe4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7fe4-123">Authorization</span></span>|<span data-ttu-id="f7fe4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7fe4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7fe4-125">Accept</span></span>|<span data-ttu-id="f7fe4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7fe4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fe4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7fe4-127">Request body</span></span>
<span data-ttu-id="f7fe4-128">В тексте запроса добавьте представление объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="f7fe4-129">В следующей таблице приведены свойства, необходимые при создании [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="f7fe4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7fe4-130">Property</span></span>|<span data-ttu-id="f7fe4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7fe4-131">Type</span></span>|<span data-ttu-id="f7fe4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7fe4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7fe4-133">id</span><span class="sxs-lookup"><span data-stu-id="f7fe4-133">id</span></span>|<span data-ttu-id="f7fe4-134">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-134">String</span></span>|<span data-ttu-id="f7fe4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-135">Key of the entity.</span></span> <span data-ttu-id="f7fe4-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7fe4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f7fe4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7fe4-138">DateTimeOffset</span></span>|<span data-ttu-id="f7fe4-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f7fe4-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7fe4-141">roleScopeTagIds</span></span>|<span data-ttu-id="f7fe4-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-142">String collection</span></span>|<span data-ttu-id="f7fe4-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f7fe4-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f7fe4-145">supportsScopeTags</span></span>|<span data-ttu-id="f7fe4-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-146">Boolean</span></span>|<span data-ttu-id="f7fe4-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f7fe4-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f7fe4-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f7fe4-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-150">This property is read-only.</span></span> <span data-ttu-id="f7fe4-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f7fe4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f7fe4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f7fe4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f7fe4-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f7fe4-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f7fe4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f7fe4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f7fe4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f7fe4-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f7fe4-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f7fe4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f7fe4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f7fe4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f7fe4-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f7fe4-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7fe4-164">createdDateTime</span></span>|<span data-ttu-id="f7fe4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7fe4-165">DateTimeOffset</span></span>|<span data-ttu-id="f7fe4-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-166">DateTime the object was created.</span></span> <span data-ttu-id="f7fe4-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-168">description</span><span class="sxs-lookup"><span data-stu-id="f7fe4-168">description</span></span>|<span data-ttu-id="f7fe4-169">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-169">String</span></span>|<span data-ttu-id="f7fe4-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f7fe4-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f7fe4-172">displayName</span></span>|<span data-ttu-id="f7fe4-173">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-173">String</span></span>|<span data-ttu-id="f7fe4-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f7fe4-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-176">version</span><span class="sxs-lookup"><span data-stu-id="f7fe4-176">version</span></span>|<span data-ttu-id="f7fe4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fe4-177">Int32</span></span>|<span data-ttu-id="f7fe4-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-178">Version of the device configuration.</span></span> <span data-ttu-id="f7fe4-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f7fe4-180">preSharedKey</span></span>|<span data-ttu-id="f7fe4-181">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-181">String</span></span>|<span data-ttu-id="f7fe4-182">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="f7fe4-183">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-184">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f7fe4-184">wifiSecurityType</span></span>|[<span data-ttu-id="f7fe4-185">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f7fe4-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="f7fe4-186">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="f7fe4-187">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="f7fe4-188">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f7fe4-189">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="f7fe4-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="f7fe4-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="f7fe4-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="f7fe4-191">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="f7fe4-192">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="f7fe4-193">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="f7fe4-194">SSID</span><span class="sxs-lookup"><span data-stu-id="f7fe4-194">ssid</span></span>|<span data-ttu-id="f7fe4-195">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-195">String</span></span>|<span data-ttu-id="f7fe4-196">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="f7fe4-197">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-198">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="f7fe4-198">networkName</span></span>|<span data-ttu-id="f7fe4-199">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-199">String</span></span>|<span data-ttu-id="f7fe4-200">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-200">Specify the network configuration name.</span></span> <span data-ttu-id="f7fe4-201">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-202">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="f7fe4-202">connectAutomatically</span></span>|<span data-ttu-id="f7fe4-203">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-203">Boolean</span></span>|<span data-ttu-id="f7fe4-204">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="f7fe4-205">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-206">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="f7fe4-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="f7fe4-207">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-207">Boolean</span></span>|<span data-ttu-id="f7fe4-208">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="f7fe4-209">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="f7fe4-210">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-211">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="f7fe4-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f7fe4-212">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-212">Boolean</span></span>|<span data-ttu-id="f7fe4-213">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="f7fe4-214">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-215">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="f7fe4-215">proxySetting</span></span>|[<span data-ttu-id="f7fe4-216">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="f7fe4-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f7fe4-217">Укажите параметры прокси-сервера для конфигурации Wi-Fi, наследуемой от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="f7fe4-218">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f7fe4-219">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="f7fe4-219">proxyManualAddress</span></span>|<span data-ttu-id="f7fe4-220">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-220">String</span></span>|<span data-ttu-id="f7fe4-221">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="f7fe4-222">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-223">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="f7fe4-223">proxyManualPort</span></span>|<span data-ttu-id="f7fe4-224">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fe4-224">Int32</span></span>|<span data-ttu-id="f7fe4-225">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="f7fe4-226">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-227">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="f7fe4-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f7fe4-228">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-228">String</span></span>|<span data-ttu-id="f7fe4-229">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="f7fe4-230">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-231">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="f7fe4-231">forceFIPSCompliance</span></span>|<span data-ttu-id="f7fe4-232">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-232">Boolean</span></span>|<span data-ttu-id="f7fe4-233">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="f7fe4-234">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7fe4-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="f7fe4-235">нетворксинглесигнон</span><span class="sxs-lookup"><span data-stu-id="f7fe4-235">networkSingleSignOn</span></span>|[<span data-ttu-id="f7fe4-236">нетворксинглесигнонтипе</span><span class="sxs-lookup"><span data-stu-id="f7fe4-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="f7fe4-237">Укажите тип единого входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-237">Specify the network single sign on type.</span></span> <span data-ttu-id="f7fe4-238">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="f7fe4-239">максимумаусентикатионтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="f7fe4-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="f7fe4-240">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fe4-240">Int32</span></span>|<span data-ttu-id="f7fe4-241">Укажите максимальное время ожидания проверки подлинности (в секундах).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="f7fe4-242">Допустимый диапазон: 1-120</span><span class="sxs-lookup"><span data-stu-id="f7fe4-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="f7fe4-243">промптфораддитионалаусентикатионкредентиалс</span><span class="sxs-lookup"><span data-stu-id="f7fe4-243">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="f7fe4-244">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-244">Boolean</span></span>|<span data-ttu-id="f7fe4-245">Укажите, должно ли подключение Wi-Fi запрашивать дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-245">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="f7fe4-246">енаблепаирвисемастеркэйкачинг</span><span class="sxs-lookup"><span data-stu-id="f7fe4-246">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="f7fe4-247">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-247">Boolean</span></span>|<span data-ttu-id="f7fe4-248">Укажите, следует ли включить кэширование парных главных ключей в подключении Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-248">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="f7fe4-249">максимумпаирвисемастеркэйкачетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="f7fe4-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="f7fe4-250">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fe4-250">Int32</span></span>|<span data-ttu-id="f7fe4-251">Указать максимальное время кэширования парных главных ключей (в минутах).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-251">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="f7fe4-252">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="f7fe4-252">Valid range: 5-1440</span></span>|
|<span data-ttu-id="f7fe4-253">максимумнумберофпаирвисемастеркэйсинкаче</span><span class="sxs-lookup"><span data-stu-id="f7fe4-253">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="f7fe4-254">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fe4-254">Int32</span></span>|<span data-ttu-id="f7fe4-255">Укажите максимальное число парных главных ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-255">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="f7fe4-256">Допустимый диапазон: 1-255</span><span class="sxs-lookup"><span data-stu-id="f7fe4-256">Valid range: 1-255</span></span>|
|<span data-ttu-id="f7fe4-257">енаблепреаусентикатион</span><span class="sxs-lookup"><span data-stu-id="f7fe4-257">enablePreAuthentication</span></span>|<span data-ttu-id="f7fe4-258">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-258">Boolean</span></span>|<span data-ttu-id="f7fe4-259">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-259">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="f7fe4-260">максимумпреаусентикатионаттемптс</span><span class="sxs-lookup"><span data-stu-id="f7fe4-260">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="f7fe4-261">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fe4-261">Int32</span></span>|<span data-ttu-id="f7fe4-262">Указать максимальное количество попыток перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-262">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="f7fe4-263">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="f7fe4-263">Valid range: 1-16</span></span>|
|<span data-ttu-id="f7fe4-264">еаптипе</span><span class="sxs-lookup"><span data-stu-id="f7fe4-264">eapType</span></span>|[<span data-ttu-id="f7fe4-265">еаптипе</span><span class="sxs-lookup"><span data-stu-id="f7fe4-265">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="f7fe4-266">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-266">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="f7fe4-267">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="f7fe4-267">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f7fe4-268">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-268">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="f7fe4-269">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="f7fe4-269">trustedServerCertificateNames</span></span>|<span data-ttu-id="f7fe4-270">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-270">String collection</span></span>|<span data-ttu-id="f7fe4-271">Укажите имена сертификатов доверенного сервера.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-271">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="f7fe4-272">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f7fe4-272">authenticationMethod</span></span>|[<span data-ttu-id="f7fe4-273">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f7fe4-273">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f7fe4-274">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-274">Specify the authentication method.</span></span> <span data-ttu-id="f7fe4-275">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-275">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f7fe4-276">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="f7fe4-276">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="f7fe4-277">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="f7fe4-277">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f7fe4-278">Укажите внутренний протокол проверки подлинности для EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-278">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="f7fe4-279">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-279">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f7fe4-280">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f7fe4-280">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f7fe4-281">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-281">String</span></span>|<span data-ttu-id="f7fe4-282">Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-282">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="f7fe4-283">рекуирекриптографикбиндинг</span><span class="sxs-lookup"><span data-stu-id="f7fe4-283">requireCryptographicBinding</span></span>|<span data-ttu-id="f7fe4-284">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-284">Boolean</span></span>|<span data-ttu-id="f7fe4-285">Указывает, следует ли включить криптографическую привязку при выборе типа EAP в качестве протокола PEAP.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-285">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="f7fe4-286">перформсервервалидатион</span><span class="sxs-lookup"><span data-stu-id="f7fe4-286">performServerValidation</span></span>|<span data-ttu-id="f7fe4-287">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-287">Boolean</span></span>|<span data-ttu-id="f7fe4-288">Укажите, следует ли включить проверку подлинности сервера путем проверки сертификата при выборе типа EAP в качестве PEAP.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-288">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="f7fe4-289">дисаблеусерпромптфорсервервалидатион</span><span class="sxs-lookup"><span data-stu-id="f7fe4-289">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="f7fe4-290">Логический</span><span class="sxs-lookup"><span data-stu-id="f7fe4-290">Boolean</span></span>|<span data-ttu-id="f7fe4-291">Укажите, следует ли запретить пользователю получать запросы на авторизацию новых серверов для доверенных центров сертификации, когда в качестве протокола PEAP выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-291">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="f7fe4-292">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7fe4-292">Response</span></span>
<span data-ttu-id="f7fe4-293">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-293">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7fe4-294">Пример</span><span class="sxs-lookup"><span data-stu-id="f7fe4-294">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7fe4-295">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7fe4-295">Request</span></span>
<span data-ttu-id="f7fe4-296">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-296">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7fe4-297">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7fe4-297">Response</span></span>
<span data-ttu-id="f7fe4-p134">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7fe4-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



