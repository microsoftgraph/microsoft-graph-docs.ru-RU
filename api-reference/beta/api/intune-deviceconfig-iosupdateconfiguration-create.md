---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f6f98ca6710015e8c9cdc1ca70d8a9e3215358c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704443"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="8ec14-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ec14-103">Create iosUpdateConfiguration</span></span>

<span data-ttu-id="8ec14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ec14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ec14-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ec14-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ec14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ec14-107">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ec14-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec14-108">Prerequisites</span></span>
<span data-ttu-id="8ec14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec14-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ec14-111">Permission type</span></span>|<span data-ttu-id="8ec14-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ec14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ec14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ec14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ec14-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec14-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ec14-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ec14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ec14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ec14-116">Not supported.</span></span>|
|<span data-ttu-id="8ec14-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ec14-117">Application</span></span>|<span data-ttu-id="8ec14-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec14-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ec14-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ec14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ec14-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ec14-120">Request headers</span></span>
|<span data-ttu-id="8ec14-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ec14-121">Header</span></span>|<span data-ttu-id="8ec14-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ec14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ec14-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ec14-123">Authorization</span></span>|<span data-ttu-id="8ec14-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ec14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ec14-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ec14-125">Accept</span></span>|<span data-ttu-id="8ec14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ec14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ec14-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ec14-127">Request body</span></span>
<span data-ttu-id="8ec14-128">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ec14-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="8ec14-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8ec14-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="8ec14-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ec14-130">Property</span></span>|<span data-ttu-id="8ec14-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ec14-131">Type</span></span>|<span data-ttu-id="8ec14-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ec14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ec14-133">id</span><span class="sxs-lookup"><span data-stu-id="8ec14-133">id</span></span>|<span data-ttu-id="8ec14-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8ec14-134">String</span></span>|<span data-ttu-id="8ec14-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ec14-135">Key of the entity.</span></span> <span data-ttu-id="8ec14-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec14-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8ec14-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ec14-138">DateTimeOffset</span></span>|<span data-ttu-id="8ec14-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ec14-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8ec14-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ec14-141">roleScopeTagIds</span></span>|<span data-ttu-id="8ec14-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8ec14-142">String collection</span></span>|<span data-ttu-id="8ec14-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8ec14-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ec14-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8ec14-145">supportsScopeTags</span></span>|<span data-ttu-id="8ec14-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8ec14-146">Boolean</span></span>|<span data-ttu-id="8ec14-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8ec14-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ec14-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8ec14-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ec14-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8ec14-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ec14-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ec14-150">This property is read-only.</span></span> <span data-ttu-id="8ec14-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ec14-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8ec14-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ec14-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8ec14-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ec14-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8ec14-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ec14-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8ec14-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ec14-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8ec14-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ec14-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8ec14-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ec14-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8ec14-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ec14-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8ec14-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ec14-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8ec14-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec14-164">createdDateTime</span></span>|<span data-ttu-id="8ec14-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ec14-165">DateTimeOffset</span></span>|<span data-ttu-id="8ec14-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ec14-166">DateTime the object was created.</span></span> <span data-ttu-id="8ec14-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-168">description</span><span class="sxs-lookup"><span data-stu-id="8ec14-168">description</span></span>|<span data-ttu-id="8ec14-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8ec14-169">String</span></span>|<span data-ttu-id="8ec14-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ec14-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ec14-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8ec14-172">displayName</span></span>|<span data-ttu-id="8ec14-173">Строка</span><span class="sxs-lookup"><span data-stu-id="8ec14-173">String</span></span>|<span data-ttu-id="8ec14-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ec14-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ec14-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-176">version</span><span class="sxs-lookup"><span data-stu-id="8ec14-176">version</span></span>|<span data-ttu-id="8ec14-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec14-177">Int32</span></span>|<span data-ttu-id="8ec14-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ec14-178">Version of the device configuration.</span></span> <span data-ttu-id="8ec14-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec14-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec14-180">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8ec14-180">isEnabled</span></span>|<span data-ttu-id="8ec14-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec14-181">Boolean</span></span>|<span data-ttu-id="8ec14-182">Включен параметр в пользовательском интерфейсе</span><span class="sxs-lookup"><span data-stu-id="8ec14-182">Is setting enabled in UI</span></span>|
|<span data-ttu-id="8ec14-183">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8ec14-183">activeHoursStart</span></span>|<span data-ttu-id="8ec14-184">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8ec14-184">TimeOfDay</span></span>|<span data-ttu-id="8ec14-185">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="8ec14-185">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="8ec14-186">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8ec14-186">activeHoursEnd</span></span>|<span data-ttu-id="8ec14-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8ec14-187">TimeOfDay</span></span>|<span data-ttu-id="8ec14-188">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="8ec14-188">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="8ec14-189">десиредосверсион</span><span class="sxs-lookup"><span data-stu-id="8ec14-189">desiredOsVersion</span></span>|<span data-ttu-id="8ec14-190">Строка</span><span class="sxs-lookup"><span data-stu-id="8ec14-190">String</span></span>|<span data-ttu-id="8ec14-191">Если параметр не задан, устройства обновляются до последней версии ОС.</span><span class="sxs-lookup"><span data-stu-id="8ec14-191">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="8ec14-192">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="8ec14-192">scheduledInstallDays</span></span>|<span data-ttu-id="8ec14-193">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="8ec14-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="8ec14-194">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="8ec14-194">Days in week for which active hours are configured.</span></span> <span data-ttu-id="8ec14-195">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ec14-195">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8ec14-196">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="8ec14-196">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8ec14-197">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="8ec14-197">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="8ec14-198">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec14-198">Int32</span></span>|<span data-ttu-id="8ec14-199">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="8ec14-199">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="8ec14-200">енфорцедсофтвареупдатеделайиндайс</span><span class="sxs-lookup"><span data-stu-id="8ec14-200">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="8ec14-201">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec14-201">Int32</span></span>|<span data-ttu-id="8ec14-202">Дней до отображения обновлений программного обеспечения для устройств с iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="8ec14-202">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="8ec14-203">упдатесчедулетипе</span><span class="sxs-lookup"><span data-stu-id="8ec14-203">updateScheduleType</span></span>|[<span data-ttu-id="8ec14-204">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="8ec14-204">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="8ec14-205">Обновление типа расписания.</span><span class="sxs-lookup"><span data-stu-id="8ec14-205">Update schedule type.</span></span> <span data-ttu-id="8ec14-206">Возможные значения: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="8ec14-206">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="8ec14-207">кустомупдатетимевиндовс</span><span class="sxs-lookup"><span data-stu-id="8ec14-207">customUpdateTimeWindows</span></span>|<span data-ttu-id="8ec14-208">Коллекция [кустомупдатетимевиндов](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="8ec14-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="8ec14-209">Если для типа расписания обновлений задано значение использовать расписание окна, настраиваемое время, когда будут планироваться обновления.</span><span class="sxs-lookup"><span data-stu-id="8ec14-209">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="8ec14-210">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ec14-210">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8ec14-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ec14-211">Response</span></span>
<span data-ttu-id="8ec14-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8ec14-212">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ec14-213">Пример</span><span class="sxs-lookup"><span data-stu-id="8ec14-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ec14-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ec14-214">Request</span></span>
<span data-ttu-id="8ec14-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ec14-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ec14-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ec14-216">Response</span></span>
<span data-ttu-id="8ec14-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ec14-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





