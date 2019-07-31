---
title: Обновление windows10TeamGeneralConfiguration
description: Обновление свойств объекта windows10TeamGeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df6bed0790c9575f818a4ed84f5675de2cfa877f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975188"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="17100-103">Обновление windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="17100-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="17100-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17100-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17100-106">Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17100-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17100-107">Prerequisites</span></span>
<span data-ttu-id="17100-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17100-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17100-110">Permission type</span></span>|<span data-ttu-id="17100-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17100-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17100-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17100-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17100-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17100-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17100-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17100-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17100-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17100-115">Not supported.</span></span>|
|<span data-ttu-id="17100-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17100-116">Application</span></span>|<span data-ttu-id="17100-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17100-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17100-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17100-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="17100-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17100-119">Request headers</span></span>
|<span data-ttu-id="17100-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17100-120">Header</span></span>|<span data-ttu-id="17100-121">Значение</span><span class="sxs-lookup"><span data-stu-id="17100-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17100-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17100-122">Authorization</span></span>|<span data-ttu-id="17100-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17100-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17100-124">Accept</span><span class="sxs-lookup"><span data-stu-id="17100-124">Accept</span></span>|<span data-ttu-id="17100-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17100-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17100-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17100-126">Request body</span></span>
<span data-ttu-id="17100-127">В теле запроса добавьте представление объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17100-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="17100-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="17100-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="17100-129">Property</span></span>|<span data-ttu-id="17100-130">Тип</span><span class="sxs-lookup"><span data-stu-id="17100-130">Type</span></span>|<span data-ttu-id="17100-131">Описание</span><span class="sxs-lookup"><span data-stu-id="17100-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17100-132">id</span><span class="sxs-lookup"><span data-stu-id="17100-132">id</span></span>|<span data-ttu-id="17100-133">Строка</span><span class="sxs-lookup"><span data-stu-id="17100-133">String</span></span>|<span data-ttu-id="17100-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17100-134">Key of the entity.</span></span> <span data-ttu-id="17100-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17100-136">lastModifiedDateTime</span></span>|<span data-ttu-id="17100-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17100-137">DateTimeOffset</span></span>|<span data-ttu-id="17100-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="17100-138">DateTime the object was last modified.</span></span> <span data-ttu-id="17100-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17100-140">roleScopeTagIds</span></span>|<span data-ttu-id="17100-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="17100-141">String collection</span></span>|<span data-ttu-id="17100-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="17100-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17100-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="17100-144">supportsScopeTags</span></span>|<span data-ttu-id="17100-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-145">Boolean</span></span>|<span data-ttu-id="17100-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="17100-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17100-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="17100-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17100-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="17100-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17100-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17100-149">This property is read-only.</span></span> <span data-ttu-id="17100-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17100-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="17100-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17100-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="17100-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="17100-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="17100-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17100-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="17100-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17100-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="17100-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="17100-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="17100-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="17100-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="17100-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="17100-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="17100-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="17100-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="17100-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17100-163">createdDateTime</span></span>|<span data-ttu-id="17100-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17100-164">DateTimeOffset</span></span>|<span data-ttu-id="17100-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="17100-165">DateTime the object was created.</span></span> <span data-ttu-id="17100-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-167">description</span><span class="sxs-lookup"><span data-stu-id="17100-167">description</span></span>|<span data-ttu-id="17100-168">String</span><span class="sxs-lookup"><span data-stu-id="17100-168">String</span></span>|<span data-ttu-id="17100-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17100-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17100-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-171">displayName</span><span class="sxs-lookup"><span data-stu-id="17100-171">displayName</span></span>|<span data-ttu-id="17100-172">Строка</span><span class="sxs-lookup"><span data-stu-id="17100-172">String</span></span>|<span data-ttu-id="17100-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17100-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17100-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17100-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-175">version</span><span class="sxs-lookup"><span data-stu-id="17100-175">version</span></span>|<span data-ttu-id="17100-176">Int32</span><span class="sxs-lookup"><span data-stu-id="17100-176">Int32</span></span>|<span data-ttu-id="17100-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17100-177">Version of the device configuration.</span></span> <span data-ttu-id="17100-178">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17100-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17100-179">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="17100-179">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="17100-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-180">Boolean</span></span>|<span data-ttu-id="17100-181">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="17100-181">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="17100-182">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="17100-182">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="17100-183">String</span><span class="sxs-lookup"><span data-stu-id="17100-183">String</span></span>|<span data-ttu-id="17100-184">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="17100-184">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="17100-185">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="17100-185">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="17100-186">String</span><span class="sxs-lookup"><span data-stu-id="17100-186">String</span></span>|<span data-ttu-id="17100-187">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="17100-187">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="17100-188">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="17100-188">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="17100-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-189">Boolean</span></span>|<span data-ttu-id="17100-190">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="17100-190">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="17100-191">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="17100-191">maintenanceWindowBlocked</span></span>|<span data-ttu-id="17100-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-192">Boolean</span></span>|<span data-ttu-id="17100-193">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="17100-193">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="17100-194">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="17100-194">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="17100-195">Int32</span><span class="sxs-lookup"><span data-stu-id="17100-195">Int32</span></span>|<span data-ttu-id="17100-196">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="17100-196">Maintenance window duration for device updates.</span></span> <span data-ttu-id="17100-197">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="17100-197">Valid values 0 to 5</span></span>|
|<span data-ttu-id="17100-198">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="17100-198">maintenanceWindowStartTime</span></span>|<span data-ttu-id="17100-199">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="17100-199">TimeOfDay</span></span>|<span data-ttu-id="17100-200">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="17100-200">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="17100-201">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="17100-201">miracastChannel</span></span>|[<span data-ttu-id="17100-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="17100-202">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="17100-203">Канал.</span><span class="sxs-lookup"><span data-stu-id="17100-203">The channel.</span></span> <span data-ttu-id="17100-204">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="17100-204">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="17100-205">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="17100-205">miracastBlocked</span></span>|<span data-ttu-id="17100-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-206">Boolean</span></span>|<span data-ttu-id="17100-207">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="17100-207">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="17100-208">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="17100-208">miracastRequirePin</span></span>|<span data-ttu-id="17100-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-209">Boolean</span></span>|<span data-ttu-id="17100-210">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="17100-210">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="17100-211">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="17100-211">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="17100-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-212">Boolean</span></span>|<span data-ttu-id="17100-213">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="17100-213">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="17100-214">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="17100-214">settingsBlockSessionResume</span></span>|<span data-ttu-id="17100-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-215">Boolean</span></span>|<span data-ttu-id="17100-216">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="17100-216">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="17100-217">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="17100-217">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="17100-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-218">Boolean</span></span>|<span data-ttu-id="17100-219">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="17100-219">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="17100-220">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="17100-220">settingsDefaultVolume</span></span>|<span data-ttu-id="17100-221">Int32</span><span class="sxs-lookup"><span data-stu-id="17100-221">Int32</span></span>|<span data-ttu-id="17100-222">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="17100-222">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="17100-223">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="17100-223">Permitted values are 0-100.</span></span> <span data-ttu-id="17100-224">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="17100-224">The default is 45.</span></span> <span data-ttu-id="17100-225">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="17100-225">Valid values 0 to 100</span></span>|
|<span data-ttu-id="17100-226">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="17100-226">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="17100-227">Int32</span><span class="sxs-lookup"><span data-stu-id="17100-227">Int32</span></span>|<span data-ttu-id="17100-228">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="17100-228">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="17100-229">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="17100-229">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="17100-230">Int32</span><span class="sxs-lookup"><span data-stu-id="17100-230">Int32</span></span>|<span data-ttu-id="17100-231">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="17100-231">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="17100-232">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="17100-232">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="17100-233">Int32</span><span class="sxs-lookup"><span data-stu-id="17100-233">Int32</span></span>|<span data-ttu-id="17100-234">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="17100-234">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="17100-235">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="17100-235">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="17100-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="17100-236">Boolean</span></span>|<span data-ttu-id="17100-237">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="17100-237">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="17100-238">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="17100-238">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="17100-239">String</span><span class="sxs-lookup"><span data-stu-id="17100-239">String</span></span>|<span data-ttu-id="17100-240">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="17100-240">The welcome screen background image URL.</span></span> <span data-ttu-id="17100-241">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="17100-241">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="17100-242">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="17100-242">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="17100-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="17100-243">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="17100-244">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="17100-244">The welcome screen meeting information shown.</span></span> <span data-ttu-id="17100-245">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="17100-245">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="17100-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="17100-246">Response</span></span>
<span data-ttu-id="17100-247">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="17100-247">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17100-248">Пример</span><span class="sxs-lookup"><span data-stu-id="17100-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="17100-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="17100-249">Request</span></span>
<span data-ttu-id="17100-250">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17100-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17100-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="17100-251">Response</span></span>
<span data-ttu-id="17100-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17100-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





