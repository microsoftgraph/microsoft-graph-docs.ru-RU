---
title: Создание Макоссофтвареупдатеконфигуратион
description: Создание нового объекта Макоссофтвареупдатеконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ccfe7f0dc7fc8f25899bcc3afba09f81993daa2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236444"
---
# <a name="create-macossoftwareupdateconfiguration"></a><span data-ttu-id="b8792-103">Создание Макоссофтвареупдатеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b8792-103">Create macOSSoftwareUpdateConfiguration</span></span>

<span data-ttu-id="b8792-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8792-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8792-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8792-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8792-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8792-107">Создание нового объекта [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b8792-107">Create a new [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8792-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8792-108">Prerequisites</span></span>
<span data-ttu-id="b8792-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8792-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8792-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8792-111">Permission type</span></span>|<span data-ttu-id="b8792-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8792-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8792-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8792-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8792-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8792-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8792-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8792-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8792-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8792-116">Not supported.</span></span>|
|<span data-ttu-id="b8792-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8792-117">Application</span></span>|<span data-ttu-id="b8792-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8792-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8792-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8792-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8792-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b8792-120">Request headers</span></span>
|<span data-ttu-id="b8792-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8792-121">Header</span></span>|<span data-ttu-id="b8792-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8792-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8792-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8792-123">Authorization</span></span>|<span data-ttu-id="b8792-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8792-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8792-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8792-125">Accept</span></span>|<span data-ttu-id="b8792-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8792-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8792-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8792-127">Request body</span></span>
<span data-ttu-id="b8792-128">В тексте запроса добавьте представление объекта Макоссофтвареупдатеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8792-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateConfiguration object.</span></span>

<span data-ttu-id="b8792-129">В следующей таблице приведены свойства, необходимые при создании Макоссофтвареупдатеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="b8792-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateConfiguration.</span></span>

|<span data-ttu-id="b8792-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8792-130">Property</span></span>|<span data-ttu-id="b8792-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b8792-131">Type</span></span>|<span data-ttu-id="b8792-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b8792-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8792-133">id</span><span class="sxs-lookup"><span data-stu-id="b8792-133">id</span></span>|<span data-ttu-id="b8792-134">String</span><span class="sxs-lookup"><span data-stu-id="b8792-134">String</span></span>|<span data-ttu-id="b8792-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b8792-135">Key of the entity.</span></span> <span data-ttu-id="b8792-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8792-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8792-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8792-138">DateTimeOffset</span></span>|<span data-ttu-id="b8792-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b8792-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8792-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8792-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8792-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b8792-142">String collection</span></span>|<span data-ttu-id="b8792-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b8792-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8792-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b8792-145">supportsScopeTags</span></span>|<span data-ttu-id="b8792-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8792-146">Boolean</span></span>|<span data-ttu-id="b8792-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b8792-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8792-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b8792-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8792-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b8792-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8792-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8792-150">This property is read-only.</span></span> <span data-ttu-id="b8792-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8792-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b8792-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8792-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b8792-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b8792-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b8792-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8792-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b8792-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8792-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b8792-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b8792-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b8792-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8792-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b8792-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8792-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b8792-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b8792-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b8792-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8792-164">createdDateTime</span></span>|<span data-ttu-id="b8792-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8792-165">DateTimeOffset</span></span>|<span data-ttu-id="b8792-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b8792-166">DateTime the object was created.</span></span> <span data-ttu-id="b8792-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-168">description</span><span class="sxs-lookup"><span data-stu-id="b8792-168">description</span></span>|<span data-ttu-id="b8792-169">String</span><span class="sxs-lookup"><span data-stu-id="b8792-169">String</span></span>|<span data-ttu-id="b8792-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8792-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8792-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b8792-172">displayName</span></span>|<span data-ttu-id="b8792-173">String</span><span class="sxs-lookup"><span data-stu-id="b8792-173">String</span></span>|<span data-ttu-id="b8792-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8792-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8792-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-176">version</span><span class="sxs-lookup"><span data-stu-id="b8792-176">version</span></span>|<span data-ttu-id="b8792-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b8792-177">Int32</span></span>|<span data-ttu-id="b8792-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8792-178">Version of the device configuration.</span></span> <span data-ttu-id="b8792-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8792-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8792-180">критикалупдатебехавиор</span><span class="sxs-lookup"><span data-stu-id="b8792-180">criticalUpdateBehavior</span></span>|[<span data-ttu-id="b8792-181">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="b8792-181">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="b8792-182">Обновление поведения критических обновлений.</span><span class="sxs-lookup"><span data-stu-id="b8792-182">Update behavior for critical updates.</span></span> <span data-ttu-id="b8792-183">Возможные значения: `notConfigured`, `default`.</span><span class="sxs-lookup"><span data-stu-id="b8792-183">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="b8792-184">конфигдатаупдатебехавиор</span><span class="sxs-lookup"><span data-stu-id="b8792-184">configDataUpdateBehavior</span></span>|[<span data-ttu-id="b8792-185">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="b8792-185">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="b8792-186">Обновление поведения обновлений файлов данных конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b8792-186">Update behavior for configuration data file updates.</span></span> <span data-ttu-id="b8792-187">Возможные значения: `notConfigured`, `default`.</span><span class="sxs-lookup"><span data-stu-id="b8792-187">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="b8792-188">фирмвареупдатебехавиор</span><span class="sxs-lookup"><span data-stu-id="b8792-188">firmwareUpdateBehavior</span></span>|[<span data-ttu-id="b8792-189">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="b8792-189">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="b8792-190">Обновление поведения обновлений микропрограммного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="b8792-190">Update behavior for firmware updates.</span></span> <span data-ttu-id="b8792-191">Возможные значения: `notConfigured`, `default`.</span><span class="sxs-lookup"><span data-stu-id="b8792-191">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="b8792-192">аллосерупдатебехавиор</span><span class="sxs-lookup"><span data-stu-id="b8792-192">allOtherUpdateBehavior</span></span>|[<span data-ttu-id="b8792-193">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="b8792-193">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="b8792-194">Обновление поведения для всех остальных обновлений.</span><span class="sxs-lookup"><span data-stu-id="b8792-194">Update behavior for all other updates.</span></span> <span data-ttu-id="b8792-195">Возможные значения: `notConfigured`, `default`.</span><span class="sxs-lookup"><span data-stu-id="b8792-195">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="b8792-196">упдатесчедулетипе</span><span class="sxs-lookup"><span data-stu-id="b8792-196">updateScheduleType</span></span>|[<span data-ttu-id="b8792-197">macOSSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="b8792-197">macOSSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|<span data-ttu-id="b8792-198">Обновление типа расписания.</span><span class="sxs-lookup"><span data-stu-id="b8792-198">Update schedule type.</span></span> <span data-ttu-id="b8792-199">Возможные значения: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span><span class="sxs-lookup"><span data-stu-id="b8792-199">Possible values are: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="b8792-200">кустомупдатетимевиндовс</span><span class="sxs-lookup"><span data-stu-id="b8792-200">customUpdateTimeWindows</span></span>|<span data-ttu-id="b8792-201">Коллекция [кустомупдатетимевиндов](../resources/intune-deviceconfig-customupdatetimewindow.md)</span><span class="sxs-lookup"><span data-stu-id="b8792-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="b8792-202">Настраиваемое время Windows, когда обновления будут разрешены или заблокированы.</span><span class="sxs-lookup"><span data-stu-id="b8792-202">Custom Time windows when updates will be allowed or blocked.</span></span> <span data-ttu-id="b8792-203">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="b8792-203">This collection can contain a maximum of 20 elements.</span></span>|
|<span data-ttu-id="b8792-204">упдатетимевиндовуткоффсетинминутес</span><span class="sxs-lookup"><span data-stu-id="b8792-204">updateTimeWindowUtcOffsetInMinutes</span></span>|<span data-ttu-id="b8792-205">Int32</span><span class="sxs-lookup"><span data-stu-id="b8792-205">Int32</span></span>|<span data-ttu-id="b8792-206">Минуты, указывающие смещение UTC для каждого периода обновления</span><span class="sxs-lookup"><span data-stu-id="b8792-206">Minutes indicating UTC offset for each update time window</span></span>|



## <a name="response"></a><span data-ttu-id="b8792-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8792-207">Response</span></span>
<span data-ttu-id="b8792-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоссофтвареупдатеконфигуратион](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8792-208">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8792-209">Пример</span><span class="sxs-lookup"><span data-stu-id="b8792-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8792-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8792-210">Request</span></span>
<span data-ttu-id="b8792-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8792-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1542

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```

### <a name="response"></a><span data-ttu-id="b8792-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8792-212">Response</span></span>
<span data-ttu-id="b8792-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8792-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1714

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
  "id": "b8e467ac-67ac-b8e4-ac67-e4b8ac67e4b8",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```




