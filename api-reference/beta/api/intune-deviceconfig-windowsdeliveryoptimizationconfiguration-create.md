---
title: Создание windowsDeliveryOptimizationConfiguration
description: Создайте новый объект WindowsDeliveryOptimizationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21298ccc592f2b80868bbe68393f5fdf9223f055
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132424"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="4b178-103">Создание windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b178-103">Create windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="4b178-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b178-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b178-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b178-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b178-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b178-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b178-107">Создайте [новый объект WindowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b178-107">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b178-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b178-108">Prerequisites</span></span>
<span data-ttu-id="4b178-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b178-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b178-111">Permission type</span></span>|<span data-ttu-id="4b178-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b178-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b178-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b178-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b178-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b178-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b178-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b178-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b178-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b178-116">Not supported.</span></span>|
|<span data-ttu-id="4b178-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4b178-117">Application</span></span>|<span data-ttu-id="4b178-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b178-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b178-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b178-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b178-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b178-120">Request headers</span></span>
|<span data-ttu-id="4b178-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b178-121">Header</span></span>|<span data-ttu-id="4b178-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b178-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b178-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b178-123">Authorization</span></span>|<span data-ttu-id="4b178-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b178-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b178-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b178-125">Accept</span></span>|<span data-ttu-id="4b178-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b178-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b178-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b178-127">Request body</span></span>
<span data-ttu-id="4b178-128">В теле запроса поставляем представление JSON для объекта WindowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4b178-128">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="4b178-129">В следующей таблице показаны свойства, необходимые при создании windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4b178-129">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="4b178-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b178-130">Property</span></span>|<span data-ttu-id="4b178-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b178-131">Type</span></span>|<span data-ttu-id="4b178-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b178-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b178-133">id</span><span class="sxs-lookup"><span data-stu-id="4b178-133">id</span></span>|<span data-ttu-id="4b178-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4b178-134">String</span></span>|<span data-ttu-id="4b178-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-135">Key of the entity.</span></span> <span data-ttu-id="4b178-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b178-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4b178-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b178-138">DateTimeOffset</span></span>|<span data-ttu-id="4b178-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4b178-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b178-141">roleScopeTagIds</span></span>|<span data-ttu-id="4b178-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b178-142">String collection</span></span>|<span data-ttu-id="4b178-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4b178-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b178-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4b178-145">supportsScopeTags</span></span>|<span data-ttu-id="4b178-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b178-146">Boolean</span></span>|<span data-ttu-id="4b178-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4b178-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b178-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="4b178-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b178-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4b178-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b178-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b178-150">This property is read-only.</span></span> <span data-ttu-id="4b178-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b178-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4b178-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b178-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4b178-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b178-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4b178-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b178-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4b178-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b178-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4b178-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b178-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4b178-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b178-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4b178-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b178-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4b178-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b178-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4b178-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b178-164">createdDateTime</span></span>|<span data-ttu-id="4b178-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b178-165">DateTimeOffset</span></span>|<span data-ttu-id="4b178-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b178-166">DateTime the object was created.</span></span> <span data-ttu-id="4b178-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-168">description</span><span class="sxs-lookup"><span data-stu-id="4b178-168">description</span></span>|<span data-ttu-id="4b178-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4b178-169">String</span></span>|<span data-ttu-id="4b178-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b178-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b178-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4b178-172">displayName</span></span>|<span data-ttu-id="4b178-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4b178-173">String</span></span>|<span data-ttu-id="4b178-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b178-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b178-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-176">version</span><span class="sxs-lookup"><span data-stu-id="4b178-176">version</span></span>|<span data-ttu-id="4b178-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-177">Int32</span></span>|<span data-ttu-id="4b178-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b178-178">Version of the device configuration.</span></span> <span data-ttu-id="4b178-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b178-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b178-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4b178-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="4b178-181">WindowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4b178-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="4b178-182">Указывает метод загрузки, который оптимизация доставки может использовать для управления потреблением пропускной способности сети для больших сценариев распространения контента.</span><span class="sxs-lookup"><span data-stu-id="4b178-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="4b178-183">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="4b178-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="4b178-184">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="4b178-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="4b178-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="4b178-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="4b178-186">Указывает ограничение выбора одноранговых рангов с помощью выбранного параметра.</span><span class="sxs-lookup"><span data-stu-id="4b178-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="4b178-187">Параметр 1 (маска subnet) применяется только к режимам оптимизации доставки Режим загрузки LAN (1) и Group (2).</span><span class="sxs-lookup"><span data-stu-id="4b178-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="4b178-188">Возможные значения: `notConfigured`, `subnetMask`.</span><span class="sxs-lookup"><span data-stu-id="4b178-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="4b178-189">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="4b178-189">groupIdSource</span></span>|[<span data-ttu-id="4b178-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="4b178-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="4b178-191">Указывает ограничение выбора одноранговых рангов на спектральный источник.</span><span class="sxs-lookup"><span data-stu-id="4b178-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="4b178-192">Параметры, задаемые в этой политике, применяются только к режиму загрузки Группы оптимизации доставки (2).</span><span class="sxs-lookup"><span data-stu-id="4b178-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="4b178-193">Если group (2) не заданной как режим загрузки, эта политика будет проигнорирована.</span><span class="sxs-lookup"><span data-stu-id="4b178-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="4b178-194">Для параметра 3 — DHCP Option ID клиент запрашивает ID параметра DHCP 234 и использует возвращенное значение GUID в качестве группового ID.</span><span class="sxs-lookup"><span data-stu-id="4b178-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="4b178-195">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="4b178-195">bandwidthMode</span></span>|[<span data-ttu-id="4b178-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="4b178-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="4b178-197">Указывает использование переднего плана и фоновой пропускной способности с использованием процентов, абсолютов или часов.</span><span class="sxs-lookup"><span data-stu-id="4b178-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="4b178-198">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="4b178-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="4b178-199">Int64</span><span class="sxs-lookup"><span data-stu-id="4b178-199">Int64</span></span>|<span data-ttu-id="4b178-200">Указывает количество секунд для задержки источника HTTP в фоновом режиме загрузки, разрешенного для одноранговой загрузки.</span><span class="sxs-lookup"><span data-stu-id="4b178-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="4b178-201">Допустимые значения от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="4b178-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="4b178-202">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="4b178-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="4b178-203">Int64</span><span class="sxs-lookup"><span data-stu-id="4b178-203">Int64</span></span>|<span data-ttu-id="4b178-204">Указывает количество секунд для задержки источника HTTP в переднем плане загрузки, разрешенной для одноранговой загрузки (0-86400).</span><span class="sxs-lookup"><span data-stu-id="4b178-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="4b178-205">Допустимые значения от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="4b178-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="4b178-206">Указание 0 наборов Оптимизация доставки для управления этим параметром с помощью облачной службы.</span><span class="sxs-lookup"><span data-stu-id="4b178-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="4b178-207">Допустимые значения от 0 до 86400</span><span class="sxs-lookup"><span data-stu-id="4b178-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="4b178-208">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="4b178-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="4b178-209">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-209">Int32</span></span>|<span data-ttu-id="4b178-210">Указывает минимальный размер оперативной памяти в ГБ для использования одноранговой кэшинг (1-100000).</span><span class="sxs-lookup"><span data-stu-id="4b178-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4b178-211">Допустимые значения от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4b178-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4b178-212">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="4b178-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="4b178-213">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-213">Int32</span></span>|<span data-ttu-id="4b178-214">Указывает минимальный размер диска в ГБ для использования одноранговой кэшинг (1-100000).</span><span class="sxs-lookup"><span data-stu-id="4b178-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4b178-215">Допустимые значения от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4b178-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="4b178-216">Рекомендуемые значения: от 64 ГБ до 256 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4b178-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="4b178-217">Допустимые значения от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4b178-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4b178-218">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="4b178-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="4b178-219">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-219">Int32</span></span>|<span data-ttu-id="4b178-220">Указывает минимальный размер файла контента в МБ, с возможностью использования одноранговой кэшинг (1-100000).</span><span class="sxs-lookup"><span data-stu-id="4b178-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="4b178-221">Допустимые значения от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4b178-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="4b178-222">Рекомендуемые значения: от 1 МБ до 100 000 МБ.</span><span class="sxs-lookup"><span data-stu-id="4b178-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="4b178-223">Допустимые значения от 1 до 100000</span><span class="sxs-lookup"><span data-stu-id="4b178-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="4b178-224">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="4b178-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="4b178-225">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-225">Int32</span></span>|<span data-ttu-id="4b178-226">Указывает минимальный процент заряда батареи, позволяющий устройству загружать данные (0-100).</span><span class="sxs-lookup"><span data-stu-id="4b178-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="4b178-227">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4b178-227">Valid values 0 to 100</span></span>
<span data-ttu-id="4b178-228">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="4b178-228">The default value is 0.</span></span> <span data-ttu-id="4b178-229">Значение 0 (ноль) означает "не ограничено", и будет использоваться значение по умолчанию облачной службы.</span><span class="sxs-lookup"><span data-stu-id="4b178-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="4b178-230">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="4b178-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4b178-231">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="4b178-231">modifyCacheLocation</span></span>|<span data-ttu-id="4b178-232">Строка</span><span class="sxs-lookup"><span data-stu-id="4b178-232">String</span></span>|<span data-ttu-id="4b178-233">Указывает диск, который оптимизация доставки должна использовать для кэша.</span><span class="sxs-lookup"><span data-stu-id="4b178-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="4b178-234">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="4b178-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="4b178-235">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-235">Int32</span></span>|<span data-ttu-id="4b178-236">Указывает максимальное время в днях, когда каждый файл находится в кэше оптимизации доставки после успешной загрузки (0-3650).</span><span class="sxs-lookup"><span data-stu-id="4b178-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="4b178-237">Допустимые значения от 0 до 3650</span><span class="sxs-lookup"><span data-stu-id="4b178-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="4b178-238">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="4b178-238">maximumCacheSize</span></span>|[<span data-ttu-id="4b178-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="4b178-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="4b178-240">Указывает максимальный размер кэша, который будет оптимизирован для доставки в процентах или в ГБ.</span><span class="sxs-lookup"><span data-stu-id="4b178-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="4b178-241">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="4b178-241">vpnPeerCaching</span></span>|[<span data-ttu-id="4b178-242">включить</span><span class="sxs-lookup"><span data-stu-id="4b178-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4b178-243">Указывает, разрешено ли устройству участвовать в кэшинге одноранговых устройств при под подключении через VPN к доменной сети.</span><span class="sxs-lookup"><span data-stu-id="4b178-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="4b178-244">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4b178-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4b178-245">cacheServerHostNames</span><span class="sxs-lookup"><span data-stu-id="4b178-245">cacheServerHostNames</span></span>|<span data-ttu-id="4b178-246">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b178-246">String collection</span></span>|<span data-ttu-id="4b178-247">Указывает имена хост-серверов кэша.</span><span class="sxs-lookup"><span data-stu-id="4b178-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="4b178-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="4b178-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="4b178-249">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-249">Int32</span></span>|<span data-ttu-id="4b178-250">Указывает количество секунд для задержки обратного падения с серверов кэша на источник HTTP для загрузки на переднем плане.</span><span class="sxs-lookup"><span data-stu-id="4b178-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="4b178-251">Допустимые значения от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="4b178-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="4b178-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="4b178-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="4b178-253">Int32</span><span class="sxs-lookup"><span data-stu-id="4b178-253">Int32</span></span>|<span data-ttu-id="4b178-254">Указывает количество секунд для задержки обратного падения с серверов кэша на источник HTTP для фоновой загрузки.</span><span class="sxs-lookup"><span data-stu-id="4b178-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="4b178-255">Допустимые значения от 0 до 2592000.</span><span class="sxs-lookup"><span data-stu-id="4b178-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="4b178-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b178-256">Response</span></span>
<span data-ttu-id="4b178-257">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b178-257">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b178-258">Пример</span><span class="sxs-lookup"><span data-stu-id="4b178-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b178-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b178-259">Request</span></span>
<span data-ttu-id="4b178-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b178-260">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b178-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b178-261">Response</span></span>
<span data-ttu-id="4b178-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b178-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




