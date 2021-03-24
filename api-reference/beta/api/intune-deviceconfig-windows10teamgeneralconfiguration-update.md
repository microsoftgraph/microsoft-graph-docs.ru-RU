---
title: Обновление windows10TeamGeneralConfiguration
description: Обновление свойств объекта windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d988bd6bc5841c721650440a868eeb1e08449419
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127370"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="7d3fd-103">Обновление windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d3fd-103">Update windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="7d3fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d3fd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d3fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d3fd-107">Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-107">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d3fd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d3fd-108">Prerequisites</span></span>
<span data-ttu-id="7d3fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d3fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d3fd-111">Permission type</span></span>|<span data-ttu-id="7d3fd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d3fd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d3fd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d3fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d3fd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3fd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d3fd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d3fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d3fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-116">Not supported.</span></span>|
|<span data-ttu-id="7d3fd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d3fd-117">Application</span></span>|<span data-ttu-id="7d3fd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3fd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d3fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d3fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7d3fd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d3fd-120">Request headers</span></span>
|<span data-ttu-id="7d3fd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d3fd-121">Header</span></span>|<span data-ttu-id="7d3fd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d3fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d3fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d3fd-123">Authorization</span></span>|<span data-ttu-id="7d3fd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d3fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d3fd-125">Accept</span></span>|<span data-ttu-id="7d3fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d3fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d3fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d3fd-127">Request body</span></span>
<span data-ttu-id="7d3fd-128">В теле запроса добавьте представление объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-128">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="7d3fd-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-129">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="7d3fd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d3fd-130">Property</span></span>|<span data-ttu-id="7d3fd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7d3fd-131">Type</span></span>|<span data-ttu-id="7d3fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7d3fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d3fd-133">id</span><span class="sxs-lookup"><span data-stu-id="7d3fd-133">id</span></span>|<span data-ttu-id="7d3fd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7d3fd-134">String</span></span>|<span data-ttu-id="7d3fd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-135">Key of the entity.</span></span> <span data-ttu-id="7d3fd-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d3fd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7d3fd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d3fd-138">DateTimeOffset</span></span>|<span data-ttu-id="7d3fd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7d3fd-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d3fd-141">roleScopeTagIds</span></span>|<span data-ttu-id="7d3fd-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7d3fd-142">String collection</span></span>|<span data-ttu-id="7d3fd-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d3fd-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d3fd-145">supportsScopeTags</span></span>|<span data-ttu-id="7d3fd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-146">Boolean</span></span>|<span data-ttu-id="7d3fd-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d3fd-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d3fd-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d3fd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-150">This property is read-only.</span></span> <span data-ttu-id="7d3fd-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7d3fd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7d3fd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7d3fd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7d3fd-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7d3fd-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7d3fd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7d3fd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7d3fd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7d3fd-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7d3fd-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7d3fd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7d3fd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7d3fd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7d3fd-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7d3fd-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d3fd-164">createdDateTime</span></span>|<span data-ttu-id="7d3fd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d3fd-165">DateTimeOffset</span></span>|<span data-ttu-id="7d3fd-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-166">DateTime the object was created.</span></span> <span data-ttu-id="7d3fd-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-168">description</span><span class="sxs-lookup"><span data-stu-id="7d3fd-168">description</span></span>|<span data-ttu-id="7d3fd-169">Строка</span><span class="sxs-lookup"><span data-stu-id="7d3fd-169">String</span></span>|<span data-ttu-id="7d3fd-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d3fd-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7d3fd-172">displayName</span></span>|<span data-ttu-id="7d3fd-173">Строка</span><span class="sxs-lookup"><span data-stu-id="7d3fd-173">String</span></span>|<span data-ttu-id="7d3fd-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d3fd-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-176">version</span><span class="sxs-lookup"><span data-stu-id="7d3fd-176">version</span></span>|<span data-ttu-id="7d3fd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3fd-177">Int32</span></span>|<span data-ttu-id="7d3fd-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-178">Version of the device configuration.</span></span> <span data-ttu-id="7d3fd-179">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d3fd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d3fd-180">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="7d3fd-180">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="7d3fd-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-181">Boolean</span></span>|<span data-ttu-id="7d3fd-182">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-182">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="7d3fd-183">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="7d3fd-183">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="7d3fd-184">String</span><span class="sxs-lookup"><span data-stu-id="7d3fd-184">String</span></span>|<span data-ttu-id="7d3fd-185">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-185">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="7d3fd-186">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="7d3fd-186">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="7d3fd-187">String</span><span class="sxs-lookup"><span data-stu-id="7d3fd-187">String</span></span>|<span data-ttu-id="7d3fd-188">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-188">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="7d3fd-189">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="7d3fd-189">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="7d3fd-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-190">Boolean</span></span>|<span data-ttu-id="7d3fd-191">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-191">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="7d3fd-192">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="7d3fd-192">maintenanceWindowBlocked</span></span>|<span data-ttu-id="7d3fd-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-193">Boolean</span></span>|<span data-ttu-id="7d3fd-194">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-194">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="7d3fd-195">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="7d3fd-195">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="7d3fd-196">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3fd-196">Int32</span></span>|<span data-ttu-id="7d3fd-197">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-197">Maintenance window duration for device updates.</span></span> <span data-ttu-id="7d3fd-198">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="7d3fd-198">Valid values 0 to 5</span></span>|
|<span data-ttu-id="7d3fd-199">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="7d3fd-199">maintenanceWindowStartTime</span></span>|<span data-ttu-id="7d3fd-200">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7d3fd-200">TimeOfDay</span></span>|<span data-ttu-id="7d3fd-201">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-201">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="7d3fd-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="7d3fd-202">miracastChannel</span></span>|[<span data-ttu-id="7d3fd-203">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="7d3fd-203">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="7d3fd-204">Канал.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-204">The channel.</span></span> <span data-ttu-id="7d3fd-205">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-205">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="7d3fd-206">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="7d3fd-206">miracastBlocked</span></span>|<span data-ttu-id="7d3fd-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-207">Boolean</span></span>|<span data-ttu-id="7d3fd-208">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-208">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="7d3fd-209">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="7d3fd-209">miracastRequirePin</span></span>|<span data-ttu-id="7d3fd-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-210">Boolean</span></span>|<span data-ttu-id="7d3fd-211">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-211">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="7d3fd-212">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="7d3fd-212">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="7d3fd-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-213">Boolean</span></span>|<span data-ttu-id="7d3fd-214">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-214">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="7d3fd-215">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="7d3fd-215">settingsBlockSessionResume</span></span>|<span data-ttu-id="7d3fd-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-216">Boolean</span></span>|<span data-ttu-id="7d3fd-217">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-217">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="7d3fd-218">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="7d3fd-218">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="7d3fd-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-219">Boolean</span></span>|<span data-ttu-id="7d3fd-220">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-220">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="7d3fd-221">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="7d3fd-221">settingsDefaultVolume</span></span>|<span data-ttu-id="7d3fd-222">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3fd-222">Int32</span></span>|<span data-ttu-id="7d3fd-223">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-223">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="7d3fd-224">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-224">Permitted values are 0-100.</span></span> <span data-ttu-id="7d3fd-225">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-225">The default is 45.</span></span> <span data-ttu-id="7d3fd-226">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="7d3fd-226">Valid values 0 to 100</span></span>|
|<span data-ttu-id="7d3fd-227">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7d3fd-227">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="7d3fd-228">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3fd-228">Int32</span></span>|<span data-ttu-id="7d3fd-229">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-229">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="7d3fd-230">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7d3fd-230">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="7d3fd-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3fd-231">Int32</span></span>|<span data-ttu-id="7d3fd-232">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-232">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="7d3fd-233">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7d3fd-233">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="7d3fd-234">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3fd-234">Int32</span></span>|<span data-ttu-id="7d3fd-235">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="7d3fd-235">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="7d3fd-236">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="7d3fd-236">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="7d3fd-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3fd-237">Boolean</span></span>|<span data-ttu-id="7d3fd-238">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-238">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="7d3fd-239">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="7d3fd-239">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="7d3fd-240">String</span><span class="sxs-lookup"><span data-stu-id="7d3fd-240">String</span></span>|<span data-ttu-id="7d3fd-241">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-241">The welcome screen background image URL.</span></span> <span data-ttu-id="7d3fd-242">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-242">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="7d3fd-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="7d3fd-243">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="7d3fd-244">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="7d3fd-244">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="7d3fd-245">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-245">The welcome screen meeting information shown.</span></span> <span data-ttu-id="7d3fd-246">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-246">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d3fd-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3fd-247">Response</span></span>
<span data-ttu-id="7d3fd-248">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-248">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d3fd-249">Пример</span><span class="sxs-lookup"><span data-stu-id="7d3fd-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d3fd-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d3fd-250">Request</span></span>
<span data-ttu-id="7d3fd-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-251">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2015

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="7d3fd-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3fd-252">Response</span></span>
<span data-ttu-id="7d3fd-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d3fd-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2187

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```




