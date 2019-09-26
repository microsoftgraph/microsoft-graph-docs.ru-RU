---
title: Обновление Андроидворкпрофилинтерприсевификонфигуратион
description: Обновление свойств объекта Андроидворкпрофилинтерприсевификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9a5d1a840bba78e6ee20a6ee98bd0751fa7f7b9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175885"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="96164-103">Обновление Андроидворкпрофилинтерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="96164-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="96164-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96164-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96164-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96164-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96164-106">Обновление свойств объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="96164-106">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96164-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96164-107">Prerequisites</span></span>
<span data-ttu-id="96164-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96164-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96164-110">Permission type</span></span>|<span data-ttu-id="96164-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96164-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96164-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96164-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96164-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96164-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96164-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96164-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96164-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96164-115">Not supported.</span></span>|
|<span data-ttu-id="96164-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96164-116">Application</span></span>|<span data-ttu-id="96164-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96164-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96164-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96164-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="96164-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96164-119">Request headers</span></span>
|<span data-ttu-id="96164-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96164-120">Header</span></span>|<span data-ttu-id="96164-121">Значение</span><span class="sxs-lookup"><span data-stu-id="96164-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96164-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96164-122">Authorization</span></span>|<span data-ttu-id="96164-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96164-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96164-124">Accept</span><span class="sxs-lookup"><span data-stu-id="96164-124">Accept</span></span>|<span data-ttu-id="96164-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96164-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96164-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96164-126">Request body</span></span>
<span data-ttu-id="96164-127">В тексте запроса добавьте представление объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96164-127">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="96164-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-128">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="96164-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="96164-129">Property</span></span>|<span data-ttu-id="96164-130">Тип</span><span class="sxs-lookup"><span data-stu-id="96164-130">Type</span></span>|<span data-ttu-id="96164-131">Описание</span><span class="sxs-lookup"><span data-stu-id="96164-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96164-132">id</span><span class="sxs-lookup"><span data-stu-id="96164-132">id</span></span>|<span data-ttu-id="96164-133">String</span><span class="sxs-lookup"><span data-stu-id="96164-133">String</span></span>|<span data-ttu-id="96164-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96164-134">Key of the entity.</span></span> <span data-ttu-id="96164-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96164-136">lastModifiedDateTime</span></span>|<span data-ttu-id="96164-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96164-137">DateTimeOffset</span></span>|<span data-ttu-id="96164-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="96164-138">DateTime the object was last modified.</span></span> <span data-ttu-id="96164-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96164-140">roleScopeTagIds</span></span>|<span data-ttu-id="96164-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96164-141">String collection</span></span>|<span data-ttu-id="96164-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="96164-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96164-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="96164-144">supportsScopeTags</span></span>|<span data-ttu-id="96164-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96164-145">Boolean</span></span>|<span data-ttu-id="96164-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="96164-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="96164-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="96164-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="96164-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="96164-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="96164-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96164-149">This property is read-only.</span></span> <span data-ttu-id="96164-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="96164-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="96164-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="96164-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="96164-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96164-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="96164-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="96164-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="96164-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="96164-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="96164-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96164-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="96164-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="96164-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="96164-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="96164-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="96164-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96164-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="96164-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96164-163">createdDateTime</span></span>|<span data-ttu-id="96164-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96164-164">DateTimeOffset</span></span>|<span data-ttu-id="96164-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="96164-165">DateTime the object was created.</span></span> <span data-ttu-id="96164-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-167">description</span><span class="sxs-lookup"><span data-stu-id="96164-167">description</span></span>|<span data-ttu-id="96164-168">String</span><span class="sxs-lookup"><span data-stu-id="96164-168">String</span></span>|<span data-ttu-id="96164-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96164-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96164-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-171">displayName</span><span class="sxs-lookup"><span data-stu-id="96164-171">displayName</span></span>|<span data-ttu-id="96164-172">Строка</span><span class="sxs-lookup"><span data-stu-id="96164-172">String</span></span>|<span data-ttu-id="96164-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96164-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96164-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-175">version</span><span class="sxs-lookup"><span data-stu-id="96164-175">version</span></span>|<span data-ttu-id="96164-176">Int32</span><span class="sxs-lookup"><span data-stu-id="96164-176">Int32</span></span>|<span data-ttu-id="96164-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96164-177">Version of the device configuration.</span></span> <span data-ttu-id="96164-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96164-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="96164-179">networkName</span></span>|<span data-ttu-id="96164-180">String.</span><span class="sxs-lookup"><span data-stu-id="96164-180">String</span></span>|<span data-ttu-id="96164-181">Сетевое имя, унаследованное от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96164-181">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="96164-182">SSID</span><span class="sxs-lookup"><span data-stu-id="96164-182">ssid</span></span>|<span data-ttu-id="96164-183">String.</span><span class="sxs-lookup"><span data-stu-id="96164-183">String</span></span>|<span data-ttu-id="96164-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="96164-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="96164-185">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96164-185">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="96164-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="96164-186">connectAutomatically</span></span>|<span data-ttu-id="96164-187">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96164-187">Boolean</span></span>|<span data-ttu-id="96164-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="96164-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="96164-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="96164-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="96164-190">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96164-190">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="96164-191">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="96164-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="96164-192">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96164-192">Boolean</span></span>|<span data-ttu-id="96164-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="96164-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="96164-194">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96164-194">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="96164-195">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="96164-195">wiFiSecurityType</span></span>|[<span data-ttu-id="96164-196">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="96164-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="96164-197">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="96164-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="96164-198">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96164-198">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="96164-199">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="96164-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="96164-200">еаптипе</span><span class="sxs-lookup"><span data-stu-id="96164-200">eapType</span></span>|[<span data-ttu-id="96164-201">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="96164-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="96164-202">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="96164-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="96164-203">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="96164-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="96164-204">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="96164-204">authenticationMethod</span></span>|[<span data-ttu-id="96164-205">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="96164-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="96164-206">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="96164-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="96164-207">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="96164-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="96164-208">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="96164-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="96164-209">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="96164-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="96164-210">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="96164-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="96164-211">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="96164-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="96164-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="96164-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="96164-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="96164-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="96164-214">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="96164-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="96164-215">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="96164-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="96164-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="96164-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="96164-217">String.</span><span class="sxs-lookup"><span data-stu-id="96164-217">String</span></span>|<span data-ttu-id="96164-218">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="96164-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="96164-219">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="96164-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="96164-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="96164-220">Response</span></span>
<span data-ttu-id="96164-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96164-221">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96164-222">Пример</span><span class="sxs-lookup"><span data-stu-id="96164-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="96164-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="96164-223">Request</span></span>
<span data-ttu-id="96164-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96164-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1549

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="96164-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="96164-225">Response</span></span>
<span data-ttu-id="96164-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96164-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1721

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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




