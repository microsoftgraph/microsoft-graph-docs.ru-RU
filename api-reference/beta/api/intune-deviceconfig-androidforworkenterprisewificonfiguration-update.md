---
title: Обновление androidForWorkEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidForWorkEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a25d37e72afbfbe090b316fe459b70f708807d2a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970879"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="6b3e1-103">Обновление androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b3e1-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="6b3e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b3e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b3e1-106">Обновление свойств объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6b3e1-106">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b3e1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b3e1-107">Prerequisites</span></span>
<span data-ttu-id="6b3e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b3e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b3e1-110">Permission type</span></span>|<span data-ttu-id="6b3e1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b3e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b3e1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b3e1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b3e1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b3e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-115">Not supported.</span></span>|
|<span data-ttu-id="6b3e1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b3e1-116">Application</span></span>|<span data-ttu-id="6b3e1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b3e1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b3e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6b3e1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b3e1-119">Request headers</span></span>
|<span data-ttu-id="6b3e1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b3e1-120">Header</span></span>|<span data-ttu-id="6b3e1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b3e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b3e1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b3e1-122">Authorization</span></span>|<span data-ttu-id="6b3e1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b3e1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6b3e1-124">Accept</span></span>|<span data-ttu-id="6b3e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b3e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b3e1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6b3e1-126">Request body</span></span>
<span data-ttu-id="6b3e1-127">В тексте запроса добавьте представление объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-127">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="6b3e1-128">В следующей таблице приведены свойства, необходимые при создании [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-128">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="6b3e1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b3e1-129">Property</span></span>|<span data-ttu-id="6b3e1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b3e1-130">Type</span></span>|<span data-ttu-id="6b3e1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b3e1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b3e1-132">id</span><span class="sxs-lookup"><span data-stu-id="6b3e1-132">id</span></span>|<span data-ttu-id="6b3e1-133">String</span><span class="sxs-lookup"><span data-stu-id="6b3e1-133">String</span></span>|<span data-ttu-id="6b3e1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-134">Key of the entity.</span></span> <span data-ttu-id="6b3e1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b3e1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6b3e1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b3e1-137">DateTimeOffset</span></span>|<span data-ttu-id="6b3e1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6b3e1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b3e1-140">roleScopeTagIds</span></span>|<span data-ttu-id="6b3e1-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6b3e1-141">String collection</span></span>|<span data-ttu-id="6b3e1-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b3e1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6b3e1-144">supportsScopeTags</span></span>|<span data-ttu-id="6b3e1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b3e1-145">Boolean</span></span>|<span data-ttu-id="6b3e1-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b3e1-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b3e1-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b3e1-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-149">This property is read-only.</span></span> <span data-ttu-id="6b3e1-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6b3e1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6b3e1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6b3e1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6b3e1-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6b3e1-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6b3e1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6b3e1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6b3e1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6b3e1-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6b3e1-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="6b3e1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6b3e1-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="6b3e1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6b3e1-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6b3e1-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b3e1-163">createdDateTime</span></span>|<span data-ttu-id="6b3e1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b3e1-164">DateTimeOffset</span></span>|<span data-ttu-id="6b3e1-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-165">DateTime the object was created.</span></span> <span data-ttu-id="6b3e1-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-167">description</span><span class="sxs-lookup"><span data-stu-id="6b3e1-167">description</span></span>|<span data-ttu-id="6b3e1-168">String</span><span class="sxs-lookup"><span data-stu-id="6b3e1-168">String</span></span>|<span data-ttu-id="6b3e1-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b3e1-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6b3e1-171">displayName</span></span>|<span data-ttu-id="6b3e1-172">Строка</span><span class="sxs-lookup"><span data-stu-id="6b3e1-172">String</span></span>|<span data-ttu-id="6b3e1-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b3e1-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-175">version</span><span class="sxs-lookup"><span data-stu-id="6b3e1-175">version</span></span>|<span data-ttu-id="6b3e1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6b3e1-176">Int32</span></span>|<span data-ttu-id="6b3e1-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-177">Version of the device configuration.</span></span> <span data-ttu-id="6b3e1-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-179">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="6b3e1-179">networkName</span></span>|<span data-ttu-id="6b3e1-180">String</span><span class="sxs-lookup"><span data-stu-id="6b3e1-180">String</span></span>|<span data-ttu-id="6b3e1-181">Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-181">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-182">SSID</span><span class="sxs-lookup"><span data-stu-id="6b3e1-182">ssid</span></span>|<span data-ttu-id="6b3e1-183">String</span><span class="sxs-lookup"><span data-stu-id="6b3e1-183">String</span></span>|<span data-ttu-id="6b3e1-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6b3e1-185">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-185">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-186">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="6b3e1-186">connectAutomatically</span></span>|<span data-ttu-id="6b3e1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b3e1-187">Boolean</span></span>|<span data-ttu-id="6b3e1-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6b3e1-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6b3e1-190">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-190">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-191">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="6b3e1-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6b3e1-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b3e1-192">Boolean</span></span>|<span data-ttu-id="6b3e1-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6b3e1-194">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b3e1-194">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="6b3e1-195">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="6b3e1-195">wiFiSecurityType</span></span>|[<span data-ttu-id="6b3e1-196">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="6b3e1-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="6b3e1-197">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6b3e1-198">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-198">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="6b3e1-199">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="6b3e1-200">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="6b3e1-200">eapType</span></span>|[<span data-ttu-id="6b3e1-201">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="6b3e1-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="6b3e1-202">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="6b3e1-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6b3e1-203">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="6b3e1-204">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6b3e1-204">authenticationMethod</span></span>|[<span data-ttu-id="6b3e1-205">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="6b3e1-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6b3e1-206">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6b3e1-207">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6b3e1-208">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="6b3e1-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6b3e1-209">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="6b3e1-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6b3e1-210">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6b3e1-211">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6b3e1-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="6b3e1-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="6b3e1-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="6b3e1-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="6b3e1-214">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6b3e1-215">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6b3e1-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6b3e1-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6b3e1-217">String</span><span class="sxs-lookup"><span data-stu-id="6b3e1-217">String</span></span>|<span data-ttu-id="6b3e1-218">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="6b3e1-219">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="6b3e1-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b3e1-220">Response</span></span>
<span data-ttu-id="6b3e1-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b3e1-222">Пример</span><span class="sxs-lookup"><span data-stu-id="6b3e1-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b3e1-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b3e1-223">Request</span></span>
<span data-ttu-id="6b3e1-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b3e1-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b3e1-225">Response</span></span>
<span data-ttu-id="6b3e1-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b3e1-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





