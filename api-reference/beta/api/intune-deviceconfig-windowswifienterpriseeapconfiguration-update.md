---
title: Обновление Виндовсвифиентерприсиапконфигуратион
description: Обновление свойств объекта Виндовсвифиентерприсиапконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ccfe6338c3650e3d4a23a35022f35e28fbf2e6d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961128"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="2d483-103">Обновление Виндовсвифиентерприсиапконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2d483-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="2d483-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d483-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d483-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d483-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d483-106">Обновление свойств объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2d483-106">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d483-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2d483-107">Prerequisites</span></span>
<span data-ttu-id="2d483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d483-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d483-110">Permission type</span></span>|<span data-ttu-id="2d483-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d483-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d483-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d483-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d483-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d483-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d483-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d483-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d483-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d483-115">Not supported.</span></span>|
|<span data-ttu-id="2d483-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d483-116">Application</span></span>|<span data-ttu-id="2d483-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d483-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d483-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d483-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2d483-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d483-119">Request headers</span></span>
|<span data-ttu-id="2d483-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d483-120">Header</span></span>|<span data-ttu-id="2d483-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d483-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d483-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d483-122">Authorization</span></span>|<span data-ttu-id="2d483-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d483-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d483-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2d483-124">Accept</span></span>|<span data-ttu-id="2d483-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d483-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d483-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d483-126">Request body</span></span>
<span data-ttu-id="2d483-127">В тексте запроса добавьте представление объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d483-127">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="2d483-128">В следующей таблице приведены свойства, необходимые при создании [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-128">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="2d483-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d483-129">Property</span></span>|<span data-ttu-id="2d483-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2d483-130">Type</span></span>|<span data-ttu-id="2d483-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2d483-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d483-132">id</span><span class="sxs-lookup"><span data-stu-id="2d483-132">id</span></span>|<span data-ttu-id="2d483-133">String</span><span class="sxs-lookup"><span data-stu-id="2d483-133">String</span></span>|<span data-ttu-id="2d483-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d483-134">Key of the entity.</span></span> <span data-ttu-id="2d483-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d483-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d483-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d483-137">DateTimeOffset</span></span>|<span data-ttu-id="2d483-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2d483-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d483-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d483-140">roleScopeTagIds</span></span>|<span data-ttu-id="2d483-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2d483-141">String collection</span></span>|<span data-ttu-id="2d483-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2d483-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2d483-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2d483-144">supportsScopeTags</span></span>|<span data-ttu-id="2d483-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-145">Boolean</span></span>|<span data-ttu-id="2d483-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2d483-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2d483-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2d483-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2d483-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2d483-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2d483-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d483-149">This property is read-only.</span></span> <span data-ttu-id="2d483-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d483-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2d483-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d483-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2d483-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d483-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2d483-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d483-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2d483-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d483-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2d483-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d483-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2d483-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="2d483-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2d483-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="2d483-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2d483-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d483-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2d483-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d483-163">createdDateTime</span></span>|<span data-ttu-id="2d483-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d483-164">DateTimeOffset</span></span>|<span data-ttu-id="2d483-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2d483-165">DateTime the object was created.</span></span> <span data-ttu-id="2d483-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-167">description</span><span class="sxs-lookup"><span data-stu-id="2d483-167">description</span></span>|<span data-ttu-id="2d483-168">String</span><span class="sxs-lookup"><span data-stu-id="2d483-168">String</span></span>|<span data-ttu-id="2d483-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d483-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d483-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2d483-171">displayName</span></span>|<span data-ttu-id="2d483-172">Строка</span><span class="sxs-lookup"><span data-stu-id="2d483-172">String</span></span>|<span data-ttu-id="2d483-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d483-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d483-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-175">version</span><span class="sxs-lookup"><span data-stu-id="2d483-175">version</span></span>|<span data-ttu-id="2d483-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2d483-176">Int32</span></span>|<span data-ttu-id="2d483-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d483-177">Version of the device configuration.</span></span> <span data-ttu-id="2d483-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d483-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="2d483-179">preSharedKey</span></span>|<span data-ttu-id="2d483-180">String</span><span class="sxs-lookup"><span data-stu-id="2d483-180">String</span></span>|<span data-ttu-id="2d483-181">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="2d483-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="2d483-182">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="2d483-183">wifiSecurityType</span></span>|[<span data-ttu-id="2d483-184">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="2d483-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="2d483-185">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="2d483-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="2d483-186">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="2d483-187">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="2d483-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="2d483-188">Метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="2d483-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="2d483-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="2d483-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="2d483-190">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="2d483-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="2d483-191">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="2d483-192">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="2d483-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="2d483-193">SSID</span><span class="sxs-lookup"><span data-stu-id="2d483-193">ssid</span></span>|<span data-ttu-id="2d483-194">String</span><span class="sxs-lookup"><span data-stu-id="2d483-194">String</span></span>|<span data-ttu-id="2d483-195">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="2d483-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="2d483-196">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-197">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="2d483-197">networkName</span></span>|<span data-ttu-id="2d483-198">String</span><span class="sxs-lookup"><span data-stu-id="2d483-198">String</span></span>|<span data-ttu-id="2d483-199">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="2d483-199">Specify the network configuration name.</span></span> <span data-ttu-id="2d483-200">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-201">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="2d483-201">connectAutomatically</span></span>|<span data-ttu-id="2d483-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-202">Boolean</span></span>|<span data-ttu-id="2d483-203">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="2d483-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="2d483-204">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-205">Коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="2d483-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="2d483-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-206">Boolean</span></span>|<span data-ttu-id="2d483-207">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="2d483-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="2d483-208">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="2d483-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="2d483-209">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-210">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="2d483-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2d483-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-211">Boolean</span></span>|<span data-ttu-id="2d483-212">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="2d483-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="2d483-213">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-214">Проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="2d483-214">proxySetting</span></span>|[<span data-ttu-id="2d483-215">Вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="2d483-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="2d483-216">Укажите параметры прокси-сервера для конфигурации Wi-Fi, наследуемой от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d483-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="2d483-217">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="2d483-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="2d483-218">Проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="2d483-218">proxyManualAddress</span></span>|<span data-ttu-id="2d483-219">String</span><span class="sxs-lookup"><span data-stu-id="2d483-219">String</span></span>|<span data-ttu-id="2d483-220">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2d483-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="2d483-221">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-222">Проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="2d483-222">proxyManualPort</span></span>|<span data-ttu-id="2d483-223">Int32</span><span class="sxs-lookup"><span data-stu-id="2d483-223">Int32</span></span>|<span data-ttu-id="2d483-224">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2d483-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="2d483-225">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-226">Проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="2d483-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="2d483-227">String</span><span class="sxs-lookup"><span data-stu-id="2d483-227">String</span></span>|<span data-ttu-id="2d483-228">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2d483-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="2d483-229">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-230">Форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="2d483-230">forceFIPSCompliance</span></span>|<span data-ttu-id="2d483-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-231">Boolean</span></span>|<span data-ttu-id="2d483-232">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="2d483-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="2d483-233">Наследуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d483-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2d483-234">Нетворксинглесигнон</span><span class="sxs-lookup"><span data-stu-id="2d483-234">networkSingleSignOn</span></span>|[<span data-ttu-id="2d483-235">Нетворксинглесигнонтипе</span><span class="sxs-lookup"><span data-stu-id="2d483-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="2d483-236">Укажите тип единого входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="2d483-236">Specify the network single sign on type.</span></span> <span data-ttu-id="2d483-237">Возможные значения: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="2d483-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="2d483-238">Максимумаусентикатионтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="2d483-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="2d483-239">Int32</span><span class="sxs-lookup"><span data-stu-id="2d483-239">Int32</span></span>|<span data-ttu-id="2d483-240">Укажите максимальное время ожидания проверки подлинности (в секундах).</span><span class="sxs-lookup"><span data-stu-id="2d483-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="2d483-241">Допустимый диапазон: 1-120</span><span class="sxs-lookup"><span data-stu-id="2d483-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="2d483-242">Промптфораддитионалаусентикатионкредентиалс</span><span class="sxs-lookup"><span data-stu-id="2d483-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="2d483-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-243">Boolean</span></span>|<span data-ttu-id="2d483-244">Укажите, должно ли подключение Wi-Fi запрашивать дополнительные учетные данные проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d483-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="2d483-245">Енаблепаирвисемастеркэйкачинг</span><span class="sxs-lookup"><span data-stu-id="2d483-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="2d483-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-246">Boolean</span></span>|<span data-ttu-id="2d483-247">Укажите, следует ли включить кэширование парных главных ключей в подключении Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="2d483-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="2d483-248">Максимумпаирвисемастеркэйкачетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="2d483-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="2d483-249">Int32</span><span class="sxs-lookup"><span data-stu-id="2d483-249">Int32</span></span>|<span data-ttu-id="2d483-250">Указать максимальное время кэширования парных главных ключей (в минутах).</span><span class="sxs-lookup"><span data-stu-id="2d483-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="2d483-251">Допустимый диапазон: 5-1440</span><span class="sxs-lookup"><span data-stu-id="2d483-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="2d483-252">Максимумнумберофпаирвисемастеркэйсинкаче</span><span class="sxs-lookup"><span data-stu-id="2d483-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="2d483-253">Int32</span><span class="sxs-lookup"><span data-stu-id="2d483-253">Int32</span></span>|<span data-ttu-id="2d483-254">Укажите максимальное число парных главных ключей в кэше.</span><span class="sxs-lookup"><span data-stu-id="2d483-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="2d483-255">Допустимый диапазон: 1-255</span><span class="sxs-lookup"><span data-stu-id="2d483-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="2d483-256">Енаблепреаусентикатион</span><span class="sxs-lookup"><span data-stu-id="2d483-256">enablePreAuthentication</span></span>|<span data-ttu-id="2d483-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d483-257">Boolean</span></span>|<span data-ttu-id="2d483-258">Укажите, следует ли включить предварительную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d483-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="2d483-259">Максимумпреаусентикатионаттемптс</span><span class="sxs-lookup"><span data-stu-id="2d483-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="2d483-260">Int32</span><span class="sxs-lookup"><span data-stu-id="2d483-260">Int32</span></span>|<span data-ttu-id="2d483-261">Указать максимальное количество попыток перед проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d483-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="2d483-262">Допустимый диапазон: 1-16</span><span class="sxs-lookup"><span data-stu-id="2d483-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="2d483-263">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="2d483-263">eapType</span></span>|[<span data-ttu-id="2d483-264">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="2d483-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="2d483-265">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="2d483-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="2d483-266">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="2d483-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="2d483-267">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="2d483-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="2d483-268">Трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="2d483-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="2d483-269">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2d483-269">String collection</span></span>|<span data-ttu-id="2d483-270">Укажите имена сертификатов доверенного сервера.</span><span class="sxs-lookup"><span data-stu-id="2d483-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="2d483-271">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="2d483-271">authenticationMethod</span></span>|[<span data-ttu-id="2d483-272">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2d483-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="2d483-273">Укажите метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d483-273">Specify the authentication method.</span></span> <span data-ttu-id="2d483-274">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="2d483-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2d483-275">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="2d483-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="2d483-276">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="2d483-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="2d483-277">Укажите внутренний протокол проверки подлинности для EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="2d483-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="2d483-278">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="2d483-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="2d483-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="2d483-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="2d483-280">String</span><span class="sxs-lookup"><span data-stu-id="2d483-280">String</span></span>|<span data-ttu-id="2d483-281">Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="2d483-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="2d483-282">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d483-282">Response</span></span>
<span data-ttu-id="2d483-283">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d483-283">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d483-284">Пример</span><span class="sxs-lookup"><span data-stu-id="2d483-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d483-285">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d483-285">Request</span></span>
<span data-ttu-id="2d483-286">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d483-286">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2d483-287">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d483-287">Response</span></span>
<span data-ttu-id="2d483-p134">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d483-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





