---
title: Обновление androidForWorkEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidForWorkEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45206bae46d805fc234a989d97e47b0c27a52b7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49239164"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="82cea-103">Обновление androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="82cea-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="82cea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82cea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82cea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82cea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82cea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82cea-107">Обновление свойств объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82cea-107">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82cea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82cea-108">Prerequisites</span></span>
<span data-ttu-id="82cea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82cea-111">Permission type</span></span>|<span data-ttu-id="82cea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82cea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82cea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82cea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82cea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82cea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82cea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82cea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82cea-116">Not supported.</span></span>|
|<span data-ttu-id="82cea-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="82cea-117">Application</span></span>|<span data-ttu-id="82cea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82cea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82cea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82cea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82cea-120">Request headers</span></span>
|<span data-ttu-id="82cea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82cea-121">Header</span></span>|<span data-ttu-id="82cea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82cea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82cea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82cea-123">Authorization</span></span>|<span data-ttu-id="82cea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82cea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82cea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82cea-125">Accept</span></span>|<span data-ttu-id="82cea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82cea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82cea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82cea-127">Request body</span></span>
<span data-ttu-id="82cea-128">В тексте запроса добавьте представление объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82cea-128">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="82cea-129">В следующей таблице приведены свойства, необходимые при создании [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-129">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="82cea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="82cea-130">Property</span></span>|<span data-ttu-id="82cea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="82cea-131">Type</span></span>|<span data-ttu-id="82cea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="82cea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82cea-133">id</span><span class="sxs-lookup"><span data-stu-id="82cea-133">id</span></span>|<span data-ttu-id="82cea-134">String</span><span class="sxs-lookup"><span data-stu-id="82cea-134">String</span></span>|<span data-ttu-id="82cea-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82cea-135">Key of the entity.</span></span> <span data-ttu-id="82cea-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82cea-137">lastModifiedDateTime</span></span>|<span data-ttu-id="82cea-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82cea-138">DateTimeOffset</span></span>|<span data-ttu-id="82cea-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82cea-139">DateTime the object was last modified.</span></span> <span data-ttu-id="82cea-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82cea-141">roleScopeTagIds</span></span>|<span data-ttu-id="82cea-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="82cea-142">String collection</span></span>|<span data-ttu-id="82cea-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="82cea-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82cea-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="82cea-145">supportsScopeTags</span></span>|<span data-ttu-id="82cea-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="82cea-146">Boolean</span></span>|<span data-ttu-id="82cea-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="82cea-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82cea-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="82cea-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82cea-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="82cea-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82cea-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82cea-150">This property is read-only.</span></span> <span data-ttu-id="82cea-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="82cea-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="82cea-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="82cea-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="82cea-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="82cea-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="82cea-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="82cea-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="82cea-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="82cea-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="82cea-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="82cea-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="82cea-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="82cea-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="82cea-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="82cea-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="82cea-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="82cea-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="82cea-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82cea-164">createdDateTime</span></span>|<span data-ttu-id="82cea-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82cea-165">DateTimeOffset</span></span>|<span data-ttu-id="82cea-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="82cea-166">DateTime the object was created.</span></span> <span data-ttu-id="82cea-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-168">description</span><span class="sxs-lookup"><span data-stu-id="82cea-168">description</span></span>|<span data-ttu-id="82cea-169">String</span><span class="sxs-lookup"><span data-stu-id="82cea-169">String</span></span>|<span data-ttu-id="82cea-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82cea-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82cea-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-172">displayName</span><span class="sxs-lookup"><span data-stu-id="82cea-172">displayName</span></span>|<span data-ttu-id="82cea-173">String</span><span class="sxs-lookup"><span data-stu-id="82cea-173">String</span></span>|<span data-ttu-id="82cea-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82cea-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82cea-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-176">version</span><span class="sxs-lookup"><span data-stu-id="82cea-176">version</span></span>|<span data-ttu-id="82cea-177">Int32</span><span class="sxs-lookup"><span data-stu-id="82cea-177">Int32</span></span>|<span data-ttu-id="82cea-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82cea-178">Version of the device configuration.</span></span> <span data-ttu-id="82cea-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82cea-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="82cea-180">networkName</span></span>|<span data-ttu-id="82cea-181">String</span><span class="sxs-lookup"><span data-stu-id="82cea-181">String</span></span>|<span data-ttu-id="82cea-182">Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82cea-182">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="82cea-183">SSID</span><span class="sxs-lookup"><span data-stu-id="82cea-183">ssid</span></span>|<span data-ttu-id="82cea-184">String</span><span class="sxs-lookup"><span data-stu-id="82cea-184">String</span></span>|<span data-ttu-id="82cea-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="82cea-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="82cea-186">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82cea-186">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="82cea-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="82cea-187">connectAutomatically</span></span>|<span data-ttu-id="82cea-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="82cea-188">Boolean</span></span>|<span data-ttu-id="82cea-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="82cea-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="82cea-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="82cea-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="82cea-191">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82cea-191">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="82cea-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="82cea-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="82cea-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="82cea-193">Boolean</span></span>|<span data-ttu-id="82cea-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="82cea-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="82cea-195">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82cea-195">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="82cea-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="82cea-196">wiFiSecurityType</span></span>|[<span data-ttu-id="82cea-197">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="82cea-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="82cea-198">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="82cea-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="82cea-199">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82cea-199">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="82cea-200">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="82cea-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="82cea-201">еаптипе</span><span class="sxs-lookup"><span data-stu-id="82cea-201">eapType</span></span>|[<span data-ttu-id="82cea-202">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="82cea-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="82cea-203">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="82cea-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="82cea-204">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="82cea-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="82cea-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="82cea-205">authenticationMethod</span></span>|[<span data-ttu-id="82cea-206">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="82cea-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="82cea-207">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="82cea-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="82cea-208">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="82cea-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="82cea-209">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="82cea-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="82cea-210">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="82cea-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="82cea-211">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="82cea-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="82cea-212">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="82cea-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="82cea-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="82cea-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="82cea-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="82cea-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="82cea-215">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="82cea-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="82cea-216">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="82cea-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="82cea-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="82cea-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="82cea-218">String</span><span class="sxs-lookup"><span data-stu-id="82cea-218">String</span></span>|<span data-ttu-id="82cea-219">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="82cea-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="82cea-220">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="82cea-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="82cea-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="82cea-221">Response</span></span>
<span data-ttu-id="82cea-222">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82cea-222">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82cea-223">Пример</span><span class="sxs-lookup"><span data-stu-id="82cea-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="82cea-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="82cea-224">Request</span></span>
<span data-ttu-id="82cea-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82cea-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82cea-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="82cea-226">Response</span></span>
<span data-ttu-id="82cea-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82cea-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




