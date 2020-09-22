---
title: Создание Виндовсделиверйоптимизатионконфигуратион
description: Создание нового объекта Виндовсделиверйоптимизатионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2be52f7ea570ef2173b93675684fe05b084c98e0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065419"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="e2951-103">Создание Виндовсделиверйоптимизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e2951-103">Create windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="e2951-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2951-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2951-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2951-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2951-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2951-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2951-107">Создание нового объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2951-107">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2951-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2951-108">Prerequisites</span></span>
<span data-ttu-id="e2951-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2951-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2951-111">Permission type</span></span>|<span data-ttu-id="e2951-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2951-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2951-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2951-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2951-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2951-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2951-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2951-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2951-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2951-116">Not supported.</span></span>|
|<span data-ttu-id="e2951-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2951-117">Application</span></span>|<span data-ttu-id="e2951-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2951-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2951-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2951-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2951-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2951-120">Request headers</span></span>
|<span data-ttu-id="e2951-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2951-121">Header</span></span>|<span data-ttu-id="e2951-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2951-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2951-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2951-123">Authorization</span></span>|<span data-ttu-id="e2951-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2951-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2951-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2951-125">Accept</span></span>|<span data-ttu-id="e2951-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2951-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2951-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2951-127">Request body</span></span>
<span data-ttu-id="e2951-128">В тексте запроса добавьте представление объекта Виндовсделиверйоптимизатионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2951-128">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="e2951-129">В следующей таблице приведены свойства, необходимые при создании Виндовсделиверйоптимизатионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="e2951-129">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="e2951-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2951-130">Property</span></span>|<span data-ttu-id="e2951-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2951-131">Type</span></span>|<span data-ttu-id="e2951-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2951-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2951-133">id</span><span class="sxs-lookup"><span data-stu-id="e2951-133">id</span></span>|<span data-ttu-id="e2951-134">String</span><span class="sxs-lookup"><span data-stu-id="e2951-134">String</span></span>|<span data-ttu-id="e2951-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2951-135">Key of the entity.</span></span> <span data-ttu-id="e2951-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2951-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2951-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2951-138">DateTimeOffset</span></span>|<span data-ttu-id="e2951-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2951-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e2951-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2951-141">roleScopeTagIds</span></span>|<span data-ttu-id="e2951-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e2951-142">String collection</span></span>|<span data-ttu-id="e2951-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e2951-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2951-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e2951-145">supportsScopeTags</span></span>|<span data-ttu-id="e2951-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2951-146">Boolean</span></span>|<span data-ttu-id="e2951-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e2951-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2951-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e2951-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2951-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e2951-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2951-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2951-150">This property is read-only.</span></span> <span data-ttu-id="e2951-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2951-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e2951-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2951-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e2951-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2951-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e2951-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2951-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e2951-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2951-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e2951-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2951-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e2951-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2951-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e2951-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2951-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e2951-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2951-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e2951-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2951-164">createdDateTime</span></span>|<span data-ttu-id="e2951-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2951-165">DateTimeOffset</span></span>|<span data-ttu-id="e2951-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2951-166">DateTime the object was created.</span></span> <span data-ttu-id="e2951-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-168">description</span><span class="sxs-lookup"><span data-stu-id="e2951-168">description</span></span>|<span data-ttu-id="e2951-169">String</span><span class="sxs-lookup"><span data-stu-id="e2951-169">String</span></span>|<span data-ttu-id="e2951-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2951-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2951-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e2951-172">displayName</span></span>|<span data-ttu-id="e2951-173">String</span><span class="sxs-lookup"><span data-stu-id="e2951-173">String</span></span>|<span data-ttu-id="e2951-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2951-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2951-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-176">version</span><span class="sxs-lookup"><span data-stu-id="e2951-176">version</span></span>|<span data-ttu-id="e2951-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-177">Int32</span></span>|<span data-ttu-id="e2951-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2951-178">Version of the device configuration.</span></span> <span data-ttu-id="e2951-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2951-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2951-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e2951-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="e2951-181">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="e2951-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="e2951-182">Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента.</span><span class="sxs-lookup"><span data-stu-id="e2951-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="e2951-183">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="e2951-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="e2951-184">рестриктпирселектионби</span><span class="sxs-lookup"><span data-stu-id="e2951-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="e2951-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="e2951-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="e2951-186">Задает ограничение выбора однорангового узла с помощью выбранного параметра.</span><span class="sxs-lookup"><span data-stu-id="e2951-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="e2951-187">Вариант 1 (маска подсети) применяется только к режимам оптимизации доставки LAN (1) и Group (2).</span><span class="sxs-lookup"><span data-stu-id="e2951-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="e2951-188">Возможные значения: `notConfigured`, `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="e2951-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="e2951-189">граупидсаурце</span><span class="sxs-lookup"><span data-stu-id="e2951-189">groupIdSource</span></span>|[<span data-ttu-id="e2951-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="e2951-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="e2951-191">Задает ограничение выбора однорангового узла для источника получать.</span><span class="sxs-lookup"><span data-stu-id="e2951-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="e2951-192">Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2).</span><span class="sxs-lookup"><span data-stu-id="e2951-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="e2951-193">Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e2951-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="e2951-194">Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.</span><span class="sxs-lookup"><span data-stu-id="e2951-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="e2951-195">бандвидсмоде</span><span class="sxs-lookup"><span data-stu-id="e2951-195">bandwidthMode</span></span>|[<span data-ttu-id="e2951-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="e2951-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="e2951-197">Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.</span><span class="sxs-lookup"><span data-stu-id="e2951-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="e2951-198">баккграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="e2951-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="e2951-199">Int64</span><span class="sxs-lookup"><span data-stu-id="e2951-199">Int64</span></span>|<span data-ttu-id="e2951-200">Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения.</span><span class="sxs-lookup"><span data-stu-id="e2951-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="e2951-201">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="e2951-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="e2951-202">фореграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="e2951-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="e2951-203">Int64</span><span class="sxs-lookup"><span data-stu-id="e2951-203">Int64</span></span>|<span data-ttu-id="e2951-204">Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400).</span><span class="sxs-lookup"><span data-stu-id="e2951-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="e2951-205">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="e2951-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="e2951-206">Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы.</span><span class="sxs-lookup"><span data-stu-id="e2951-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="e2951-207">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="e2951-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="e2951-208">минимумрамалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="e2951-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="e2951-209">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-209">Int32</span></span>|<span data-ttu-id="e2951-210">Указывает минимальный размер ОЗУ в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="e2951-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="e2951-211">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="e2951-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="e2951-212">минимумдисксизеалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="e2951-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="e2951-213">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-213">Int32</span></span>|<span data-ttu-id="e2951-214">Указывает минимальный размер диска в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="e2951-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="e2951-215">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="e2951-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="e2951-216">Рекомендуемые значения: 64 ГБ до 256 ГБ.</span><span class="sxs-lookup"><span data-stu-id="e2951-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="e2951-217">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="e2951-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="e2951-218">минимумфилесизетокачеинмегабитес</span><span class="sxs-lookup"><span data-stu-id="e2951-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="e2951-219">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-219">Int32</span></span>|<span data-ttu-id="e2951-220">Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000).</span><span class="sxs-lookup"><span data-stu-id="e2951-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="e2951-221">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="e2951-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="e2951-222">Рекомендуемые значения: от 1 МБ до 100 000 МБ.</span><span class="sxs-lookup"><span data-stu-id="e2951-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="e2951-223">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="e2951-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="e2951-224">минимумбаттериперцентажеалловедтауплоад</span><span class="sxs-lookup"><span data-stu-id="e2951-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="e2951-225">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-225">Int32</span></span>|<span data-ttu-id="e2951-226">Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100).</span><span class="sxs-lookup"><span data-stu-id="e2951-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="e2951-227">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="e2951-227">Valid values 0 to 100</span></span>
<span data-ttu-id="e2951-228">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="e2951-228">The default value is 0.</span></span> <span data-ttu-id="e2951-229">Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы.</span><span class="sxs-lookup"><span data-stu-id="e2951-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="e2951-230">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="e2951-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="e2951-231">модификачелокатион</span><span class="sxs-lookup"><span data-stu-id="e2951-231">modifyCacheLocation</span></span>|<span data-ttu-id="e2951-232">String</span><span class="sxs-lookup"><span data-stu-id="e2951-232">String</span></span>|<span data-ttu-id="e2951-233">Указывает диск, который должна использовать оптимизация доставки для своего кэша.</span><span class="sxs-lookup"><span data-stu-id="e2951-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="e2951-234">максимумкачеажеиндайс</span><span class="sxs-lookup"><span data-stu-id="e2951-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="e2951-235">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-235">Int32</span></span>|<span data-ttu-id="e2951-236">Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-3650).</span><span class="sxs-lookup"><span data-stu-id="e2951-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="e2951-237">Допустимые значения — от 0 до 3650</span><span class="sxs-lookup"><span data-stu-id="e2951-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="e2951-238">максимумкачесизе</span><span class="sxs-lookup"><span data-stu-id="e2951-238">maximumCacheSize</span></span>|[<span data-ttu-id="e2951-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="e2951-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="e2951-240">Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.</span><span class="sxs-lookup"><span data-stu-id="e2951-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="e2951-241">впнпиркачинг</span><span class="sxs-lookup"><span data-stu-id="e2951-241">vpnPeerCaching</span></span>|[<span data-ttu-id="e2951-242">Включение</span><span class="sxs-lookup"><span data-stu-id="e2951-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="e2951-243">Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети.</span><span class="sxs-lookup"><span data-stu-id="e2951-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="e2951-244">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e2951-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e2951-245">качесерверхостнамес</span><span class="sxs-lookup"><span data-stu-id="e2951-245">cacheServerHostNames</span></span>|<span data-ttu-id="e2951-246">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e2951-246">String collection</span></span>|<span data-ttu-id="e2951-247">Указывает имена узлов серверов кэша.</span><span class="sxs-lookup"><span data-stu-id="e2951-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="e2951-248">качесерверфореграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="e2951-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="e2951-249">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-249">Int32</span></span>|<span data-ttu-id="e2951-250">Указывает время (в секундах), по истечении которого откладывается обратное сообщение от серверов кэша к источнику HTTP для загрузки переднего плана.</span><span class="sxs-lookup"><span data-stu-id="e2951-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="e2951-251">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="e2951-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="e2951-252">качесервербаккграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="e2951-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="e2951-253">Int32</span><span class="sxs-lookup"><span data-stu-id="e2951-253">Int32</span></span>|<span data-ttu-id="e2951-254">Указывает время (в секундах), по истечении которого будет возвращаться обратно от серверов кэша к источнику HTTP для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="e2951-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="e2951-255">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="e2951-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="e2951-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2951-256">Response</span></span>
<span data-ttu-id="e2951-257">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2951-257">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2951-258">Пример</span><span class="sxs-lookup"><span data-stu-id="e2951-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2951-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2951-259">Request</span></span>
<span data-ttu-id="e2951-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2951-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="e2951-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2951-261">Response</span></span>
<span data-ttu-id="e2951-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2951-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






