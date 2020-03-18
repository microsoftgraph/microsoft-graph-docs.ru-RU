---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2d7cf7268b62410e688a472359bdfbe523429f2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42749125"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="48bcb-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="48bcb-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="48bcb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48bcb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48bcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48bcb-106">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48bcb-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48bcb-107">Prerequisites</span></span>
<span data-ttu-id="48bcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48bcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48bcb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48bcb-110">Permission type</span></span>|<span data-ttu-id="48bcb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48bcb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48bcb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48bcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48bcb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48bcb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48bcb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48bcb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48bcb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bcb-115">Not supported.</span></span>|
|<span data-ttu-id="48bcb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="48bcb-116">Application</span></span>|<span data-ttu-id="48bcb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48bcb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48bcb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48bcb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48bcb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="48bcb-119">Request headers</span></span>
|<span data-ttu-id="48bcb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48bcb-120">Header</span></span>|<span data-ttu-id="48bcb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="48bcb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48bcb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48bcb-122">Authorization</span></span>|<span data-ttu-id="48bcb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48bcb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48bcb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="48bcb-124">Accept</span></span>|<span data-ttu-id="48bcb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48bcb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48bcb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48bcb-126">Request body</span></span>
<span data-ttu-id="48bcb-127">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48bcb-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="48bcb-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="48bcb-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="48bcb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="48bcb-129">Property</span></span>|<span data-ttu-id="48bcb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="48bcb-130">Type</span></span>|<span data-ttu-id="48bcb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="48bcb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48bcb-132">id</span><span class="sxs-lookup"><span data-stu-id="48bcb-132">id</span></span>|<span data-ttu-id="48bcb-133">String</span><span class="sxs-lookup"><span data-stu-id="48bcb-133">String</span></span>|<span data-ttu-id="48bcb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48bcb-134">Key of the entity.</span></span> <span data-ttu-id="48bcb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48bcb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="48bcb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48bcb-137">DateTimeOffset</span></span>|<span data-ttu-id="48bcb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="48bcb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="48bcb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48bcb-140">roleScopeTagIds</span></span>|<span data-ttu-id="48bcb-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="48bcb-141">String collection</span></span>|<span data-ttu-id="48bcb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="48bcb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="48bcb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="48bcb-144">supportsScopeTags</span></span>|<span data-ttu-id="48bcb-145">Логический</span><span class="sxs-lookup"><span data-stu-id="48bcb-145">Boolean</span></span>|<span data-ttu-id="48bcb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="48bcb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="48bcb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="48bcb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="48bcb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="48bcb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="48bcb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48bcb-149">This property is read-only.</span></span> <span data-ttu-id="48bcb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="48bcb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="48bcb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="48bcb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="48bcb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="48bcb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="48bcb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="48bcb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="48bcb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="48bcb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="48bcb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="48bcb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="48bcb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48bcb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="48bcb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48bcb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="48bcb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="48bcb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="48bcb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48bcb-163">createdDateTime</span></span>|<span data-ttu-id="48bcb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48bcb-164">DateTimeOffset</span></span>|<span data-ttu-id="48bcb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="48bcb-165">DateTime the object was created.</span></span> <span data-ttu-id="48bcb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-167">description</span><span class="sxs-lookup"><span data-stu-id="48bcb-167">description</span></span>|<span data-ttu-id="48bcb-168">String</span><span class="sxs-lookup"><span data-stu-id="48bcb-168">String</span></span>|<span data-ttu-id="48bcb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="48bcb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48bcb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="48bcb-171">displayName</span></span>|<span data-ttu-id="48bcb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="48bcb-172">String</span></span>|<span data-ttu-id="48bcb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="48bcb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48bcb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-175">version</span><span class="sxs-lookup"><span data-stu-id="48bcb-175">version</span></span>|<span data-ttu-id="48bcb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="48bcb-176">Int32</span></span>|<span data-ttu-id="48bcb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="48bcb-177">Version of the device configuration.</span></span> <span data-ttu-id="48bcb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48bcb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48bcb-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="48bcb-179">isEnabled</span></span>|<span data-ttu-id="48bcb-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="48bcb-180">Boolean</span></span>|<span data-ttu-id="48bcb-181">Включен параметр в пользовательском интерфейсе</span><span class="sxs-lookup"><span data-stu-id="48bcb-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="48bcb-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="48bcb-182">activeHoursStart</span></span>|<span data-ttu-id="48bcb-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="48bcb-183">TimeOfDay</span></span>|<span data-ttu-id="48bcb-184">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="48bcb-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="48bcb-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="48bcb-185">activeHoursEnd</span></span>|<span data-ttu-id="48bcb-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="48bcb-186">TimeOfDay</span></span>|<span data-ttu-id="48bcb-187">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="48bcb-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="48bcb-188">десиредосверсион</span><span class="sxs-lookup"><span data-stu-id="48bcb-188">desiredOsVersion</span></span>|<span data-ttu-id="48bcb-189">String</span><span class="sxs-lookup"><span data-stu-id="48bcb-189">String</span></span>|<span data-ttu-id="48bcb-190">Если параметр не задан, устройства обновляются до последней версии ОС.</span><span class="sxs-lookup"><span data-stu-id="48bcb-190">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="48bcb-191">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="48bcb-191">scheduledInstallDays</span></span>|<span data-ttu-id="48bcb-192">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="48bcb-192">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="48bcb-193">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="48bcb-193">Days in week for which active hours are configured.</span></span> <span data-ttu-id="48bcb-194">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="48bcb-194">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="48bcb-195">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="48bcb-195">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="48bcb-196">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="48bcb-196">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="48bcb-197">Int32</span><span class="sxs-lookup"><span data-stu-id="48bcb-197">Int32</span></span>|<span data-ttu-id="48bcb-198">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="48bcb-198">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="48bcb-199">енфорцедсофтвареупдатеделайиндайс</span><span class="sxs-lookup"><span data-stu-id="48bcb-199">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="48bcb-200">Int32</span><span class="sxs-lookup"><span data-stu-id="48bcb-200">Int32</span></span>|<span data-ttu-id="48bcb-201">Дней до отображения обновлений программного обеспечения для устройств с iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="48bcb-201">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="48bcb-202">упдатесчедулетипе</span><span class="sxs-lookup"><span data-stu-id="48bcb-202">updateScheduleType</span></span>|[<span data-ttu-id="48bcb-203">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="48bcb-203">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="48bcb-204">Обновление типа расписания.</span><span class="sxs-lookup"><span data-stu-id="48bcb-204">Update schedule type.</span></span> <span data-ttu-id="48bcb-205">Возможные значения: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="48bcb-205">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="48bcb-206">кустомупдатетимевиндовс</span><span class="sxs-lookup"><span data-stu-id="48bcb-206">customUpdateTimeWindows</span></span>|<span data-ttu-id="48bcb-207">Коллекция [кустомупдатетимевиндов](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="48bcb-207">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="48bcb-208">Если для типа расписания обновлений задано значение использовать расписание окна, настраиваемое время, когда будут планироваться обновления.</span><span class="sxs-lookup"><span data-stu-id="48bcb-208">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="48bcb-209">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="48bcb-209">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="48bcb-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="48bcb-210">Response</span></span>
<span data-ttu-id="48bcb-211">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48bcb-211">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48bcb-212">Пример</span><span class="sxs-lookup"><span data-stu-id="48bcb-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="48bcb-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="48bcb-213">Request</span></span>
<span data-ttu-id="48bcb-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48bcb-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="48bcb-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="48bcb-215">Response</span></span>
<span data-ttu-id="48bcb-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48bcb-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




