---
title: Обновление androidEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8eef7c7c7fe6fa8b2ba0e04058a3f9e583e6a2f0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733205"
---
# <a name="update-androidenterprisewificonfiguration"></a><span data-ttu-id="2fc7a-103">Обновление androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fc7a-103">Update androidEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="2fc7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fc7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fc7a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fc7a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fc7a-107">Обновление свойств объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2fc7a-107">Update the properties of a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fc7a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2fc7a-108">Prerequisites</span></span>
<span data-ttu-id="2fc7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fc7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fc7a-111">Permission type</span></span>|<span data-ttu-id="2fc7a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fc7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fc7a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc7a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fc7a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fc7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-116">Not supported.</span></span>|
|<span data-ttu-id="2fc7a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fc7a-117">Application</span></span>|<span data-ttu-id="2fc7a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc7a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fc7a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fc7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2fc7a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2fc7a-120">Request headers</span></span>
|<span data-ttu-id="2fc7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fc7a-121">Header</span></span>|<span data-ttu-id="2fc7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2fc7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fc7a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fc7a-123">Authorization</span></span>|<span data-ttu-id="2fc7a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fc7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fc7a-125">Accept</span></span>|<span data-ttu-id="2fc7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fc7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fc7a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2fc7a-127">Request body</span></span>
<span data-ttu-id="2fc7a-128">В тексте запроса добавьте представление объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-128">In the request body, supply a JSON representation for the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="2fc7a-129">В следующей таблице приведены свойства, необходимые при создании [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-129">The following table shows the properties that are required when you create the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="2fc7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fc7a-130">Property</span></span>|<span data-ttu-id="2fc7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2fc7a-131">Type</span></span>|<span data-ttu-id="2fc7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2fc7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc7a-133">id</span><span class="sxs-lookup"><span data-stu-id="2fc7a-133">id</span></span>|<span data-ttu-id="2fc7a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-134">String</span></span>|<span data-ttu-id="2fc7a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-135">Key of the entity.</span></span> <span data-ttu-id="2fc7a-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc7a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2fc7a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc7a-138">DateTimeOffset</span></span>|<span data-ttu-id="2fc7a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2fc7a-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2fc7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="2fc7a-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2fc7a-142">String collection</span></span>|<span data-ttu-id="2fc7a-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2fc7a-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2fc7a-145">supportsScopeTags</span></span>|<span data-ttu-id="2fc7a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="2fc7a-146">Boolean</span></span>|<span data-ttu-id="2fc7a-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2fc7a-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2fc7a-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2fc7a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-150">This property is read-only.</span></span> <span data-ttu-id="2fc7a-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2fc7a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2fc7a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2fc7a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2fc7a-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2fc7a-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2fc7a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2fc7a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2fc7a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2fc7a-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2fc7a-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2fc7a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2fc7a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2fc7a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2fc7a-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2fc7a-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc7a-164">createdDateTime</span></span>|<span data-ttu-id="2fc7a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc7a-165">DateTimeOffset</span></span>|<span data-ttu-id="2fc7a-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-166">DateTime the object was created.</span></span> <span data-ttu-id="2fc7a-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-168">description</span><span class="sxs-lookup"><span data-stu-id="2fc7a-168">description</span></span>|<span data-ttu-id="2fc7a-169">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-169">String</span></span>|<span data-ttu-id="2fc7a-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2fc7a-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2fc7a-172">displayName</span></span>|<span data-ttu-id="2fc7a-173">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-173">String</span></span>|<span data-ttu-id="2fc7a-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2fc7a-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-176">version</span><span class="sxs-lookup"><span data-stu-id="2fc7a-176">version</span></span>|<span data-ttu-id="2fc7a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc7a-177">Int32</span></span>|<span data-ttu-id="2fc7a-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-178">Version of the device configuration.</span></span> <span data-ttu-id="2fc7a-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="2fc7a-180">networkName</span></span>|<span data-ttu-id="2fc7a-181">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-181">String</span></span>|<span data-ttu-id="2fc7a-182">Сетевое имя, унаследованное от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-182">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-183">SSID</span><span class="sxs-lookup"><span data-stu-id="2fc7a-183">ssid</span></span>|<span data-ttu-id="2fc7a-184">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-184">String</span></span>|<span data-ttu-id="2fc7a-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="2fc7a-186">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="2fc7a-187">connectAutomatically</span></span>|<span data-ttu-id="2fc7a-188">Логический</span><span class="sxs-lookup"><span data-stu-id="2fc7a-188">Boolean</span></span>|<span data-ttu-id="2fc7a-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="2fc7a-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="2fc7a-191">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-191">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="2fc7a-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2fc7a-193">Логический</span><span class="sxs-lookup"><span data-stu-id="2fc7a-193">Boolean</span></span>|<span data-ttu-id="2fc7a-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="2fc7a-195">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fc7a-195">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="2fc7a-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="2fc7a-196">wiFiSecurityType</span></span>|[<span data-ttu-id="2fc7a-197">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="2fc7a-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="2fc7a-198">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="2fc7a-199">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-199">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="2fc7a-200">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="2fc7a-201">еаптипе</span><span class="sxs-lookup"><span data-stu-id="2fc7a-201">eapType</span></span>|[<span data-ttu-id="2fc7a-202">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="2fc7a-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="2fc7a-203">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="2fc7a-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="2fc7a-204">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="2fc7a-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="2fc7a-205">authenticationMethod</span></span>|[<span data-ttu-id="2fc7a-206">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2fc7a-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="2fc7a-207">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="2fc7a-208">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2fc7a-209">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="2fc7a-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="2fc7a-210">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="2fc7a-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="2fc7a-211">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="2fc7a-212">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="2fc7a-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="2fc7a-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="2fc7a-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="2fc7a-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="2fc7a-215">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="2fc7a-216">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="2fc7a-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="2fc7a-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="2fc7a-218">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-218">String</span></span>|<span data-ttu-id="2fc7a-219">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="2fc7a-220">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="2fc7a-221">усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="2fc7a-221">usernameFormatString</span></span>|<span data-ttu-id="2fc7a-222">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-222">String</span></span>|<span data-ttu-id="2fc7a-223">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="2fc7a-223">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="2fc7a-224">пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="2fc7a-224">passwordFormatString</span></span>|<span data-ttu-id="2fc7a-225">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-225">String</span></span>|<span data-ttu-id="2fc7a-226">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="2fc7a-226">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="2fc7a-227">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="2fc7a-227">preSharedKey</span></span>|<span data-ttu-id="2fc7a-228">Строка</span><span class="sxs-lookup"><span data-stu-id="2fc7a-228">String</span></span>|<span data-ttu-id="2fc7a-229">PreSharedKey, используемый для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="2fc7a-229">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="2fc7a-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fc7a-230">Response</span></span>
<span data-ttu-id="2fc7a-231">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-231">If successful, this method returns a `200 OK` response code and an updated [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fc7a-232">Пример</span><span class="sxs-lookup"><span data-stu-id="2fc7a-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fc7a-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fc7a-233">Request</span></span>
<span data-ttu-id="2fc7a-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fc7a-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fc7a-235">Response</span></span>
<span data-ttu-id="2fc7a-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fc7a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





