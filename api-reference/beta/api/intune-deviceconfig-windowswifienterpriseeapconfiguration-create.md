---
title: Создание Виндовсвифиентерприсиапконфигуратион
description: Создание нового объекта Виндовсвифиентерприсиапконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89f3a2ca38fc9b5082f73d8508271f1ff182183b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731728"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="92f67-103">Создание Виндовсвифиентерприсиапконфигуратион</span><span class="sxs-lookup"><span data-stu-id="92f67-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="92f67-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92f67-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92f67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92f67-106">Создание нового объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="92f67-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92f67-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92f67-107">Prerequisites</span></span>
<span data-ttu-id="92f67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92f67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92f67-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92f67-110">Permission type</span></span>|<span data-ttu-id="92f67-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92f67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92f67-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92f67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92f67-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f67-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92f67-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92f67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92f67-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f67-115">Not supported.</span></span>|
|<span data-ttu-id="92f67-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="92f67-116">Application</span></span>|<span data-ttu-id="92f67-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f67-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92f67-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92f67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92f67-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92f67-119">Request headers</span></span>
|<span data-ttu-id="92f67-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92f67-120">Header</span></span>|<span data-ttu-id="92f67-121">Значение</span><span class="sxs-lookup"><span data-stu-id="92f67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92f67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92f67-122">Authorization</span></span>|<span data-ttu-id="92f67-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92f67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92f67-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92f67-124">Accept</span></span>|<span data-ttu-id="92f67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92f67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92f67-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92f67-126">Request body</span></span>
<span data-ttu-id="92f67-127">В тексте запроса добавьте представление объекта Виндовсвифиентерприсиапконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92f67-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="92f67-128">В следующей таблице приведены свойства, необходимые при создании Виндовсвифиентерприсиапконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="92f67-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="92f67-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92f67-129">Property</span></span>|<span data-ttu-id="92f67-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92f67-130">Type</span></span>|<span data-ttu-id="92f67-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92f67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92f67-132">id</span><span class="sxs-lookup"><span data-stu-id="92f67-132">id</span></span>|<span data-ttu-id="92f67-133">String</span><span class="sxs-lookup"><span data-stu-id="92f67-133">String</span></span>|<span data-ttu-id="92f67-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92f67-134">Key of the entity.</span></span> <span data-ttu-id="92f67-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92f67-136">lastModifiedDateTime</span></span>|<span data-ttu-id="92f67-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f67-137">DateTimeOffset</span></span>|<span data-ttu-id="92f67-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="92f67-138">DateTime the object was last modified.</span></span> <span data-ttu-id="92f67-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92f67-140">roleScopeTagIds</span></span>|<span data-ttu-id="92f67-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="92f67-141">String collection</span></span>|<span data-ttu-id="92f67-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="92f67-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92f67-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="92f67-144">supportsScopeTags</span></span>|<span data-ttu-id="92f67-145">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-145">Boolean</span></span>|<span data-ttu-id="92f67-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="92f67-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92f67-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="92f67-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92f67-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="92f67-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92f67-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92f67-149">This property is read-only.</span></span> <span data-ttu-id="92f67-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92f67-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="92f67-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92f67-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="92f67-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="92f67-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="92f67-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92f67-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="92f67-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92f67-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="92f67-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="92f67-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="92f67-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92f67-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="92f67-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92f67-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="92f67-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="92f67-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="92f67-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92f67-163">createdDateTime</span></span>|<span data-ttu-id="92f67-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f67-164">DateTimeOffset</span></span>|<span data-ttu-id="92f67-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="92f67-165">DateTime the object was created.</span></span> <span data-ttu-id="92f67-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-167">description</span><span class="sxs-lookup"><span data-stu-id="92f67-167">description</span></span>|<span data-ttu-id="92f67-168">String</span><span class="sxs-lookup"><span data-stu-id="92f67-168">String</span></span>|<span data-ttu-id="92f67-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="92f67-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92f67-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-171">displayName</span><span class="sxs-lookup"><span data-stu-id="92f67-171">displayName</span></span>|<span data-ttu-id="92f67-172">Строка</span><span class="sxs-lookup"><span data-stu-id="92f67-172">String</span></span>|<span data-ttu-id="92f67-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="92f67-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92f67-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-175">version</span><span class="sxs-lookup"><span data-stu-id="92f67-175">version</span></span>|<span data-ttu-id="92f67-176">Int32</span><span class="sxs-lookup"><span data-stu-id="92f67-176">Int32</span></span>|<span data-ttu-id="92f67-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="92f67-177">Version of the device configuration.</span></span> <span data-ttu-id="92f67-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f67-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="92f67-179">preSharedKey</span></span>|<span data-ttu-id="92f67-180">String</span><span class="sxs-lookup"><span data-stu-id="92f67-180">String</span></span>|<span data-ttu-id="92f67-181">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="92f67-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="92f67-182">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-183">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="92f67-183">wifiSecurityType</span></span>|[<span data-ttu-id="92f67-184">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="92f67-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="92f67-185">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="92f67-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="92f67-186">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="92f67-187">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="92f67-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="92f67-188">метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="92f67-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="92f67-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="92f67-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="92f67-190">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="92f67-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="92f67-191">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="92f67-192">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="92f67-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="92f67-193">SSID</span><span class="sxs-lookup"><span data-stu-id="92f67-193">ssid</span></span>|<span data-ttu-id="92f67-194">String</span><span class="sxs-lookup"><span data-stu-id="92f67-194">String</span></span>|<span data-ttu-id="92f67-195">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="92f67-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="92f67-196">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-197">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="92f67-197">networkName</span></span>|<span data-ttu-id="92f67-198">String</span><span class="sxs-lookup"><span data-stu-id="92f67-198">String</span></span>|<span data-ttu-id="92f67-199">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="92f67-199">Specify the network configuration name.</span></span> <span data-ttu-id="92f67-200">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-201">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="92f67-201">connectAutomatically</span></span>|<span data-ttu-id="92f67-202">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-202">Boolean</span></span>|<span data-ttu-id="92f67-203">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="92f67-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="92f67-204">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-205">коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="92f67-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="92f67-206">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-206">Boolean</span></span>|<span data-ttu-id="92f67-207">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="92f67-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="92f67-208">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="92f67-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="92f67-209">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-210">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="92f67-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="92f67-211">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-211">Boolean</span></span>|<span data-ttu-id="92f67-212">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="92f67-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="92f67-213">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-214">проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="92f67-214">proxySetting</span></span>|[<span data-ttu-id="92f67-215">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="92f67-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="92f67-216">Укажите параметры прокси-сервера для конфигурации Wi-Fi, наследуемой от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92f67-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="92f67-217">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="92f67-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="92f67-218">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="92f67-218">proxyManualAddress</span></span>|<span data-ttu-id="92f67-219">String</span><span class="sxs-lookup"><span data-stu-id="92f67-219">String</span></span>|<span data-ttu-id="92f67-220">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="92f67-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="92f67-221">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-222">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="92f67-222">proxyManualPort</span></span>|<span data-ttu-id="92f67-223">Int32</span><span class="sxs-lookup"><span data-stu-id="92f67-223">Int32</span></span>|<span data-ttu-id="92f67-224">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="92f67-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="92f67-225">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-226">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="92f67-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="92f67-227">String</span><span class="sxs-lookup"><span data-stu-id="92f67-227">String</span></span>|<span data-ttu-id="92f67-228">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="92f67-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="92f67-229">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-230">форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="92f67-230">forceFIPSCompliance</span></span>|<span data-ttu-id="92f67-231">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-231">Boolean</span></span>|<span data-ttu-id="92f67-232">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="92f67-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="92f67-233">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f67-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f67-234">нетворксинглесигнон</span><span class="sxs-lookup"><span data-stu-id="92f67-234">networkSingleSignOn</span></span>|[<span data-ttu-id="92f67-235">нетворксинглесигнонтипе</span><span class="sxs-lookup"><span data-stu-id="92f67-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="92f67-236">Укажите тип единого входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="92f67-236">Specify the network single sign on type.</span></span> <span data-ttu-id="92f67-237">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="92f67-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="92f67-238">максимумаусентикатионтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="92f67-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="92f67-239">Int32</span><span class="sxs-lookup"><span data-stu-id="92f67-239">Int32</span></span>|<span data-ttu-id="92f67-240">Укажите максимальное время ожидания проверки подлинности (в секундах).</span><span class="sxs-lookup"><span data-stu-id="92f67-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="92f67-241">Допустимый диапазон: 1-120</span><span class="sxs-lookup"><span data-stu-id="92f67-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="92f67-242">промптфораддитионалаусентикатионкредентиалс</span><span class="sxs-lookup"><span data-stu-id="92f67-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="92f67-243">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-243">Boolean</span></span>|<span data-ttu-id="92f67-244">Укажите, должно ли подключение Wi-Fi запрашивать дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="92f67-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="92f67-245">енаблепаирвисемастеркэйкачинг</span><span class="sxs-lookup"><span data-stu-id="92f67-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="92f67-246">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-246">Boolean</span></span>|<span data-ttu-id="92f67-247">Укажите, следует ли включить кэширование парных главных ключей в подключении Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="92f67-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="92f67-248">максимумпаирвисемастеркэйкачетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="92f67-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="92f67-249">Int32</span><span class="sxs-lookup"><span data-stu-id="92f67-249">Int32</span></span>|<span data-ttu-id="92f67-250">Указать максимальное время кэширования парных главных ключей (в минутах).</span><span class="sxs-lookup"><span data-stu-id="92f67-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="92f67-251">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="92f67-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="92f67-252">максимумнумберофпаирвисемастеркэйсинкаче</span><span class="sxs-lookup"><span data-stu-id="92f67-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="92f67-253">Int32</span><span class="sxs-lookup"><span data-stu-id="92f67-253">Int32</span></span>|<span data-ttu-id="92f67-254">Укажите максимальное число парных главных ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="92f67-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="92f67-255">Допустимый диапазон: 1-255</span><span class="sxs-lookup"><span data-stu-id="92f67-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="92f67-256">енаблепреаусентикатион</span><span class="sxs-lookup"><span data-stu-id="92f67-256">enablePreAuthentication</span></span>|<span data-ttu-id="92f67-257">Логический</span><span class="sxs-lookup"><span data-stu-id="92f67-257">Boolean</span></span>|<span data-ttu-id="92f67-258">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="92f67-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="92f67-259">максимумпреаусентикатионаттемптс</span><span class="sxs-lookup"><span data-stu-id="92f67-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="92f67-260">Int32</span><span class="sxs-lookup"><span data-stu-id="92f67-260">Int32</span></span>|<span data-ttu-id="92f67-261">Указать максимальное количество попыток перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="92f67-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="92f67-262">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="92f67-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="92f67-263">еаптипе</span><span class="sxs-lookup"><span data-stu-id="92f67-263">eapType</span></span>|[<span data-ttu-id="92f67-264">еаптипе</span><span class="sxs-lookup"><span data-stu-id="92f67-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="92f67-265">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="92f67-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="92f67-266">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="92f67-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="92f67-267">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="92f67-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="92f67-268">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="92f67-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="92f67-269">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="92f67-269">String collection</span></span>|<span data-ttu-id="92f67-270">Укажите имена сертификатов доверенного сервера.</span><span class="sxs-lookup"><span data-stu-id="92f67-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="92f67-271">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="92f67-271">authenticationMethod</span></span>|[<span data-ttu-id="92f67-272">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="92f67-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="92f67-273">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="92f67-273">Specify the authentication method.</span></span> <span data-ttu-id="92f67-274">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="92f67-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="92f67-275">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="92f67-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="92f67-276">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="92f67-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="92f67-277">Укажите внутренний протокол проверки подлинности для EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="92f67-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="92f67-278">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="92f67-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="92f67-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="92f67-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="92f67-280">String</span><span class="sxs-lookup"><span data-stu-id="92f67-280">String</span></span>|<span data-ttu-id="92f67-281">Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="92f67-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="92f67-282">Отклик</span><span class="sxs-lookup"><span data-stu-id="92f67-282">Response</span></span>
<span data-ttu-id="92f67-283">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92f67-283">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92f67-284">Пример</span><span class="sxs-lookup"><span data-stu-id="92f67-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="92f67-285">Запрос</span><span class="sxs-lookup"><span data-stu-id="92f67-285">Request</span></span>
<span data-ttu-id="92f67-286">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92f67-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2277

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="92f67-287">Отклик</span><span class="sxs-lookup"><span data-stu-id="92f67-287">Response</span></span>
<span data-ttu-id="92f67-p134">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92f67-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2449

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




