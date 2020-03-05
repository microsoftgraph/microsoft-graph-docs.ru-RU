---
title: Обновление androidForWorkEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidForWorkEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86bb332132ee273fe3268d59d8e958e2238cdd8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443897"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="cf80e-103">Обновление androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf80e-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="cf80e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cf80e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf80e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf80e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf80e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf80e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf80e-107">Обновление свойств объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cf80e-107">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf80e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf80e-108">Prerequisites</span></span>
<span data-ttu-id="cf80e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf80e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf80e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf80e-111">Permission type</span></span>|<span data-ttu-id="cf80e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf80e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf80e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf80e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf80e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf80e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf80e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf80e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf80e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf80e-116">Not supported.</span></span>|
|<span data-ttu-id="cf80e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf80e-117">Application</span></span>|<span data-ttu-id="cf80e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf80e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf80e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf80e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cf80e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf80e-120">Request headers</span></span>
|<span data-ttu-id="cf80e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf80e-121">Header</span></span>|<span data-ttu-id="cf80e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf80e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf80e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf80e-123">Authorization</span></span>|<span data-ttu-id="cf80e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf80e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf80e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf80e-125">Accept</span></span>|<span data-ttu-id="cf80e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf80e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf80e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf80e-127">Request body</span></span>
<span data-ttu-id="cf80e-128">В тексте запроса добавьте представление объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf80e-128">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="cf80e-129">В следующей таблице приведены свойства, необходимые при создании [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-129">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="cf80e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf80e-130">Property</span></span>|<span data-ttu-id="cf80e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf80e-131">Type</span></span>|<span data-ttu-id="cf80e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf80e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf80e-133">id</span><span class="sxs-lookup"><span data-stu-id="cf80e-133">id</span></span>|<span data-ttu-id="cf80e-134">String</span><span class="sxs-lookup"><span data-stu-id="cf80e-134">String</span></span>|<span data-ttu-id="cf80e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cf80e-135">Key of the entity.</span></span> <span data-ttu-id="cf80e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf80e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cf80e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf80e-138">DateTimeOffset</span></span>|<span data-ttu-id="cf80e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cf80e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cf80e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf80e-141">roleScopeTagIds</span></span>|<span data-ttu-id="cf80e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf80e-142">String collection</span></span>|<span data-ttu-id="cf80e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cf80e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cf80e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cf80e-145">supportsScopeTags</span></span>|<span data-ttu-id="cf80e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="cf80e-146">Boolean</span></span>|<span data-ttu-id="cf80e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cf80e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cf80e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cf80e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cf80e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cf80e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cf80e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf80e-150">This property is read-only.</span></span> <span data-ttu-id="cf80e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cf80e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cf80e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cf80e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cf80e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cf80e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cf80e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cf80e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cf80e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cf80e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cf80e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cf80e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cf80e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cf80e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cf80e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cf80e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cf80e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cf80e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cf80e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf80e-164">createdDateTime</span></span>|<span data-ttu-id="cf80e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf80e-165">DateTimeOffset</span></span>|<span data-ttu-id="cf80e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cf80e-166">DateTime the object was created.</span></span> <span data-ttu-id="cf80e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-168">description</span><span class="sxs-lookup"><span data-stu-id="cf80e-168">description</span></span>|<span data-ttu-id="cf80e-169">String</span><span class="sxs-lookup"><span data-stu-id="cf80e-169">String</span></span>|<span data-ttu-id="cf80e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf80e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf80e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="cf80e-172">displayName</span></span>|<span data-ttu-id="cf80e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="cf80e-173">String</span></span>|<span data-ttu-id="cf80e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf80e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf80e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-176">version</span><span class="sxs-lookup"><span data-stu-id="cf80e-176">version</span></span>|<span data-ttu-id="cf80e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cf80e-177">Int32</span></span>|<span data-ttu-id="cf80e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf80e-178">Version of the device configuration.</span></span> <span data-ttu-id="cf80e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="cf80e-180">networkName</span></span>|<span data-ttu-id="cf80e-181">String</span><span class="sxs-lookup"><span data-stu-id="cf80e-181">String</span></span>|<span data-ttu-id="cf80e-182">Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf80e-182">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-183">SSID</span><span class="sxs-lookup"><span data-stu-id="cf80e-183">ssid</span></span>|<span data-ttu-id="cf80e-184">String</span><span class="sxs-lookup"><span data-stu-id="cf80e-184">String</span></span>|<span data-ttu-id="cf80e-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="cf80e-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="cf80e-186">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf80e-186">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="cf80e-187">connectAutomatically</span></span>|<span data-ttu-id="cf80e-188">Логический</span><span class="sxs-lookup"><span data-stu-id="cf80e-188">Boolean</span></span>|<span data-ttu-id="cf80e-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="cf80e-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="cf80e-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="cf80e-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="cf80e-191">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf80e-191">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="cf80e-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="cf80e-193">Логический</span><span class="sxs-lookup"><span data-stu-id="cf80e-193">Boolean</span></span>|<span data-ttu-id="cf80e-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="cf80e-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="cf80e-195">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf80e-195">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="cf80e-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="cf80e-196">wiFiSecurityType</span></span>|[<span data-ttu-id="cf80e-197">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="cf80e-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="cf80e-198">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="cf80e-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="cf80e-199">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf80e-199">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="cf80e-200">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="cf80e-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="cf80e-201">еаптипе</span><span class="sxs-lookup"><span data-stu-id="cf80e-201">eapType</span></span>|[<span data-ttu-id="cf80e-202">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="cf80e-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="cf80e-203">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="cf80e-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="cf80e-204">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="cf80e-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="cf80e-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="cf80e-205">authenticationMethod</span></span>|[<span data-ttu-id="cf80e-206">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="cf80e-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="cf80e-207">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="cf80e-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="cf80e-208">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="cf80e-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="cf80e-209">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="cf80e-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="cf80e-210">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="cf80e-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="cf80e-211">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="cf80e-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="cf80e-212">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="cf80e-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="cf80e-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="cf80e-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="cf80e-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="cf80e-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="cf80e-215">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="cf80e-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="cf80e-216">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="cf80e-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="cf80e-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="cf80e-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="cf80e-218">String</span><span class="sxs-lookup"><span data-stu-id="cf80e-218">String</span></span>|<span data-ttu-id="cf80e-219">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="cf80e-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="cf80e-220">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="cf80e-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="cf80e-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf80e-221">Response</span></span>
<span data-ttu-id="cf80e-222">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf80e-222">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf80e-223">Пример</span><span class="sxs-lookup"><span data-stu-id="cf80e-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf80e-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf80e-224">Request</span></span>
<span data-ttu-id="cf80e-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf80e-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="cf80e-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf80e-226">Response</span></span>
<span data-ttu-id="cf80e-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf80e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1717

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





