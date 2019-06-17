---
title: Создание androidForWorkEnterpriseWiFiConfiguration
description: Создание нового объекта androidForWorkEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f44893984202e1ddf9baf67ef6210ae03529aae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970942"
---
# <a name="create-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="5db66-103">Создание androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="5db66-103">Create androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="5db66-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5db66-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5db66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5db66-106">Создание нового объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5db66-106">Create a new [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5db66-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5db66-107">Prerequisites</span></span>
<span data-ttu-id="5db66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5db66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5db66-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5db66-110">Permission type</span></span>|<span data-ttu-id="5db66-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5db66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5db66-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5db66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5db66-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db66-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5db66-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5db66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5db66-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db66-115">Not supported.</span></span>|
|<span data-ttu-id="5db66-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5db66-116">Application</span></span>|<span data-ttu-id="5db66-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5db66-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5db66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5db66-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5db66-119">Request headers</span></span>
|<span data-ttu-id="5db66-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5db66-120">Header</span></span>|<span data-ttu-id="5db66-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5db66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5db66-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5db66-122">Authorization</span></span>|<span data-ttu-id="5db66-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5db66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5db66-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5db66-124">Accept</span></span>|<span data-ttu-id="5db66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5db66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5db66-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5db66-126">Request body</span></span>
<span data-ttu-id="5db66-127">В тексте запроса добавьте представление объекта androidForWorkEnterpriseWiFiConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5db66-127">In the request body, supply a JSON representation for the androidForWorkEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="5db66-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5db66-128">The following table shows the properties that are required when you create the androidForWorkEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="5db66-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5db66-129">Property</span></span>|<span data-ttu-id="5db66-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5db66-130">Type</span></span>|<span data-ttu-id="5db66-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5db66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5db66-132">id</span><span class="sxs-lookup"><span data-stu-id="5db66-132">id</span></span>|<span data-ttu-id="5db66-133">String</span><span class="sxs-lookup"><span data-stu-id="5db66-133">String</span></span>|<span data-ttu-id="5db66-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5db66-134">Key of the entity.</span></span> <span data-ttu-id="5db66-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5db66-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5db66-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db66-137">DateTimeOffset</span></span>|<span data-ttu-id="5db66-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5db66-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5db66-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5db66-140">roleScopeTagIds</span></span>|<span data-ttu-id="5db66-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5db66-141">String collection</span></span>|<span data-ttu-id="5db66-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5db66-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5db66-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5db66-144">supportsScopeTags</span></span>|<span data-ttu-id="5db66-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5db66-145">Boolean</span></span>|<span data-ttu-id="5db66-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5db66-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5db66-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5db66-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5db66-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5db66-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5db66-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5db66-149">This property is read-only.</span></span> <span data-ttu-id="5db66-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5db66-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5db66-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5db66-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5db66-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5db66-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5db66-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5db66-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5db66-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5db66-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5db66-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5db66-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5db66-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="5db66-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5db66-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="5db66-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5db66-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5db66-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5db66-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5db66-163">createdDateTime</span></span>|<span data-ttu-id="5db66-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db66-164">DateTimeOffset</span></span>|<span data-ttu-id="5db66-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5db66-165">DateTime the object was created.</span></span> <span data-ttu-id="5db66-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-167">description</span><span class="sxs-lookup"><span data-stu-id="5db66-167">description</span></span>|<span data-ttu-id="5db66-168">String</span><span class="sxs-lookup"><span data-stu-id="5db66-168">String</span></span>|<span data-ttu-id="5db66-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5db66-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5db66-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5db66-171">displayName</span></span>|<span data-ttu-id="5db66-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5db66-172">String</span></span>|<span data-ttu-id="5db66-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5db66-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5db66-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-175">version</span><span class="sxs-lookup"><span data-stu-id="5db66-175">version</span></span>|<span data-ttu-id="5db66-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5db66-176">Int32</span></span>|<span data-ttu-id="5db66-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5db66-177">Version of the device configuration.</span></span> <span data-ttu-id="5db66-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5db66-179">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="5db66-179">networkName</span></span>|<span data-ttu-id="5db66-180">String</span><span class="sxs-lookup"><span data-stu-id="5db66-180">String</span></span>|<span data-ttu-id="5db66-181">Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5db66-181">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="5db66-182">SSID</span><span class="sxs-lookup"><span data-stu-id="5db66-182">ssid</span></span>|<span data-ttu-id="5db66-183">String</span><span class="sxs-lookup"><span data-stu-id="5db66-183">String</span></span>|<span data-ttu-id="5db66-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="5db66-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="5db66-185">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5db66-185">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="5db66-186">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="5db66-186">connectAutomatically</span></span>|<span data-ttu-id="5db66-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5db66-187">Boolean</span></span>|<span data-ttu-id="5db66-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="5db66-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="5db66-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="5db66-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="5db66-190">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5db66-190">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="5db66-191">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="5db66-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="5db66-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5db66-192">Boolean</span></span>|<span data-ttu-id="5db66-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="5db66-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="5db66-194">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5db66-194">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="5db66-195">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="5db66-195">wiFiSecurityType</span></span>|[<span data-ttu-id="5db66-196">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="5db66-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="5db66-197">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="5db66-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="5db66-198">Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5db66-198">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="5db66-199">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="5db66-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="5db66-200">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="5db66-200">eapType</span></span>|[<span data-ttu-id="5db66-201">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="5db66-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="5db66-202">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="5db66-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="5db66-203">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="5db66-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="5db66-204">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="5db66-204">authenticationMethod</span></span>|[<span data-ttu-id="5db66-205">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="5db66-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="5db66-206">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="5db66-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="5db66-207">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="5db66-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="5db66-208">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="5db66-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="5db66-209">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="5db66-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="5db66-210">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="5db66-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="5db66-211">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="5db66-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="5db66-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="5db66-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="5db66-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="5db66-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="5db66-214">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="5db66-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="5db66-215">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="5db66-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="5db66-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="5db66-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="5db66-217">String</span><span class="sxs-lookup"><span data-stu-id="5db66-217">String</span></span>|<span data-ttu-id="5db66-218">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="5db66-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="5db66-219">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="5db66-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="5db66-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db66-220">Response</span></span>
<span data-ttu-id="5db66-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5db66-221">If successful, this method returns a `201 Created` response code and a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db66-222">Пример</span><span class="sxs-lookup"><span data-stu-id="5db66-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="5db66-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="5db66-223">Request</span></span>
<span data-ttu-id="5db66-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5db66-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="5db66-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db66-225">Response</span></span>
<span data-ttu-id="5db66-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5db66-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





