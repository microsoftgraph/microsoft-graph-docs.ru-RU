---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2579341d4929d73a61684445c24e32da464f962
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137436"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="8acef-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="8acef-103">Create iosUpdateConfiguration</span></span>

<span data-ttu-id="8acef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8acef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8acef-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8acef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8acef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8acef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8acef-107">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8acef-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8acef-108">Prerequisites</span></span>
<span data-ttu-id="8acef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8acef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8acef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8acef-111">Permission type</span></span>|<span data-ttu-id="8acef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8acef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8acef-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8acef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8acef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8acef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8acef-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8acef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8acef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8acef-116">Not supported.</span></span>|
|<span data-ttu-id="8acef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8acef-117">Application</span></span>|<span data-ttu-id="8acef-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8acef-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8acef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8acef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8acef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8acef-120">Request headers</span></span>
|<span data-ttu-id="8acef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8acef-121">Header</span></span>|<span data-ttu-id="8acef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8acef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8acef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8acef-123">Authorization</span></span>|<span data-ttu-id="8acef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8acef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8acef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8acef-125">Accept</span></span>|<span data-ttu-id="8acef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8acef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8acef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8acef-127">Request body</span></span>
<span data-ttu-id="8acef-128">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8acef-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="8acef-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8acef-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="8acef-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8acef-130">Property</span></span>|<span data-ttu-id="8acef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8acef-131">Type</span></span>|<span data-ttu-id="8acef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8acef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8acef-133">id</span><span class="sxs-lookup"><span data-stu-id="8acef-133">id</span></span>|<span data-ttu-id="8acef-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8acef-134">String</span></span>|<span data-ttu-id="8acef-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8acef-135">Key of the entity.</span></span> <span data-ttu-id="8acef-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8acef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8acef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8acef-138">DateTimeOffset</span></span>|<span data-ttu-id="8acef-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8acef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8acef-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8acef-141">roleScopeTagIds</span></span>|<span data-ttu-id="8acef-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8acef-142">String collection</span></span>|<span data-ttu-id="8acef-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="8acef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8acef-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8acef-145">supportsScopeTags</span></span>|<span data-ttu-id="8acef-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8acef-146">Boolean</span></span>|<span data-ttu-id="8acef-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8acef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8acef-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="8acef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8acef-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8acef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8acef-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8acef-150">This property is read-only.</span></span> <span data-ttu-id="8acef-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8acef-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8acef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8acef-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8acef-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8acef-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8acef-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8acef-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8acef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8acef-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8acef-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8acef-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8acef-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8acef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8acef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8acef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8acef-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8acef-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8acef-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8acef-164">createdDateTime</span></span>|<span data-ttu-id="8acef-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8acef-165">DateTimeOffset</span></span>|<span data-ttu-id="8acef-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8acef-166">DateTime the object was created.</span></span> <span data-ttu-id="8acef-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-168">description</span><span class="sxs-lookup"><span data-stu-id="8acef-168">description</span></span>|<span data-ttu-id="8acef-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8acef-169">String</span></span>|<span data-ttu-id="8acef-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8acef-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8acef-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8acef-172">displayName</span></span>|<span data-ttu-id="8acef-173">Строка</span><span class="sxs-lookup"><span data-stu-id="8acef-173">String</span></span>|<span data-ttu-id="8acef-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8acef-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8acef-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-176">version</span><span class="sxs-lookup"><span data-stu-id="8acef-176">version</span></span>|<span data-ttu-id="8acef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8acef-177">Int32</span></span>|<span data-ttu-id="8acef-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8acef-178">Version of the device configuration.</span></span> <span data-ttu-id="8acef-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8acef-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8acef-180">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8acef-180">isEnabled</span></span>|<span data-ttu-id="8acef-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8acef-181">Boolean</span></span>|<span data-ttu-id="8acef-182">Включено ли параметр в пользовательском интерфейсе</span><span class="sxs-lookup"><span data-stu-id="8acef-182">Is setting enabled in UI</span></span>|
|<span data-ttu-id="8acef-183">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8acef-183">activeHoursStart</span></span>|<span data-ttu-id="8acef-184">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8acef-184">TimeOfDay</span></span>|<span data-ttu-id="8acef-185">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="8acef-185">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="8acef-186">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8acef-186">activeHoursEnd</span></span>|<span data-ttu-id="8acef-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8acef-187">TimeOfDay</span></span>|<span data-ttu-id="8acef-188">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="8acef-188">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="8acef-189">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="8acef-189">desiredOsVersion</span></span>|<span data-ttu-id="8acef-190">Строка</span><span class="sxs-lookup"><span data-stu-id="8acef-190">String</span></span>|<span data-ttu-id="8acef-191">Если оставить неустановленными, устройства будут обновляться до последней версии ОС.</span><span class="sxs-lookup"><span data-stu-id="8acef-191">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="8acef-192">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="8acef-192">scheduledInstallDays</span></span>|<span data-ttu-id="8acef-193">[коллекция dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="8acef-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="8acef-194">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="8acef-194">Days in week for which active hours are configured.</span></span> <span data-ttu-id="8acef-195">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="8acef-195">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8acef-196">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="8acef-196">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8acef-197">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="8acef-197">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="8acef-198">Int32</span><span class="sxs-lookup"><span data-stu-id="8acef-198">Int32</span></span>|<span data-ttu-id="8acef-199">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="8acef-199">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="8acef-200">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="8acef-200">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="8acef-201">Int32</span><span class="sxs-lookup"><span data-stu-id="8acef-201">Int32</span></span>|<span data-ttu-id="8acef-202">За несколько дней до обновления программного обеспечения можно увидеть на устройствах iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="8acef-202">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="8acef-203">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="8acef-203">updateScheduleType</span></span>|[<span data-ttu-id="8acef-204">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="8acef-204">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="8acef-205">Тип расписания обновления.</span><span class="sxs-lookup"><span data-stu-id="8acef-205">Update schedule type.</span></span> <span data-ttu-id="8acef-206">Возможные значения: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="8acef-206">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="8acef-207">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="8acef-207">customUpdateTimeWindows</span></span>|<span data-ttu-id="8acef-208">[настраиваемая коллекцияUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="8acef-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="8acef-209">Если тип расписания обновления настроен на использование планирования окне времени, настраиваемые окна времени при планировании обновлений.</span><span class="sxs-lookup"><span data-stu-id="8acef-209">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="8acef-210">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="8acef-210">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8acef-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="8acef-211">Response</span></span>
<span data-ttu-id="8acef-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8acef-212">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8acef-213">Пример</span><span class="sxs-lookup"><span data-stu-id="8acef-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="8acef-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="8acef-214">Request</span></span>
<span data-ttu-id="8acef-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8acef-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8acef-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="8acef-216">Response</span></span>
<span data-ttu-id="8acef-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8acef-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




