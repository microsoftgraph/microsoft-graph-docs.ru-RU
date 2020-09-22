---
title: Обновление androidEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0031757281fdbeebe39077378b2edf8c5ded8eb8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970280"
---
# <a name="update-androidenterprisewificonfiguration"></a><span data-ttu-id="8ccdb-103">Обновление androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ccdb-103">Update androidEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="8ccdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ccdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ccdb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ccdb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ccdb-107">Обновление свойств объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8ccdb-107">Update the properties of a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ccdb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ccdb-108">Prerequisites</span></span>
<span data-ttu-id="8ccdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ccdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ccdb-111">Permission type</span></span>|<span data-ttu-id="8ccdb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ccdb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ccdb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ccdb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ccdb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ccdb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-116">Not supported.</span></span>|
|<span data-ttu-id="8ccdb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ccdb-117">Application</span></span>|<span data-ttu-id="8ccdb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ccdb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ccdb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ccdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8ccdb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ccdb-120">Request headers</span></span>
|<span data-ttu-id="8ccdb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ccdb-121">Header</span></span>|<span data-ttu-id="8ccdb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ccdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ccdb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ccdb-123">Authorization</span></span>|<span data-ttu-id="8ccdb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ccdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ccdb-125">Accept</span></span>|<span data-ttu-id="8ccdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ccdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ccdb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ccdb-127">Request body</span></span>
<span data-ttu-id="8ccdb-128">В тексте запроса добавьте представление объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-128">In the request body, supply a JSON representation for the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="8ccdb-129">В следующей таблице приведены свойства, необходимые при создании [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-129">The following table shows the properties that are required when you create the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="8ccdb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ccdb-130">Property</span></span>|<span data-ttu-id="8ccdb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ccdb-131">Type</span></span>|<span data-ttu-id="8ccdb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ccdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ccdb-133">id</span><span class="sxs-lookup"><span data-stu-id="8ccdb-133">id</span></span>|<span data-ttu-id="8ccdb-134">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-134">String</span></span>|<span data-ttu-id="8ccdb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-135">Key of the entity.</span></span> <span data-ttu-id="8ccdb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ccdb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8ccdb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ccdb-138">DateTimeOffset</span></span>|<span data-ttu-id="8ccdb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8ccdb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ccdb-141">roleScopeTagIds</span></span>|<span data-ttu-id="8ccdb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-142">String collection</span></span>|<span data-ttu-id="8ccdb-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ccdb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8ccdb-145">supportsScopeTags</span></span>|<span data-ttu-id="8ccdb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ccdb-146">Boolean</span></span>|<span data-ttu-id="8ccdb-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ccdb-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ccdb-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ccdb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-150">This property is read-only.</span></span> <span data-ttu-id="8ccdb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ccdb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8ccdb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ccdb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8ccdb-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8ccdb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ccdb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8ccdb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ccdb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8ccdb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8ccdb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ccdb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8ccdb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ccdb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8ccdb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8ccdb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ccdb-164">createdDateTime</span></span>|<span data-ttu-id="8ccdb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ccdb-165">DateTimeOffset</span></span>|<span data-ttu-id="8ccdb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-166">DateTime the object was created.</span></span> <span data-ttu-id="8ccdb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-168">description</span><span class="sxs-lookup"><span data-stu-id="8ccdb-168">description</span></span>|<span data-ttu-id="8ccdb-169">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-169">String</span></span>|<span data-ttu-id="8ccdb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ccdb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8ccdb-172">displayName</span></span>|<span data-ttu-id="8ccdb-173">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-173">String</span></span>|<span data-ttu-id="8ccdb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ccdb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-176">version</span><span class="sxs-lookup"><span data-stu-id="8ccdb-176">version</span></span>|<span data-ttu-id="8ccdb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8ccdb-177">Int32</span></span>|<span data-ttu-id="8ccdb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-178">Version of the device configuration.</span></span> <span data-ttu-id="8ccdb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="8ccdb-180">networkName</span></span>|<span data-ttu-id="8ccdb-181">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-181">String</span></span>|<span data-ttu-id="8ccdb-182">Сетевое имя, унаследованное от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-182">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-183">SSID</span><span class="sxs-lookup"><span data-stu-id="8ccdb-183">ssid</span></span>|<span data-ttu-id="8ccdb-184">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-184">String</span></span>|<span data-ttu-id="8ccdb-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="8ccdb-186">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="8ccdb-187">connectAutomatically</span></span>|<span data-ttu-id="8ccdb-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ccdb-188">Boolean</span></span>|<span data-ttu-id="8ccdb-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8ccdb-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="8ccdb-191">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-191">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="8ccdb-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8ccdb-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ccdb-193">Boolean</span></span>|<span data-ttu-id="8ccdb-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="8ccdb-195">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ccdb-195">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="8ccdb-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="8ccdb-196">wiFiSecurityType</span></span>|[<span data-ttu-id="8ccdb-197">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="8ccdb-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="8ccdb-198">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8ccdb-199">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-199">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="8ccdb-200">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="8ccdb-201">еаптипе</span><span class="sxs-lookup"><span data-stu-id="8ccdb-201">eapType</span></span>|[<span data-ttu-id="8ccdb-202">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="8ccdb-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="8ccdb-203">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="8ccdb-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="8ccdb-204">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="8ccdb-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="8ccdb-205">authenticationMethod</span></span>|[<span data-ttu-id="8ccdb-206">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="8ccdb-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="8ccdb-207">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="8ccdb-208">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="8ccdb-209">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="8ccdb-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="8ccdb-210">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="8ccdb-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="8ccdb-211">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="8ccdb-212">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="8ccdb-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="8ccdb-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="8ccdb-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="8ccdb-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="8ccdb-215">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="8ccdb-216">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="8ccdb-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="8ccdb-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="8ccdb-218">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-218">String</span></span>|<span data-ttu-id="8ccdb-219">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="8ccdb-220">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="8ccdb-221">усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="8ccdb-221">usernameFormatString</span></span>|<span data-ttu-id="8ccdb-222">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-222">String</span></span>|<span data-ttu-id="8ccdb-223">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="8ccdb-223">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="8ccdb-224">пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="8ccdb-224">passwordFormatString</span></span>|<span data-ttu-id="8ccdb-225">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-225">String</span></span>|<span data-ttu-id="8ccdb-226">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="8ccdb-226">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="8ccdb-227">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="8ccdb-227">preSharedKey</span></span>|<span data-ttu-id="8ccdb-228">String</span><span class="sxs-lookup"><span data-stu-id="8ccdb-228">String</span></span>|<span data-ttu-id="8ccdb-229">PreSharedKey, используемый для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="8ccdb-229">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="8ccdb-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ccdb-230">Response</span></span>
<span data-ttu-id="8ccdb-231">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-231">If successful, this method returns a `200 OK` response code and an updated [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ccdb-232">Пример</span><span class="sxs-lookup"><span data-stu-id="8ccdb-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ccdb-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ccdb-233">Request</span></span>
<span data-ttu-id="8ccdb-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1699

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="8ccdb-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ccdb-235">Response</span></span>
<span data-ttu-id="8ccdb-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ccdb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1871

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```






