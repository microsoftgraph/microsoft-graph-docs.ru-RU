---
title: Обновление Виндовсделиверйоптимизатионконфигуратион
description: Обновление свойств объекта Виндовсделиверйоптимизатионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e51eea388dff37672a6291c8219a4c141bfb595
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186815"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="562e9-103">Обновление Виндовсделиверйоптимизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="562e9-103">Update windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="562e9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="562e9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="562e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="562e9-106">Обновление свойств объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="562e9-106">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="562e9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="562e9-107">Prerequisites</span></span>
<span data-ttu-id="562e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="562e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="562e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="562e9-110">Permission type</span></span>|<span data-ttu-id="562e9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="562e9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="562e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="562e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="562e9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="562e9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="562e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="562e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="562e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562e9-115">Not supported.</span></span>|
|<span data-ttu-id="562e9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="562e9-116">Application</span></span>|<span data-ttu-id="562e9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="562e9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="562e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="562e9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="562e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="562e9-119">Request headers</span></span>
|<span data-ttu-id="562e9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="562e9-120">Header</span></span>|<span data-ttu-id="562e9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="562e9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="562e9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="562e9-122">Authorization</span></span>|<span data-ttu-id="562e9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562e9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="562e9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="562e9-124">Accept</span></span>|<span data-ttu-id="562e9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="562e9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="562e9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="562e9-126">Request body</span></span>
<span data-ttu-id="562e9-127">В тексте запроса добавьте представление объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="562e9-127">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="562e9-128">В следующей таблице приведены свойства, необходимые при создании [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-128">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="562e9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="562e9-129">Property</span></span>|<span data-ttu-id="562e9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="562e9-130">Type</span></span>|<span data-ttu-id="562e9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="562e9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="562e9-132">id</span><span class="sxs-lookup"><span data-stu-id="562e9-132">id</span></span>|<span data-ttu-id="562e9-133">String</span><span class="sxs-lookup"><span data-stu-id="562e9-133">String</span></span>|<span data-ttu-id="562e9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="562e9-134">Key of the entity.</span></span> <span data-ttu-id="562e9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="562e9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="562e9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="562e9-137">DateTimeOffset</span></span>|<span data-ttu-id="562e9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="562e9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="562e9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="562e9-140">roleScopeTagIds</span></span>|<span data-ttu-id="562e9-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="562e9-141">String collection</span></span>|<span data-ttu-id="562e9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="562e9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="562e9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="562e9-144">supportsScopeTags</span></span>|<span data-ttu-id="562e9-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="562e9-145">Boolean</span></span>|<span data-ttu-id="562e9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="562e9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="562e9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="562e9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="562e9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="562e9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="562e9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="562e9-149">This property is read-only.</span></span> <span data-ttu-id="562e9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="562e9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="562e9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="562e9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="562e9-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="562e9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="562e9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="562e9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="562e9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="562e9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="562e9-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="562e9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="562e9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="562e9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="562e9-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="562e9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="562e9-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="562e9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="562e9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="562e9-163">createdDateTime</span></span>|<span data-ttu-id="562e9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="562e9-164">DateTimeOffset</span></span>|<span data-ttu-id="562e9-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="562e9-165">DateTime the object was created.</span></span> <span data-ttu-id="562e9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-167">description</span><span class="sxs-lookup"><span data-stu-id="562e9-167">description</span></span>|<span data-ttu-id="562e9-168">String</span><span class="sxs-lookup"><span data-stu-id="562e9-168">String</span></span>|<span data-ttu-id="562e9-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="562e9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="562e9-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="562e9-171">displayName</span></span>|<span data-ttu-id="562e9-172">Строка</span><span class="sxs-lookup"><span data-stu-id="562e9-172">String</span></span>|<span data-ttu-id="562e9-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="562e9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="562e9-174">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="562e9-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-175">version</span><span class="sxs-lookup"><span data-stu-id="562e9-175">version</span></span>|<span data-ttu-id="562e9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-176">Int32</span></span>|<span data-ttu-id="562e9-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="562e9-177">Version of the device configuration.</span></span> <span data-ttu-id="562e9-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="562e9-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="562e9-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="562e9-180">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="562e9-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="562e9-181">Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента.</span><span class="sxs-lookup"><span data-stu-id="562e9-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="562e9-182">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="562e9-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="562e9-183">рестриктпирселектионби</span><span class="sxs-lookup"><span data-stu-id="562e9-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="562e9-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="562e9-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="562e9-185">Задает ограничение выбора однорангового узла с помощью выбранного параметра.</span><span class="sxs-lookup"><span data-stu-id="562e9-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="562e9-186">Вариант 1 (маска подсети) применяется только к режимам оптимизации доставки LAN (1) и Group (2).</span><span class="sxs-lookup"><span data-stu-id="562e9-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="562e9-187">Возможные значения: `notConfigured`, `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="562e9-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="562e9-188">граупидсаурце</span><span class="sxs-lookup"><span data-stu-id="562e9-188">groupIdSource</span></span>|[<span data-ttu-id="562e9-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="562e9-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="562e9-190">Задает ограничение выбора однорангового узла для источника получать.</span><span class="sxs-lookup"><span data-stu-id="562e9-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="562e9-191">Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2).</span><span class="sxs-lookup"><span data-stu-id="562e9-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="562e9-192">Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="562e9-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="562e9-193">Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="562e9-194">бандвидсмоде</span><span class="sxs-lookup"><span data-stu-id="562e9-194">bandwidthMode</span></span>|[<span data-ttu-id="562e9-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="562e9-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="562e9-196">Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.</span><span class="sxs-lookup"><span data-stu-id="562e9-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="562e9-197">баккграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="562e9-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="562e9-198">Int64</span><span class="sxs-lookup"><span data-stu-id="562e9-198">Int64</span></span>|<span data-ttu-id="562e9-199">Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения.</span><span class="sxs-lookup"><span data-stu-id="562e9-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="562e9-200">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="562e9-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="562e9-201">фореграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="562e9-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="562e9-202">Int64</span><span class="sxs-lookup"><span data-stu-id="562e9-202">Int64</span></span>|<span data-ttu-id="562e9-203">Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400).</span><span class="sxs-lookup"><span data-stu-id="562e9-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="562e9-204">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="562e9-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="562e9-205">Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы.</span><span class="sxs-lookup"><span data-stu-id="562e9-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="562e9-206">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="562e9-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="562e9-207">минимумрамалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="562e9-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="562e9-208">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-208">Int32</span></span>|<span data-ttu-id="562e9-209">Указывает минимальный размер ОЗУ в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="562e9-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="562e9-210">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="562e9-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="562e9-211">минимумдисксизеалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="562e9-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="562e9-212">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-212">Int32</span></span>|<span data-ttu-id="562e9-213">Указывает минимальный размер диска в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="562e9-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="562e9-214">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="562e9-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="562e9-215">Рекомендуемые значения: 64 ГБ до 256 ГБ.</span><span class="sxs-lookup"><span data-stu-id="562e9-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="562e9-216">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="562e9-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="562e9-217">минимумфилесизетокачеинмегабитес</span><span class="sxs-lookup"><span data-stu-id="562e9-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="562e9-218">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-218">Int32</span></span>|<span data-ttu-id="562e9-219">Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000).</span><span class="sxs-lookup"><span data-stu-id="562e9-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="562e9-220">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="562e9-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="562e9-221">Рекомендуемые значения: от 1 МБ до 100 000 МБ.</span><span class="sxs-lookup"><span data-stu-id="562e9-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="562e9-222">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="562e9-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="562e9-223">минимумбаттериперцентажеалловедтауплоад</span><span class="sxs-lookup"><span data-stu-id="562e9-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="562e9-224">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-224">Int32</span></span>|<span data-ttu-id="562e9-225">Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100).</span><span class="sxs-lookup"><span data-stu-id="562e9-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="562e9-226">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="562e9-226">Valid values 0 to 100</span></span>
<span data-ttu-id="562e9-227">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="562e9-227">The default value is 0.</span></span> <span data-ttu-id="562e9-228">Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы.</span><span class="sxs-lookup"><span data-stu-id="562e9-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="562e9-229">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="562e9-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="562e9-230">модификачелокатион</span><span class="sxs-lookup"><span data-stu-id="562e9-230">modifyCacheLocation</span></span>|<span data-ttu-id="562e9-231">String.</span><span class="sxs-lookup"><span data-stu-id="562e9-231">String</span></span>|<span data-ttu-id="562e9-232">Указывает диск, который должна использовать оптимизация доставки для своего кэша.</span><span class="sxs-lookup"><span data-stu-id="562e9-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="562e9-233">максимумкачеажеиндайс</span><span class="sxs-lookup"><span data-stu-id="562e9-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="562e9-234">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-234">Int32</span></span>|<span data-ttu-id="562e9-235">Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-3650).</span><span class="sxs-lookup"><span data-stu-id="562e9-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="562e9-236">Допустимые значения — от 0 до 3650</span><span class="sxs-lookup"><span data-stu-id="562e9-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="562e9-237">максимумкачесизе</span><span class="sxs-lookup"><span data-stu-id="562e9-237">maximumCacheSize</span></span>|[<span data-ttu-id="562e9-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="562e9-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="562e9-239">Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.</span><span class="sxs-lookup"><span data-stu-id="562e9-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="562e9-240">впнпиркачинг</span><span class="sxs-lookup"><span data-stu-id="562e9-240">vpnPeerCaching</span></span>|[<span data-ttu-id="562e9-241">Включение</span><span class="sxs-lookup"><span data-stu-id="562e9-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="562e9-242">Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети.</span><span class="sxs-lookup"><span data-stu-id="562e9-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="562e9-243">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="562e9-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="562e9-244">качесерверхостнамес</span><span class="sxs-lookup"><span data-stu-id="562e9-244">cacheServerHostNames</span></span>|<span data-ttu-id="562e9-245">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="562e9-245">String collection</span></span>|<span data-ttu-id="562e9-246">Указывает имена узлов серверов кэша.</span><span class="sxs-lookup"><span data-stu-id="562e9-246">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="562e9-247">качесерверфореграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="562e9-247">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="562e9-248">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-248">Int32</span></span>|<span data-ttu-id="562e9-249">Указывает время (в секундах), по истечении которого откладывается обратное сообщение от серверов кэша к источнику HTTP для загрузки переднего плана.</span><span class="sxs-lookup"><span data-stu-id="562e9-249">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="562e9-250">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="562e9-250">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="562e9-251">качесервербаккграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="562e9-251">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="562e9-252">Int32</span><span class="sxs-lookup"><span data-stu-id="562e9-252">Int32</span></span>|<span data-ttu-id="562e9-253">Указывает время (в секундах), по истечении которого будет возвращаться обратно от серверов кэша к источнику HTTP для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="562e9-253">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="562e9-254">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="562e9-254">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="562e9-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="562e9-255">Response</span></span>
<span data-ttu-id="562e9-256">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="562e9-256">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="562e9-257">Пример</span><span class="sxs-lookup"><span data-stu-id="562e9-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="562e9-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="562e9-258">Request</span></span>
<span data-ttu-id="562e9-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="562e9-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2039

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```

### <a name="response"></a><span data-ttu-id="562e9-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="562e9-260">Response</span></span>
<span data-ttu-id="562e9-p130">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="562e9-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2211

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
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
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```




