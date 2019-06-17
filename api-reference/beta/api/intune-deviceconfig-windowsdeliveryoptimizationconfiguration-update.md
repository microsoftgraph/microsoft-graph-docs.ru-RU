---
title: Обновление Виндовсделиверйоптимизатионконфигуратион
description: Обновление свойств объекта Виндовсделиверйоптимизатионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea12634b689b5df13313ae22aaf585eadb0e3659
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961989"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="b09a0-103">Обновление Виндовсделиверйоптимизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b09a0-103">Update windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="b09a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b09a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b09a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b09a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b09a0-106">Обновление свойств объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b09a0-106">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b09a0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b09a0-107">Prerequisites</span></span>
<span data-ttu-id="b09a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b09a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b09a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b09a0-110">Permission type</span></span>|<span data-ttu-id="b09a0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b09a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b09a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b09a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b09a0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b09a0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b09a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b09a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b09a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b09a0-115">Not supported.</span></span>|
|<span data-ttu-id="b09a0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b09a0-116">Application</span></span>|<span data-ttu-id="b09a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b09a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b09a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b09a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b09a0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b09a0-119">Request headers</span></span>
|<span data-ttu-id="b09a0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b09a0-120">Header</span></span>|<span data-ttu-id="b09a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b09a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b09a0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b09a0-122">Authorization</span></span>|<span data-ttu-id="b09a0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b09a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b09a0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b09a0-124">Accept</span></span>|<span data-ttu-id="b09a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b09a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b09a0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b09a0-126">Request body</span></span>
<span data-ttu-id="b09a0-127">В тексте запроса добавьте представление объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b09a0-127">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="b09a0-128">В следующей таблице приведены свойства, необходимые при создании [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-128">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="b09a0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b09a0-129">Property</span></span>|<span data-ttu-id="b09a0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b09a0-130">Type</span></span>|<span data-ttu-id="b09a0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b09a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b09a0-132">id</span><span class="sxs-lookup"><span data-stu-id="b09a0-132">id</span></span>|<span data-ttu-id="b09a0-133">String</span><span class="sxs-lookup"><span data-stu-id="b09a0-133">String</span></span>|<span data-ttu-id="b09a0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b09a0-134">Key of the entity.</span></span> <span data-ttu-id="b09a0-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b09a0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b09a0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b09a0-137">DateTimeOffset</span></span>|<span data-ttu-id="b09a0-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b09a0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b09a0-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b09a0-140">roleScopeTagIds</span></span>|<span data-ttu-id="b09a0-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b09a0-141">String collection</span></span>|<span data-ttu-id="b09a0-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b09a0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b09a0-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b09a0-144">supportsScopeTags</span></span>|<span data-ttu-id="b09a0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b09a0-145">Boolean</span></span>|<span data-ttu-id="b09a0-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b09a0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b09a0-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b09a0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b09a0-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b09a0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b09a0-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b09a0-149">This property is read-only.</span></span> <span data-ttu-id="b09a0-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b09a0-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b09a0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b09a0-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b09a0-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b09a0-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b09a0-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b09a0-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b09a0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b09a0-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b09a0-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b09a0-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b09a0-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="b09a0-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b09a0-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="b09a0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b09a0-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b09a0-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b09a0-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b09a0-163">createdDateTime</span></span>|<span data-ttu-id="b09a0-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b09a0-164">DateTimeOffset</span></span>|<span data-ttu-id="b09a0-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b09a0-165">DateTime the object was created.</span></span> <span data-ttu-id="b09a0-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-167">description</span><span class="sxs-lookup"><span data-stu-id="b09a0-167">description</span></span>|<span data-ttu-id="b09a0-168">String</span><span class="sxs-lookup"><span data-stu-id="b09a0-168">String</span></span>|<span data-ttu-id="b09a0-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b09a0-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b09a0-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b09a0-171">displayName</span></span>|<span data-ttu-id="b09a0-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b09a0-172">String</span></span>|<span data-ttu-id="b09a0-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b09a0-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b09a0-174">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b09a0-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-175">version</span><span class="sxs-lookup"><span data-stu-id="b09a0-175">version</span></span>|<span data-ttu-id="b09a0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b09a0-176">Int32</span></span>|<span data-ttu-id="b09a0-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b09a0-177">Version of the device configuration.</span></span> <span data-ttu-id="b09a0-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b09a0-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b09a0-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="b09a0-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="b09a0-180">Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="b09a0-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="b09a0-181">Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента.</span><span class="sxs-lookup"><span data-stu-id="b09a0-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="b09a0-182">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="b09a0-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="b09a0-183">Рестриктпирселектионби</span><span class="sxs-lookup"><span data-stu-id="b09a0-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="b09a0-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="b09a0-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="b09a0-185">Задает ограничение выбора однорангового узла с помощью выбранного параметра.</span><span class="sxs-lookup"><span data-stu-id="b09a0-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="b09a0-186">Вариант 1 (маска подсети) применяется только к режимам оптимизации доставки LAN (1) и Group (2).</span><span class="sxs-lookup"><span data-stu-id="b09a0-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="b09a0-187">Возможные значения: `notConfigured`, `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="b09a0-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="b09a0-188">Граупидсаурце</span><span class="sxs-lookup"><span data-stu-id="b09a0-188">groupIdSource</span></span>|[<span data-ttu-id="b09a0-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="b09a0-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="b09a0-190">Задает ограничение выбора однорангового узла для источника получать.</span><span class="sxs-lookup"><span data-stu-id="b09a0-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="b09a0-191">Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2).</span><span class="sxs-lookup"><span data-stu-id="b09a0-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="b09a0-192">Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="b09a0-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="b09a0-193">Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.</span><span class="sxs-lookup"><span data-stu-id="b09a0-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="b09a0-194">Бандвидсмоде</span><span class="sxs-lookup"><span data-stu-id="b09a0-194">bandwidthMode</span></span>|[<span data-ttu-id="b09a0-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="b09a0-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="b09a0-196">Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.</span><span class="sxs-lookup"><span data-stu-id="b09a0-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="b09a0-197">Баккграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="b09a0-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="b09a0-198">Int64</span><span class="sxs-lookup"><span data-stu-id="b09a0-198">Int64</span></span>|<span data-ttu-id="b09a0-199">Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения.</span><span class="sxs-lookup"><span data-stu-id="b09a0-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="b09a0-200">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="b09a0-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="b09a0-201">Фореграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="b09a0-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="b09a0-202">Int64</span><span class="sxs-lookup"><span data-stu-id="b09a0-202">Int64</span></span>|<span data-ttu-id="b09a0-203">Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400).</span><span class="sxs-lookup"><span data-stu-id="b09a0-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="b09a0-204">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="b09a0-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="b09a0-205">Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы.</span><span class="sxs-lookup"><span data-stu-id="b09a0-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="b09a0-206">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="b09a0-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="b09a0-207">Минимумрамалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="b09a0-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="b09a0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="b09a0-208">Int32</span></span>|<span data-ttu-id="b09a0-209">Указывает минимальный размер ОЗУ в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="b09a0-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="b09a0-210">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="b09a0-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="b09a0-211">Минимумдисксизеалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="b09a0-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="b09a0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b09a0-212">Int32</span></span>|<span data-ttu-id="b09a0-213">Указывает минимальный размер диска в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="b09a0-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="b09a0-214">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="b09a0-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="b09a0-215">Рекомендуемые значения: 64 ГБ до 256 ГБ.</span><span class="sxs-lookup"><span data-stu-id="b09a0-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="b09a0-216">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="b09a0-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="b09a0-217">Минимумфилесизетокачеинмегабитес</span><span class="sxs-lookup"><span data-stu-id="b09a0-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="b09a0-218">Int32</span><span class="sxs-lookup"><span data-stu-id="b09a0-218">Int32</span></span>|<span data-ttu-id="b09a0-219">Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000).</span><span class="sxs-lookup"><span data-stu-id="b09a0-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="b09a0-220">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="b09a0-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="b09a0-221">Рекомендуемые значения: от 1 МБ до 100 000 МБ.</span><span class="sxs-lookup"><span data-stu-id="b09a0-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="b09a0-222">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="b09a0-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="b09a0-223">Минимумбаттериперцентажеалловедтауплоад</span><span class="sxs-lookup"><span data-stu-id="b09a0-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="b09a0-224">Int32</span><span class="sxs-lookup"><span data-stu-id="b09a0-224">Int32</span></span>|<span data-ttu-id="b09a0-225">Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100).</span><span class="sxs-lookup"><span data-stu-id="b09a0-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="b09a0-226">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="b09a0-226">Valid values 0 to 100</span></span>
<span data-ttu-id="b09a0-227">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="b09a0-227">The default value is 0.</span></span> <span data-ttu-id="b09a0-228">Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы.</span><span class="sxs-lookup"><span data-stu-id="b09a0-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="b09a0-229">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="b09a0-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b09a0-230">Модификачелокатион</span><span class="sxs-lookup"><span data-stu-id="b09a0-230">modifyCacheLocation</span></span>|<span data-ttu-id="b09a0-231">String</span><span class="sxs-lookup"><span data-stu-id="b09a0-231">String</span></span>|<span data-ttu-id="b09a0-232">Указывает диск, который должна использовать оптимизация доставки для своего кэша.</span><span class="sxs-lookup"><span data-stu-id="b09a0-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="b09a0-233">Максимумкачеажеиндайс</span><span class="sxs-lookup"><span data-stu-id="b09a0-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="b09a0-234">Int32</span><span class="sxs-lookup"><span data-stu-id="b09a0-234">Int32</span></span>|<span data-ttu-id="b09a0-235">Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-3650).</span><span class="sxs-lookup"><span data-stu-id="b09a0-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="b09a0-236">Допустимые значения — от 0 до 3650</span><span class="sxs-lookup"><span data-stu-id="b09a0-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="b09a0-237">Максимумкачесизе</span><span class="sxs-lookup"><span data-stu-id="b09a0-237">maximumCacheSize</span></span>|[<span data-ttu-id="b09a0-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="b09a0-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="b09a0-239">Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.</span><span class="sxs-lookup"><span data-stu-id="b09a0-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="b09a0-240">Впнпиркачинг</span><span class="sxs-lookup"><span data-stu-id="b09a0-240">vpnPeerCaching</span></span>|[<span data-ttu-id="b09a0-241">Включение</span><span class="sxs-lookup"><span data-stu-id="b09a0-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b09a0-242">Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети.</span><span class="sxs-lookup"><span data-stu-id="b09a0-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="b09a0-243">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b09a0-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="b09a0-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="b09a0-244">Response</span></span>
<span data-ttu-id="b09a0-245">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b09a0-245">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b09a0-246">Пример</span><span class="sxs-lookup"><span data-stu-id="b09a0-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="b09a0-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="b09a0-247">Request</span></span>
<span data-ttu-id="b09a0-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b09a0-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1833

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
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="b09a0-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="b09a0-249">Response</span></span>
<span data-ttu-id="b09a0-p128">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b09a0-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2005

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
  "vpnPeerCaching": "enabled"
}
```





