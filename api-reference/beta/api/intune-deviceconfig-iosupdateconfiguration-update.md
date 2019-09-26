---
title: Обновление объекта iosUpdateConfiguration
description: Обновление свойств объекта iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3340475f58211c6e14a4837311f79d72aa724088
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179161"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="d60aa-103">Обновление объекта iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="d60aa-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="d60aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d60aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d60aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d60aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d60aa-106">Обновление свойств объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d60aa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d60aa-107">Prerequisites</span></span>
<span data-ttu-id="d60aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d60aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d60aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d60aa-110">Permission type</span></span>|<span data-ttu-id="d60aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d60aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d60aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d60aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d60aa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60aa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d60aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d60aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d60aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d60aa-115">Not supported.</span></span>|
|<span data-ttu-id="d60aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d60aa-116">Application</span></span>|<span data-ttu-id="d60aa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60aa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d60aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d60aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d60aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d60aa-119">Request headers</span></span>
|<span data-ttu-id="d60aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d60aa-120">Header</span></span>|<span data-ttu-id="d60aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d60aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d60aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d60aa-122">Authorization</span></span>|<span data-ttu-id="d60aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d60aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d60aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d60aa-124">Accept</span></span>|<span data-ttu-id="d60aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d60aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d60aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d60aa-126">Request body</span></span>
<span data-ttu-id="d60aa-127">В теле запроса добавьте представление объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d60aa-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="d60aa-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="d60aa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d60aa-129">Property</span></span>|<span data-ttu-id="d60aa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d60aa-130">Type</span></span>|<span data-ttu-id="d60aa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d60aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d60aa-132">id</span><span class="sxs-lookup"><span data-stu-id="d60aa-132">id</span></span>|<span data-ttu-id="d60aa-133">String</span><span class="sxs-lookup"><span data-stu-id="d60aa-133">String</span></span>|<span data-ttu-id="d60aa-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d60aa-134">Key of the entity.</span></span> <span data-ttu-id="d60aa-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d60aa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d60aa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d60aa-137">DateTimeOffset</span></span>|<span data-ttu-id="d60aa-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d60aa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d60aa-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d60aa-140">roleScopeTagIds</span></span>|<span data-ttu-id="d60aa-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d60aa-141">String collection</span></span>|<span data-ttu-id="d60aa-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d60aa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d60aa-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d60aa-144">supportsScopeTags</span></span>|<span data-ttu-id="d60aa-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="d60aa-145">Boolean</span></span>|<span data-ttu-id="d60aa-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d60aa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d60aa-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d60aa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d60aa-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d60aa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d60aa-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d60aa-149">This property is read-only.</span></span> <span data-ttu-id="d60aa-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d60aa-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d60aa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d60aa-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d60aa-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d60aa-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d60aa-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d60aa-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d60aa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d60aa-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d60aa-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d60aa-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d60aa-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d60aa-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d60aa-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d60aa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d60aa-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d60aa-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d60aa-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d60aa-163">createdDateTime</span></span>|<span data-ttu-id="d60aa-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d60aa-164">DateTimeOffset</span></span>|<span data-ttu-id="d60aa-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d60aa-165">DateTime the object was created.</span></span> <span data-ttu-id="d60aa-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-167">description</span><span class="sxs-lookup"><span data-stu-id="d60aa-167">description</span></span>|<span data-ttu-id="d60aa-168">String</span><span class="sxs-lookup"><span data-stu-id="d60aa-168">String</span></span>|<span data-ttu-id="d60aa-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d60aa-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d60aa-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d60aa-171">displayName</span></span>|<span data-ttu-id="d60aa-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d60aa-172">String</span></span>|<span data-ttu-id="d60aa-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d60aa-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d60aa-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-175">version</span><span class="sxs-lookup"><span data-stu-id="d60aa-175">version</span></span>|<span data-ttu-id="d60aa-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d60aa-176">Int32</span></span>|<span data-ttu-id="d60aa-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d60aa-177">Version of the device configuration.</span></span> <span data-ttu-id="d60aa-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d60aa-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d60aa-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d60aa-179">isEnabled</span></span>|<span data-ttu-id="d60aa-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d60aa-180">Boolean</span></span>|<span data-ttu-id="d60aa-181">Включен параметр в пользовательском интерфейсе</span><span class="sxs-lookup"><span data-stu-id="d60aa-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="d60aa-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d60aa-182">activeHoursStart</span></span>|<span data-ttu-id="d60aa-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d60aa-183">TimeOfDay</span></span>|<span data-ttu-id="d60aa-184">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="d60aa-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="d60aa-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d60aa-185">activeHoursEnd</span></span>|<span data-ttu-id="d60aa-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d60aa-186">TimeOfDay</span></span>|<span data-ttu-id="d60aa-187">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="d60aa-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="d60aa-188">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="d60aa-188">scheduledInstallDays</span></span>|<span data-ttu-id="d60aa-189">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="d60aa-189">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="d60aa-190">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="d60aa-190">Days in week for which active hours are configured.</span></span> <span data-ttu-id="d60aa-191">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="d60aa-191">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="d60aa-192">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="d60aa-192">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d60aa-193">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="d60aa-193">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="d60aa-194">Int32</span><span class="sxs-lookup"><span data-stu-id="d60aa-194">Int32</span></span>|<span data-ttu-id="d60aa-195">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="d60aa-195">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="d60aa-196">енфорцедсофтвареупдатеделайиндайс</span><span class="sxs-lookup"><span data-stu-id="d60aa-196">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="d60aa-197">Int32</span><span class="sxs-lookup"><span data-stu-id="d60aa-197">Int32</span></span>|<span data-ttu-id="d60aa-198">Дней до отображения обновлений программного обеспечения для устройств с iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="d60aa-198">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="d60aa-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="d60aa-199">Response</span></span>
<span data-ttu-id="d60aa-200">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d60aa-200">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d60aa-201">Пример</span><span class="sxs-lookup"><span data-stu-id="d60aa-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="d60aa-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="d60aa-202">Request</span></span>
<span data-ttu-id="d60aa-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d60aa-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1255

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
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="d60aa-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="d60aa-204">Response</span></span>
<span data-ttu-id="d60aa-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d60aa-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1427

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
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```




