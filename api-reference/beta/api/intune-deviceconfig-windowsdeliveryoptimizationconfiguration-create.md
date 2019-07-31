---
title: Создание Виндовсделиверйоптимизатионконфигуратион
description: Создание нового объекта Виндовсделиверйоптимизатионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64c0ca78ad24c730d26a30bc104a27c254c58f5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982328"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="4f185-103">Создание Виндовсделиверйоптимизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4f185-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="4f185-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f185-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f185-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f185-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f185-106">Создание нового объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4f185-106">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f185-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f185-107">Prerequisites</span></span>
<span data-ttu-id="4f185-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f185-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f185-110">Permission type</span></span>|<span data-ttu-id="4f185-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f185-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f185-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f185-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f185-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f185-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f185-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f185-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f185-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f185-115">Not supported.</span></span>|
|<span data-ttu-id="4f185-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f185-116">Application</span></span>|<span data-ttu-id="4f185-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f185-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f185-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f185-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f185-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f185-119">Request headers</span></span>
|<span data-ttu-id="4f185-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f185-120">Header</span></span>|<span data-ttu-id="4f185-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f185-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f185-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f185-122">Authorization</span></span>|<span data-ttu-id="4f185-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f185-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f185-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f185-124">Accept</span></span>|<span data-ttu-id="4f185-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f185-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f185-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f185-126">Request body</span></span>
<span data-ttu-id="4f185-127">В тексте запроса добавьте представление объекта Виндовсделиверйоптимизатионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f185-127">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="4f185-128">В следующей таблице приведены свойства, необходимые при создании Виндовсделиверйоптимизатионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4f185-128">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="4f185-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f185-129">Property</span></span>|<span data-ttu-id="4f185-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4f185-130">Type</span></span>|<span data-ttu-id="4f185-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4f185-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f185-132">id</span><span class="sxs-lookup"><span data-stu-id="4f185-132">id</span></span>|<span data-ttu-id="4f185-133">String</span><span class="sxs-lookup"><span data-stu-id="4f185-133">String</span></span>|<span data-ttu-id="4f185-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f185-134">Key of the entity.</span></span> <span data-ttu-id="4f185-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f185-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4f185-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f185-137">DateTimeOffset</span></span>|<span data-ttu-id="4f185-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4f185-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4f185-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f185-140">roleScopeTagIds</span></span>|<span data-ttu-id="4f185-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4f185-141">String collection</span></span>|<span data-ttu-id="4f185-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4f185-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f185-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4f185-144">supportsScopeTags</span></span>|<span data-ttu-id="4f185-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f185-145">Boolean</span></span>|<span data-ttu-id="4f185-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4f185-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4f185-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4f185-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4f185-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4f185-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4f185-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f185-149">This property is read-only.</span></span> <span data-ttu-id="4f185-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f185-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4f185-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f185-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4f185-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f185-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4f185-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f185-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4f185-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f185-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4f185-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f185-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4f185-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4f185-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4f185-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4f185-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4f185-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f185-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4f185-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f185-163">createdDateTime</span></span>|<span data-ttu-id="4f185-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f185-164">DateTimeOffset</span></span>|<span data-ttu-id="4f185-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4f185-165">DateTime the object was created.</span></span> <span data-ttu-id="4f185-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-167">description</span><span class="sxs-lookup"><span data-stu-id="4f185-167">description</span></span>|<span data-ttu-id="4f185-168">String</span><span class="sxs-lookup"><span data-stu-id="4f185-168">String</span></span>|<span data-ttu-id="4f185-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f185-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f185-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4f185-171">displayName</span></span>|<span data-ttu-id="4f185-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4f185-172">String</span></span>|<span data-ttu-id="4f185-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f185-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f185-174">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f185-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-175">version</span><span class="sxs-lookup"><span data-stu-id="4f185-175">version</span></span>|<span data-ttu-id="4f185-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-176">Int32</span></span>|<span data-ttu-id="4f185-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f185-177">Version of the device configuration.</span></span> <span data-ttu-id="4f185-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f185-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f185-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4f185-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="4f185-180">Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="4f185-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="4f185-181">Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента.</span><span class="sxs-lookup"><span data-stu-id="4f185-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="4f185-182">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="4f185-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="4f185-183">Рестриктпирселектионби</span><span class="sxs-lookup"><span data-stu-id="4f185-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="4f185-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="4f185-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="4f185-185">Задает ограничение выбора однорангового узла с помощью выбранного параметра.</span><span class="sxs-lookup"><span data-stu-id="4f185-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="4f185-186">Вариант 1 (маска подсети) применяется только к режимам оптимизации доставки LAN (1) и Group (2).</span><span class="sxs-lookup"><span data-stu-id="4f185-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="4f185-187">Возможные значения: `notConfigured`, `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="4f185-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="4f185-188">Граупидсаурце</span><span class="sxs-lookup"><span data-stu-id="4f185-188">groupIdSource</span></span>|[<span data-ttu-id="4f185-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="4f185-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="4f185-190">Задает ограничение выбора однорангового узла для источника получать.</span><span class="sxs-lookup"><span data-stu-id="4f185-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="4f185-191">Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2).</span><span class="sxs-lookup"><span data-stu-id="4f185-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="4f185-192">Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="4f185-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="4f185-193">Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.</span><span class="sxs-lookup"><span data-stu-id="4f185-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="4f185-194">Бандвидсмоде</span><span class="sxs-lookup"><span data-stu-id="4f185-194">bandwidthMode</span></span>|[<span data-ttu-id="4f185-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="4f185-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="4f185-196">Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.</span><span class="sxs-lookup"><span data-stu-id="4f185-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="4f185-197">Баккграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="4f185-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="4f185-198">Int64</span><span class="sxs-lookup"><span data-stu-id="4f185-198">Int64</span></span>|<span data-ttu-id="4f185-199">Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения.</span><span class="sxs-lookup"><span data-stu-id="4f185-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="4f185-200">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="4f185-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="4f185-201">Фореграунддовнлоадфромхттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="4f185-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="4f185-202">Int64</span><span class="sxs-lookup"><span data-stu-id="4f185-202">Int64</span></span>|<span data-ttu-id="4f185-203">Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400).</span><span class="sxs-lookup"><span data-stu-id="4f185-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="4f185-204">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="4f185-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="4f185-205">Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы.</span><span class="sxs-lookup"><span data-stu-id="4f185-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="4f185-206">Допустимые значения — от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="4f185-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="4f185-207">Минимумрамалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="4f185-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="4f185-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-208">Int32</span></span>|<span data-ttu-id="4f185-209">Указывает минимальный размер ОЗУ в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="4f185-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4f185-210">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4f185-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4f185-211">Минимумдисксизеалловедтопирингигабитес</span><span class="sxs-lookup"><span data-stu-id="4f185-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="4f185-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-212">Int32</span></span>|<span data-ttu-id="4f185-213">Указывает минимальный размер диска в ГБ для использования однорангового кэширования (1-100000).</span><span class="sxs-lookup"><span data-stu-id="4f185-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4f185-214">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4f185-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="4f185-215">Рекомендуемые значения: 64 ГБ до 256 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4f185-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="4f185-216">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4f185-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4f185-217">Минимумфилесизетокачеинмегабитес</span><span class="sxs-lookup"><span data-stu-id="4f185-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="4f185-218">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-218">Int32</span></span>|<span data-ttu-id="4f185-219">Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000).</span><span class="sxs-lookup"><span data-stu-id="4f185-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4f185-220">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4f185-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="4f185-221">Рекомендуемые значения: от 1 МБ до 100 000 МБ.</span><span class="sxs-lookup"><span data-stu-id="4f185-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="4f185-222">Допустимые значения — от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4f185-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4f185-223">Минимумбаттериперцентажеалловедтауплоад</span><span class="sxs-lookup"><span data-stu-id="4f185-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="4f185-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-224">Int32</span></span>|<span data-ttu-id="4f185-225">Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100).</span><span class="sxs-lookup"><span data-stu-id="4f185-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="4f185-226">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4f185-226">Valid values 0 to 100</span></span>
<span data-ttu-id="4f185-227">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="4f185-227">The default value is 0.</span></span> <span data-ttu-id="4f185-228">Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы.</span><span class="sxs-lookup"><span data-stu-id="4f185-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="4f185-229">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4f185-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4f185-230">Модификачелокатион</span><span class="sxs-lookup"><span data-stu-id="4f185-230">modifyCacheLocation</span></span>|<span data-ttu-id="4f185-231">String</span><span class="sxs-lookup"><span data-stu-id="4f185-231">String</span></span>|<span data-ttu-id="4f185-232">Указывает диск, который должна использовать оптимизация доставки для своего кэша.</span><span class="sxs-lookup"><span data-stu-id="4f185-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="4f185-233">Максимумкачеажеиндайс</span><span class="sxs-lookup"><span data-stu-id="4f185-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="4f185-234">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-234">Int32</span></span>|<span data-ttu-id="4f185-235">Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-3650).</span><span class="sxs-lookup"><span data-stu-id="4f185-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="4f185-236">Допустимые значения — от 0 до 3650</span><span class="sxs-lookup"><span data-stu-id="4f185-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="4f185-237">Максимумкачесизе</span><span class="sxs-lookup"><span data-stu-id="4f185-237">maximumCacheSize</span></span>|[<span data-ttu-id="4f185-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="4f185-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="4f185-239">Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.</span><span class="sxs-lookup"><span data-stu-id="4f185-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="4f185-240">Впнпиркачинг</span><span class="sxs-lookup"><span data-stu-id="4f185-240">vpnPeerCaching</span></span>|[<span data-ttu-id="4f185-241">Включение</span><span class="sxs-lookup"><span data-stu-id="4f185-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4f185-242">Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети.</span><span class="sxs-lookup"><span data-stu-id="4f185-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="4f185-243">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4f185-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4f185-244">Качесерверхостнамес</span><span class="sxs-lookup"><span data-stu-id="4f185-244">cacheServerHostNames</span></span>|<span data-ttu-id="4f185-245">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4f185-245">String collection</span></span>|<span data-ttu-id="4f185-246">Указывает имена узлов серверов кэша.</span><span class="sxs-lookup"><span data-stu-id="4f185-246">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="4f185-247">Качесерверфореграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="4f185-247">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="4f185-248">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-248">Int32</span></span>|<span data-ttu-id="4f185-249">Указывает время (в секундах), по истечении которого откладывается обратное сообщение от серверов кэша к источнику HTTP для загрузки переднего плана.</span><span class="sxs-lookup"><span data-stu-id="4f185-249">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="4f185-250">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="4f185-250">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="4f185-251">Качесервербаккграунддовнлоадфаллбакктохттпделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="4f185-251">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="4f185-252">Int32</span><span class="sxs-lookup"><span data-stu-id="4f185-252">Int32</span></span>|<span data-ttu-id="4f185-253">Указывает время (в секундах), по истечении которого будет возвращаться обратно от серверов кэша к источнику HTTP для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="4f185-253">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="4f185-254">Допустимые значения: от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="4f185-254">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="4f185-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f185-255">Response</span></span>
<span data-ttu-id="4f185-256">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f185-256">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f185-257">Пример</span><span class="sxs-lookup"><span data-stu-id="4f185-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f185-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f185-258">Request</span></span>
<span data-ttu-id="4f185-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f185-259">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f185-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f185-260">Response</span></span>
<span data-ttu-id="4f185-p130">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f185-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





