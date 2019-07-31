---
title: Обновление androidForWorkEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidForWorkEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6706c637a625e07f69fd5db5cc4846af3cf7e03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963677"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="33b1f-103">Обновление androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="33b1f-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="33b1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33b1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33b1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33b1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b1f-106">Обновление свойств объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="33b1f-106">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33b1f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33b1f-107">Prerequisites</span></span>
<span data-ttu-id="33b1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33b1f-110">Permission type</span></span>|<span data-ttu-id="33b1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33b1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33b1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33b1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33b1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33b1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33b1f-115">Not supported.</span></span>|
|<span data-ttu-id="33b1f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33b1f-116">Application</span></span>|<span data-ttu-id="33b1f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33b1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b1f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33b1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33b1f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33b1f-119">Request headers</span></span>
|<span data-ttu-id="33b1f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33b1f-120">Header</span></span>|<span data-ttu-id="33b1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33b1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33b1f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33b1f-122">Authorization</span></span>|<span data-ttu-id="33b1f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33b1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33b1f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33b1f-124">Accept</span></span>|<span data-ttu-id="33b1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33b1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b1f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33b1f-126">Request body</span></span>
<span data-ttu-id="33b1f-127">В тексте запроса добавьте представление объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33b1f-127">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="33b1f-128">В следующей таблице приведены свойства, необходимые при создании [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-128">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="33b1f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="33b1f-129">Property</span></span>|<span data-ttu-id="33b1f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="33b1f-130">Type</span></span>|<span data-ttu-id="33b1f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="33b1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b1f-132">id</span><span class="sxs-lookup"><span data-stu-id="33b1f-132">id</span></span>|<span data-ttu-id="33b1f-133">String</span><span class="sxs-lookup"><span data-stu-id="33b1f-133">String</span></span>|<span data-ttu-id="33b1f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33b1f-134">Key of the entity.</span></span> <span data-ttu-id="33b1f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33b1f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33b1f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b1f-137">DateTimeOffset</span></span>|<span data-ttu-id="33b1f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33b1f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33b1f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33b1f-140">roleScopeTagIds</span></span>|<span data-ttu-id="33b1f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33b1f-141">String collection</span></span>|<span data-ttu-id="33b1f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="33b1f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33b1f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="33b1f-144">supportsScopeTags</span></span>|<span data-ttu-id="33b1f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="33b1f-145">Boolean</span></span>|<span data-ttu-id="33b1f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="33b1f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33b1f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="33b1f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33b1f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="33b1f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33b1f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33b1f-149">This property is read-only.</span></span> <span data-ttu-id="33b1f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="33b1f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="33b1f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="33b1f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="33b1f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33b1f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="33b1f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="33b1f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="33b1f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="33b1f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="33b1f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33b1f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="33b1f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="33b1f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="33b1f-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="33b1f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="33b1f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33b1f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="33b1f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33b1f-163">createdDateTime</span></span>|<span data-ttu-id="33b1f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b1f-164">DateTimeOffset</span></span>|<span data-ttu-id="33b1f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33b1f-165">DateTime the object was created.</span></span> <span data-ttu-id="33b1f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-167">description</span><span class="sxs-lookup"><span data-stu-id="33b1f-167">description</span></span>|<span data-ttu-id="33b1f-168">String</span><span class="sxs-lookup"><span data-stu-id="33b1f-168">String</span></span>|<span data-ttu-id="33b1f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33b1f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33b1f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="33b1f-171">displayName</span></span>|<span data-ttu-id="33b1f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="33b1f-172">String</span></span>|<span data-ttu-id="33b1f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33b1f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33b1f-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-175">version</span><span class="sxs-lookup"><span data-stu-id="33b1f-175">version</span></span>|<span data-ttu-id="33b1f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="33b1f-176">Int32</span></span>|<span data-ttu-id="33b1f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33b1f-177">Version of the device configuration.</span></span> <span data-ttu-id="33b1f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-179">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="33b1f-179">networkName</span></span>|<span data-ttu-id="33b1f-180">String</span><span class="sxs-lookup"><span data-stu-id="33b1f-180">String</span></span>|<span data-ttu-id="33b1f-181">Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33b1f-181">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-182">SSID</span><span class="sxs-lookup"><span data-stu-id="33b1f-182">ssid</span></span>|<span data-ttu-id="33b1f-183">String</span><span class="sxs-lookup"><span data-stu-id="33b1f-183">String</span></span>|<span data-ttu-id="33b1f-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="33b1f-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="33b1f-185">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33b1f-185">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-186">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="33b1f-186">connectAutomatically</span></span>|<span data-ttu-id="33b1f-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="33b1f-187">Boolean</span></span>|<span data-ttu-id="33b1f-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="33b1f-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="33b1f-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="33b1f-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="33b1f-190">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33b1f-190">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-191">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="33b1f-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="33b1f-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="33b1f-192">Boolean</span></span>|<span data-ttu-id="33b1f-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="33b1f-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="33b1f-194">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33b1f-194">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="33b1f-195">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="33b1f-195">wiFiSecurityType</span></span>|[<span data-ttu-id="33b1f-196">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="33b1f-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="33b1f-197">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="33b1f-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="33b1f-198">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33b1f-198">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="33b1f-199">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="33b1f-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="33b1f-200">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="33b1f-200">eapType</span></span>|[<span data-ttu-id="33b1f-201">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="33b1f-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="33b1f-202">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="33b1f-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="33b1f-203">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="33b1f-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="33b1f-204">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="33b1f-204">authenticationMethod</span></span>|[<span data-ttu-id="33b1f-205">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="33b1f-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="33b1f-206">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="33b1f-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="33b1f-207">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="33b1f-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="33b1f-208">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="33b1f-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="33b1f-209">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="33b1f-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="33b1f-210">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="33b1f-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="33b1f-211">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="33b1f-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="33b1f-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="33b1f-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="33b1f-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="33b1f-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="33b1f-214">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="33b1f-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="33b1f-215">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="33b1f-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="33b1f-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="33b1f-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="33b1f-217">String</span><span class="sxs-lookup"><span data-stu-id="33b1f-217">String</span></span>|<span data-ttu-id="33b1f-218">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="33b1f-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="33b1f-219">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="33b1f-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="33b1f-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b1f-220">Response</span></span>
<span data-ttu-id="33b1f-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33b1f-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b1f-222">Пример</span><span class="sxs-lookup"><span data-stu-id="33b1f-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="33b1f-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="33b1f-223">Request</span></span>
<span data-ttu-id="33b1f-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33b1f-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="33b1f-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b1f-225">Response</span></span>
<span data-ttu-id="33b1f-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33b1f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





