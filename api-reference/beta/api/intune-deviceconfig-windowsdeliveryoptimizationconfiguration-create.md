---
title: Создание Виндовсделиверйоптимизатионконфигуратион
description: Создание нового объекта Виндовсделиверйоптимизатионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 682eae86adf98c52979d4ecf9e3790d15b218974
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43429757"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="f6384-103">Создание Виндовсделиверйоптимизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f6384-103">Create windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="f6384-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6384-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6384-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6384-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6384-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6384-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6384-107">Создание нового объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f6384-107">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6384-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6384-108">Prerequisites</span></span>
<span data-ttu-id="f6384-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6384-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6384-111">Permission type</span></span>|<span data-ttu-id="f6384-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6384-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6384-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6384-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6384-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6384-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6384-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6384-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6384-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6384-116">Not supported.</span></span>|
|<span data-ttu-id="f6384-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6384-117">Application</span></span>|<span data-ttu-id="f6384-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6384-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6384-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6384-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6384-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6384-120">Request headers</span></span>
|<span data-ttu-id="f6384-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6384-121">Header</span></span>|<span data-ttu-id="f6384-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6384-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6384-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6384-123">Authorization</span></span>|<span data-ttu-id="f6384-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6384-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6384-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6384-125">Accept</span></span>|<span data-ttu-id="f6384-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6384-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6384-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6384-127">Request body</span></span>
<span data-ttu-id="f6384-128">В тексте запроса добавьте представление объекта Виндовсделиверйоптимизатионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6384-128">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="f6384-129">В следующей таблице приведены свойства, необходимые при создании Виндовсделиверйоптимизатионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f6384-129">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="f6384-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6384-130">Property</span></span>|<span data-ttu-id="f6384-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6384-131">Type</span></span>|<span data-ttu-id="f6384-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6384-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6384-133">id</span><span class="sxs-lookup"><span data-stu-id="f6384-133">id</span></span>|<span data-ttu-id="f6384-134">String</span><span class="sxs-lookup"><span data-stu-id="f6384-134">String</span></span>|<span data-ttu-id="f6384-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f6384-135">Key of the entity.</span></span> <span data-ttu-id="f6384-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6384-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f6384-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6384-138">DateTimeOffset</span></span>|<span data-ttu-id="f6384-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f6384-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f6384-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6384-141">roleScopeTagIds</span></span>|<span data-ttu-id="f6384-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f6384-142">String collection</span></span>|<span data-ttu-id="f6384-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f6384-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6384-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f6384-145">supportsScopeTags</span></span>|<span data-ttu-id="f6384-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6384-146">Boolean</span></span>|<span data-ttu-id="f6384-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f6384-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f6384-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f6384-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f6384-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f6384-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f6384-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6384-150">This property is read-only.</span></span> <span data-ttu-id="f6384-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6384-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f6384-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6384-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f6384-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f6384-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f6384-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6384-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f6384-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6384-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f6384-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f6384-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f6384-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f6384-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f6384-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f6384-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f6384-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f6384-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f6384-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6384-164">createdDateTime</span></span>|<span data-ttu-id="f6384-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6384-165">DateTimeOffset</span></span>|<span data-ttu-id="f6384-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f6384-166">DateTime the object was created.</span></span> <span data-ttu-id="f6384-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-168">description</span><span class="sxs-lookup"><span data-stu-id="f6384-168">description</span></span>|<span data-ttu-id="f6384-169">String</span><span class="sxs-lookup"><span data-stu-id="f6384-169">String</span></span>|<span data-ttu-id="f6384-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6384-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6384-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f6384-172">displayName</span></span>|<span data-ttu-id="f6384-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f6384-173">String</span></span>|<span data-ttu-id="f6384-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6384-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6384-175">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6384-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-176">version</span><span class="sxs-lookup"><span data-stu-id="f6384-176">version</span></span>|<span data-ttu-id="f6384-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-177">Int32</span></span>|<span data-ttu-id="f6384-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f6384-178">Version of the device configuration.</span></span> <span data-ttu-id="f6384-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6384-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6384-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f6384-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f6384-181">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="f6384-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f6384-182">Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента.</span><span class="sxs-lookup"><span data-stu-id="f6384-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="f6384-183">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="f6384-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f6384-184">рестриктпирселектионби</span><span class="sxs-lookup"><span data-stu-id="f6384-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="f6384-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="f6384-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="f6384-186">Задает ограничение выбора однорангового узла с помощью выбранного параметра.</span><span class="sxs-lookup"><span data-stu-id="f6384-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="f6384-187">Вариант 1 (маска подсети) применяется только к режимам оптимизации доставки LAN (1) и Group (2).</span><span class="sxs-lookup"><span data-stu-id="f6384-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="f6384-188">Возможные значения: `notConfigured`, `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="f6384-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="f6384-189">граупидсаурце</span><span class="sxs-lookup"><span data-stu-id="f6384-189">groupIdSource</span></span>|[<span data-ttu-id="f6384-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="f6384-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="f6384-191">Задает ограничение выбора однорангового узла для источника получать.</span><span class="sxs-lookup"><span data-stu-id="f6384-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="f6384-192">Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2).</span><span class="sxs-lookup"><span data-stu-id="f6384-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="f6384-193">Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="f6384-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="f6384-194">Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.</span><span class="sxs-lookup"><span data-stu-id="f6384-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="f6384-195">бандвидсмоде</span><span class="sxs-lookup"><span data-stu-id="f6384-195">bandwidthMode</span></span>|[<span data-ttu-id="f6384-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="f6384-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="f6384-197">Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.</span><span class="sxs-lookup"><span data-stu-id="f6384-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="f6384-198">баккграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="f6384-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="f6384-199">Int64</span><span class="sxs-lookup"><span data-stu-id="f6384-199">Int64</span></span>|<span data-ttu-id="f6384-200">Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения.</span><span class="sxs-lookup"><span data-stu-id="f6384-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="f6384-201">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="f6384-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="f6384-202">фореграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="f6384-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="f6384-203">Int64</span><span class="sxs-lookup"><span data-stu-id="f6384-203">Int64</span></span>|<span data-ttu-id="f6384-204">Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400).</span><span class="sxs-lookup"><span data-stu-id="f6384-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="f6384-205">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="f6384-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="f6384-206">Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы.</span><span class="sxs-lookup"><span data-stu-id="f6384-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="f6384-207">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="f6384-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="f6384-208">минимумрамалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="f6384-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="f6384-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-209">Int32</span></span>|<span data-ttu-id="f6384-210">Указывает минимальный размер ОЗУ в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="f6384-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="f6384-211">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="f6384-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="f6384-212">минимумдисксизеалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="f6384-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="f6384-213">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-213">Int32</span></span>|<span data-ttu-id="f6384-214">Указывает минимальный размер диска в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="f6384-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="f6384-215">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="f6384-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="f6384-216">Рекомендуемые значения: 64 ГБ до 256 ГБ.</span><span class="sxs-lookup"><span data-stu-id="f6384-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="f6384-217">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="f6384-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="f6384-218">минимумфилесизетокачеинмегабитес</span><span class="sxs-lookup"><span data-stu-id="f6384-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="f6384-219">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-219">Int32</span></span>|<span data-ttu-id="f6384-220">Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000).</span><span class="sxs-lookup"><span data-stu-id="f6384-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="f6384-221">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="f6384-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="f6384-222">Рекомендуемые значения: от 1 МБ до 100 000 МБ.</span><span class="sxs-lookup"><span data-stu-id="f6384-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="f6384-223">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="f6384-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="f6384-224">минимумбаттериперцентажеалловедтауплоад</span><span class="sxs-lookup"><span data-stu-id="f6384-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="f6384-225">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-225">Int32</span></span>|<span data-ttu-id="f6384-226">Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100).</span><span class="sxs-lookup"><span data-stu-id="f6384-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="f6384-227">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="f6384-227">Valid values 0 to 100</span></span>
<span data-ttu-id="f6384-228">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="f6384-228">The default value is 0.</span></span> <span data-ttu-id="f6384-229">Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы.</span><span class="sxs-lookup"><span data-stu-id="f6384-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="f6384-230">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="f6384-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="f6384-231">модификачелокатион</span><span class="sxs-lookup"><span data-stu-id="f6384-231">modifyCacheLocation</span></span>|<span data-ttu-id="f6384-232">String</span><span class="sxs-lookup"><span data-stu-id="f6384-232">String</span></span>|<span data-ttu-id="f6384-233">Указывает диск, который должна использовать оптимизация доставки для своего кэша.</span><span class="sxs-lookup"><span data-stu-id="f6384-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="f6384-234">максимумкачеажеиндайс</span><span class="sxs-lookup"><span data-stu-id="f6384-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="f6384-235">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-235">Int32</span></span>|<span data-ttu-id="f6384-236">Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-3650).</span><span class="sxs-lookup"><span data-stu-id="f6384-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="f6384-237">Допустимые значения — от 0 до 3650</span><span class="sxs-lookup"><span data-stu-id="f6384-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="f6384-238">максимумкачесизе</span><span class="sxs-lookup"><span data-stu-id="f6384-238">maximumCacheSize</span></span>|[<span data-ttu-id="f6384-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="f6384-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="f6384-240">Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.</span><span class="sxs-lookup"><span data-stu-id="f6384-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="f6384-241">впнпиркачинг</span><span class="sxs-lookup"><span data-stu-id="f6384-241">vpnPeerCaching</span></span>|[<span data-ttu-id="f6384-242">Включение</span><span class="sxs-lookup"><span data-stu-id="f6384-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6384-243">Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети.</span><span class="sxs-lookup"><span data-stu-id="f6384-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="f6384-244">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f6384-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f6384-245">качесерверхостнамес</span><span class="sxs-lookup"><span data-stu-id="f6384-245">cacheServerHostNames</span></span>|<span data-ttu-id="f6384-246">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f6384-246">String collection</span></span>|<span data-ttu-id="f6384-247">Указывает имена узлов серверов кэша.</span><span class="sxs-lookup"><span data-stu-id="f6384-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="f6384-248">качесерверфореграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="f6384-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="f6384-249">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-249">Int32</span></span>|<span data-ttu-id="f6384-250">Указывает время (в секундах), по истечении которого откладывается обратное сообщение от серверов кэша к источнику HTTP для загрузки переднего плана.</span><span class="sxs-lookup"><span data-stu-id="f6384-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="f6384-251">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="f6384-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="f6384-252">качесервербаккграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="f6384-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="f6384-253">Int32</span><span class="sxs-lookup"><span data-stu-id="f6384-253">Int32</span></span>|<span data-ttu-id="f6384-254">Указывает время (в секундах), по истечении которого будет возвращаться обратно от серверов кэша к источнику HTTP для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="f6384-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="f6384-255">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="f6384-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="f6384-256">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6384-256">Response</span></span>
<span data-ttu-id="f6384-257">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6384-257">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6384-258">Пример</span><span class="sxs-lookup"><span data-stu-id="f6384-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6384-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6384-259">Request</span></span>
<span data-ttu-id="f6384-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6384-260">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6384-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6384-261">Response</span></span>
<span data-ttu-id="f6384-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6384-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



