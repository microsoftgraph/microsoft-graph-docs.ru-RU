---
title: Обновление macOSEnterpriseWiFiConfiguration
description: Обновление свойств объекта macOSEnterpriseWiFiConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57fa3910f4b3bf9ac65f1968e0803839ed68cc02
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42746332"
---
# <a name="update-macosenterprisewificonfiguration"></a><span data-ttu-id="c716e-103">Обновление macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="c716e-103">Update macOSEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="c716e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c716e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c716e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c716e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c716e-106">Обновление свойств объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c716e-106">Update the properties of a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c716e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c716e-107">Prerequisites</span></span>
<span data-ttu-id="c716e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c716e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c716e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c716e-110">Permission type</span></span>|<span data-ttu-id="c716e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c716e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c716e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c716e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c716e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c716e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c716e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c716e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c716e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c716e-115">Not supported.</span></span>|
|<span data-ttu-id="c716e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c716e-116">Application</span></span>|<span data-ttu-id="c716e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c716e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c716e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c716e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c716e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c716e-119">Request headers</span></span>
|<span data-ttu-id="c716e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c716e-120">Header</span></span>|<span data-ttu-id="c716e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c716e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c716e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c716e-122">Authorization</span></span>|<span data-ttu-id="c716e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c716e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c716e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c716e-124">Accept</span></span>|<span data-ttu-id="c716e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c716e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c716e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c716e-126">Request body</span></span>
<span data-ttu-id="c716e-127">В тексте запроса добавьте представление объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c716e-127">In the request body, supply a JSON representation for the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="c716e-128">В следующей таблице приведены свойства, необходимые при создании [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-128">The following table shows the properties that are required when you create the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="c716e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c716e-129">Property</span></span>|<span data-ttu-id="c716e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c716e-130">Type</span></span>|<span data-ttu-id="c716e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c716e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c716e-132">id</span><span class="sxs-lookup"><span data-stu-id="c716e-132">id</span></span>|<span data-ttu-id="c716e-133">String</span><span class="sxs-lookup"><span data-stu-id="c716e-133">String</span></span>|<span data-ttu-id="c716e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c716e-134">Key of the entity.</span></span> <span data-ttu-id="c716e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c716e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c716e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c716e-137">DateTimeOffset</span></span>|<span data-ttu-id="c716e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c716e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c716e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c716e-140">roleScopeTagIds</span></span>|<span data-ttu-id="c716e-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c716e-141">String collection</span></span>|<span data-ttu-id="c716e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c716e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c716e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c716e-144">supportsScopeTags</span></span>|<span data-ttu-id="c716e-145">Логический</span><span class="sxs-lookup"><span data-stu-id="c716e-145">Boolean</span></span>|<span data-ttu-id="c716e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c716e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c716e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c716e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c716e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c716e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c716e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c716e-149">This property is read-only.</span></span> <span data-ttu-id="c716e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c716e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c716e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c716e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c716e-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c716e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c716e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c716e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c716e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c716e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c716e-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c716e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c716e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c716e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c716e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c716e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c716e-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c716e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c716e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c716e-163">createdDateTime</span></span>|<span data-ttu-id="c716e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c716e-164">DateTimeOffset</span></span>|<span data-ttu-id="c716e-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c716e-165">DateTime the object was created.</span></span> <span data-ttu-id="c716e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-167">description</span><span class="sxs-lookup"><span data-stu-id="c716e-167">description</span></span>|<span data-ttu-id="c716e-168">String</span><span class="sxs-lookup"><span data-stu-id="c716e-168">String</span></span>|<span data-ttu-id="c716e-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c716e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c716e-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c716e-171">displayName</span></span>|<span data-ttu-id="c716e-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c716e-172">String</span></span>|<span data-ttu-id="c716e-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c716e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c716e-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-175">version</span><span class="sxs-lookup"><span data-stu-id="c716e-175">version</span></span>|<span data-ttu-id="c716e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c716e-176">Int32</span></span>|<span data-ttu-id="c716e-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c716e-177">Version of the device configuration.</span></span> <span data-ttu-id="c716e-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c716e-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="c716e-179">networkName</span></span>|<span data-ttu-id="c716e-180">String</span><span class="sxs-lookup"><span data-stu-id="c716e-180">String</span></span>|<span data-ttu-id="c716e-181">Сетевое имя, унаследованное от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-181">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-182">SSID</span><span class="sxs-lookup"><span data-stu-id="c716e-182">ssid</span></span>|<span data-ttu-id="c716e-183">String</span><span class="sxs-lookup"><span data-stu-id="c716e-183">String</span></span>|<span data-ttu-id="c716e-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="c716e-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="c716e-185">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-185">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="c716e-186">connectAutomatically</span></span>|<span data-ttu-id="c716e-187">Логический</span><span class="sxs-lookup"><span data-stu-id="c716e-187">Boolean</span></span>|<span data-ttu-id="c716e-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c716e-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="c716e-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="c716e-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="c716e-190">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-190">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-191">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="c716e-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c716e-192">Логический</span><span class="sxs-lookup"><span data-stu-id="c716e-192">Boolean</span></span>|<span data-ttu-id="c716e-193">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="c716e-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="c716e-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="c716e-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="c716e-195">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-195">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="c716e-196">wiFiSecurityType</span></span>|[<span data-ttu-id="c716e-197">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="c716e-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="c716e-198">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="c716e-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="c716e-199">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-199">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="c716e-200">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="c716e-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="c716e-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="c716e-201">proxySettings</span></span>|[<span data-ttu-id="c716e-202">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="c716e-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="c716e-203">Тип прокси-сервера для этого подключения Wi-Fi наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c716e-203">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="c716e-204">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="c716e-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="c716e-205">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="c716e-205">proxyManualAddress</span></span>|<span data-ttu-id="c716e-206">String</span><span class="sxs-lookup"><span data-stu-id="c716e-206">String</span></span>|<span data-ttu-id="c716e-207">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="c716e-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="c716e-208">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-208">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-209">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="c716e-209">proxyManualPort</span></span>|<span data-ttu-id="c716e-210">Int32</span><span class="sxs-lookup"><span data-stu-id="c716e-210">Int32</span></span>|<span data-ttu-id="c716e-211">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="c716e-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="c716e-212">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-212">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-213">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="c716e-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="c716e-214">String</span><span class="sxs-lookup"><span data-stu-id="c716e-214">String</span></span>|<span data-ttu-id="c716e-215">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="c716e-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="c716e-216">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="c716e-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="c716e-217">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-217">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="c716e-218">preSharedKey</span></span>|<span data-ttu-id="c716e-219">String</span><span class="sxs-lookup"><span data-stu-id="c716e-219">String</span></span>|<span data-ttu-id="c716e-220">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="c716e-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="c716e-221">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c716e-221">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="c716e-222">еаптипе</span><span class="sxs-lookup"><span data-stu-id="c716e-222">eapType</span></span>|[<span data-ttu-id="c716e-223">еаптипе</span><span class="sxs-lookup"><span data-stu-id="c716e-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="c716e-224">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="c716e-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="c716e-225">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="c716e-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c716e-226">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="c716e-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="c716e-227">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c716e-227">eapFastConfiguration</span></span>|[<span data-ttu-id="c716e-228">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c716e-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="c716e-229">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="c716e-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="c716e-230">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="c716e-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="c716e-231">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="c716e-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="c716e-232">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c716e-232">String collection</span></span>|<span data-ttu-id="c716e-233">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="c716e-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="c716e-234">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="c716e-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="c716e-235">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c716e-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="c716e-236">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c716e-236">authenticationMethod</span></span>|[<span data-ttu-id="c716e-237">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="c716e-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c716e-238">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="c716e-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="c716e-239">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c716e-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c716e-240">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="c716e-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="c716e-241">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="c716e-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c716e-242">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="c716e-242">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="c716e-243">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="c716e-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c716e-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c716e-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c716e-245">String</span><span class="sxs-lookup"><span data-stu-id="c716e-245">String</span></span>|<span data-ttu-id="c716e-246">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="c716e-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="c716e-247">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="c716e-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="c716e-248">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этого подключения Wi-Fi, с помощью действительного имени пользователя отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="c716e-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="c716e-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="c716e-249">Response</span></span>
<span data-ttu-id="c716e-250">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c716e-250">If successful, this method returns a `200 OK` response code and an updated [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c716e-251">Пример</span><span class="sxs-lookup"><span data-stu-id="c716e-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="c716e-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="c716e-252">Request</span></span>
<span data-ttu-id="c716e-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c716e-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1858

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="c716e-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="c716e-254">Response</span></span>
<span data-ttu-id="c716e-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c716e-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2030

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




