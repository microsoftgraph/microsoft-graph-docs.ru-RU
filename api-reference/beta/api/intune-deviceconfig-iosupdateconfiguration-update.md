---
title: Обновление объекта iosUpdateConfiguration
description: Обновление свойств объекта iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40d4ccc57ef3643b778fcc3a031aa4977833e761
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733065"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="7725c-103">Обновление объекта iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="7725c-103">Update iosUpdateConfiguration</span></span>

<span data-ttu-id="7725c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7725c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7725c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7725c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7725c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7725c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7725c-107">Обновление свойств объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-107">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7725c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7725c-108">Prerequisites</span></span>
<span data-ttu-id="7725c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7725c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7725c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7725c-111">Permission type</span></span>|<span data-ttu-id="7725c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7725c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7725c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7725c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7725c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7725c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7725c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7725c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7725c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7725c-116">Not supported.</span></span>|
|<span data-ttu-id="7725c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7725c-117">Application</span></span>|<span data-ttu-id="7725c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7725c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7725c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7725c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7725c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7725c-120">Request headers</span></span>
|<span data-ttu-id="7725c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7725c-121">Header</span></span>|<span data-ttu-id="7725c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7725c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7725c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7725c-123">Authorization</span></span>|<span data-ttu-id="7725c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7725c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7725c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7725c-125">Accept</span></span>|<span data-ttu-id="7725c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7725c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7725c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7725c-127">Request body</span></span>
<span data-ttu-id="7725c-128">В теле запроса добавьте представление объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7725c-128">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="7725c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-129">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="7725c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7725c-130">Property</span></span>|<span data-ttu-id="7725c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7725c-131">Type</span></span>|<span data-ttu-id="7725c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7725c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7725c-133">id</span><span class="sxs-lookup"><span data-stu-id="7725c-133">id</span></span>|<span data-ttu-id="7725c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7725c-134">String</span></span>|<span data-ttu-id="7725c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7725c-135">Key of the entity.</span></span> <span data-ttu-id="7725c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7725c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7725c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7725c-138">DateTimeOffset</span></span>|<span data-ttu-id="7725c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7725c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7725c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7725c-141">roleScopeTagIds</span></span>|<span data-ttu-id="7725c-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7725c-142">String collection</span></span>|<span data-ttu-id="7725c-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7725c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7725c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7725c-145">supportsScopeTags</span></span>|<span data-ttu-id="7725c-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7725c-146">Boolean</span></span>|<span data-ttu-id="7725c-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7725c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7725c-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7725c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7725c-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7725c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7725c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7725c-150">This property is read-only.</span></span> <span data-ttu-id="7725c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7725c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7725c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7725c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7725c-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7725c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7725c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7725c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7725c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7725c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7725c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7725c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7725c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7725c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7725c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7725c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7725c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7725c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7725c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7725c-164">createdDateTime</span></span>|<span data-ttu-id="7725c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7725c-165">DateTimeOffset</span></span>|<span data-ttu-id="7725c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7725c-166">DateTime the object was created.</span></span> <span data-ttu-id="7725c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-168">description</span><span class="sxs-lookup"><span data-stu-id="7725c-168">description</span></span>|<span data-ttu-id="7725c-169">Строка</span><span class="sxs-lookup"><span data-stu-id="7725c-169">String</span></span>|<span data-ttu-id="7725c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7725c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7725c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7725c-172">displayName</span></span>|<span data-ttu-id="7725c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="7725c-173">String</span></span>|<span data-ttu-id="7725c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7725c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7725c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-176">version</span><span class="sxs-lookup"><span data-stu-id="7725c-176">version</span></span>|<span data-ttu-id="7725c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7725c-177">Int32</span></span>|<span data-ttu-id="7725c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7725c-178">Version of the device configuration.</span></span> <span data-ttu-id="7725c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7725c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7725c-180">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7725c-180">isEnabled</span></span>|<span data-ttu-id="7725c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7725c-181">Boolean</span></span>|<span data-ttu-id="7725c-182">Включен параметр в пользовательском интерфейсе</span><span class="sxs-lookup"><span data-stu-id="7725c-182">Is setting enabled in UI</span></span>|
|<span data-ttu-id="7725c-183">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7725c-183">activeHoursStart</span></span>|<span data-ttu-id="7725c-184">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7725c-184">TimeOfDay</span></span>|<span data-ttu-id="7725c-185">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="7725c-185">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7725c-186">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7725c-186">activeHoursEnd</span></span>|<span data-ttu-id="7725c-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7725c-187">TimeOfDay</span></span>|<span data-ttu-id="7725c-188">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="7725c-188">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="7725c-189">десиредосверсион</span><span class="sxs-lookup"><span data-stu-id="7725c-189">desiredOsVersion</span></span>|<span data-ttu-id="7725c-190">Строка</span><span class="sxs-lookup"><span data-stu-id="7725c-190">String</span></span>|<span data-ttu-id="7725c-191">Если параметр не задан, устройства обновляются до последней версии ОС.</span><span class="sxs-lookup"><span data-stu-id="7725c-191">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="7725c-192">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="7725c-192">scheduledInstallDays</span></span>|<span data-ttu-id="7725c-193">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="7725c-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="7725c-194">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="7725c-194">Days in week for which active hours are configured.</span></span> <span data-ttu-id="7725c-195">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="7725c-195">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="7725c-196">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="7725c-196">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="7725c-197">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="7725c-197">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="7725c-198">Int32</span><span class="sxs-lookup"><span data-stu-id="7725c-198">Int32</span></span>|<span data-ttu-id="7725c-199">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="7725c-199">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="7725c-200">енфорцедсофтвареупдатеделайиндайс</span><span class="sxs-lookup"><span data-stu-id="7725c-200">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="7725c-201">Int32</span><span class="sxs-lookup"><span data-stu-id="7725c-201">Int32</span></span>|<span data-ttu-id="7725c-202">Дней до отображения обновлений программного обеспечения для устройств с iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="7725c-202">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="7725c-203">упдатесчедулетипе</span><span class="sxs-lookup"><span data-stu-id="7725c-203">updateScheduleType</span></span>|[<span data-ttu-id="7725c-204">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="7725c-204">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="7725c-205">Обновление типа расписания.</span><span class="sxs-lookup"><span data-stu-id="7725c-205">Update schedule type.</span></span> <span data-ttu-id="7725c-206">Возможные значения: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="7725c-206">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="7725c-207">кустомупдатетимевиндовс</span><span class="sxs-lookup"><span data-stu-id="7725c-207">customUpdateTimeWindows</span></span>|<span data-ttu-id="7725c-208">Коллекция [кустомупдатетимевиндов](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="7725c-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="7725c-209">Если для типа расписания обновлений задано значение использовать расписание окна, настраиваемое время, когда будут планироваться обновления.</span><span class="sxs-lookup"><span data-stu-id="7725c-209">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="7725c-210">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="7725c-210">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7725c-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="7725c-211">Response</span></span>
<span data-ttu-id="7725c-212">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7725c-212">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7725c-213">Пример</span><span class="sxs-lookup"><span data-stu-id="7725c-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="7725c-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="7725c-214">Request</span></span>
<span data-ttu-id="7725c-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7725c-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1596

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7725c-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="7725c-216">Response</span></span>
<span data-ttu-id="7725c-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7725c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1768

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```





