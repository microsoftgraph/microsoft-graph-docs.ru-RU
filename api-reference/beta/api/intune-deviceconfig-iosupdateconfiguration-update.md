---
title: Обновление объекта iosUpdateConfiguration
description: Обновление свойств объекта iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b69f4334f65541f866da1eb44ccb9ebf8f42b609
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315710"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="a0d60-103">Обновление объекта iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0d60-103">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="a0d60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0d60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0d60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0d60-106">Обновление свойств объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-106">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0d60-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a0d60-107">Prerequisites</span></span>
<span data-ttu-id="a0d60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d60-110">Permission type</span></span>|<span data-ttu-id="a0d60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0d60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0d60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0d60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0d60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0d60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0d60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0d60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d60-115">Not supported.</span></span>|
|<span data-ttu-id="a0d60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0d60-116">Application</span></span>|<span data-ttu-id="a0d60-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d60-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0d60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0d60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a0d60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0d60-119">Request headers</span></span>
|<span data-ttu-id="a0d60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0d60-120">Header</span></span>|<span data-ttu-id="a0d60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a0d60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0d60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0d60-122">Authorization</span></span>|<span data-ttu-id="a0d60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0d60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0d60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a0d60-124">Accept</span></span>|<span data-ttu-id="a0d60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0d60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d60-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0d60-126">Request body</span></span>
<span data-ttu-id="a0d60-127">В теле запроса добавьте представление объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d60-127">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="a0d60-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-128">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="a0d60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0d60-129">Property</span></span>|<span data-ttu-id="a0d60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a0d60-130">Type</span></span>|<span data-ttu-id="a0d60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d60-132">id</span><span class="sxs-lookup"><span data-stu-id="a0d60-132">id</span></span>|<span data-ttu-id="a0d60-133">String</span><span class="sxs-lookup"><span data-stu-id="a0d60-133">String</span></span>|<span data-ttu-id="a0d60-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a0d60-134">Key of the entity.</span></span> <span data-ttu-id="a0d60-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d60-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a0d60-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d60-137">DateTimeOffset</span></span>|<span data-ttu-id="a0d60-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a0d60-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a0d60-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0d60-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0d60-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a0d60-141">String collection</span></span>|<span data-ttu-id="a0d60-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a0d60-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0d60-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a0d60-144">supportsScopeTags</span></span>|<span data-ttu-id="a0d60-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0d60-145">Boolean</span></span>|<span data-ttu-id="a0d60-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a0d60-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0d60-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a0d60-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0d60-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a0d60-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0d60-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0d60-149">This property is read-only.</span></span> <span data-ttu-id="a0d60-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0d60-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a0d60-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0d60-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a0d60-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a0d60-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a0d60-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0d60-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a0d60-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0d60-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a0d60-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a0d60-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a0d60-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="a0d60-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a0d60-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="a0d60-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a0d60-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a0d60-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a0d60-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d60-163">createdDateTime</span></span>|<span data-ttu-id="a0d60-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d60-164">DateTimeOffset</span></span>|<span data-ttu-id="a0d60-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a0d60-165">DateTime the object was created.</span></span> <span data-ttu-id="a0d60-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-167">description</span><span class="sxs-lookup"><span data-stu-id="a0d60-167">description</span></span>|<span data-ttu-id="a0d60-168">String</span><span class="sxs-lookup"><span data-stu-id="a0d60-168">String</span></span>|<span data-ttu-id="a0d60-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a0d60-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0d60-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a0d60-171">displayName</span></span>|<span data-ttu-id="a0d60-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a0d60-172">String</span></span>|<span data-ttu-id="a0d60-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a0d60-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0d60-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-175">version</span><span class="sxs-lookup"><span data-stu-id="a0d60-175">version</span></span>|<span data-ttu-id="a0d60-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d60-176">Int32</span></span>|<span data-ttu-id="a0d60-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a0d60-177">Version of the device configuration.</span></span> <span data-ttu-id="a0d60-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d60-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d60-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a0d60-179">isEnabled</span></span>|<span data-ttu-id="a0d60-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0d60-180">Boolean</span></span>|<span data-ttu-id="a0d60-181">Включен параметр в пользовательском интерфейсе</span><span class="sxs-lookup"><span data-stu-id="a0d60-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="a0d60-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a0d60-182">activeHoursStart</span></span>|<span data-ttu-id="a0d60-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0d60-183">TimeOfDay</span></span>|<span data-ttu-id="a0d60-184">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="a0d60-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a0d60-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a0d60-185">activeHoursEnd</span></span>|<span data-ttu-id="a0d60-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0d60-186">TimeOfDay</span></span>|<span data-ttu-id="a0d60-187">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="a0d60-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a0d60-188">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="a0d60-188">scheduledInstallDays</span></span>|<span data-ttu-id="a0d60-189">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="a0d60-189">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="a0d60-190">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="a0d60-190">Days in week for which active hours are configured.</span></span> <span data-ttu-id="a0d60-191">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="a0d60-191">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="a0d60-192">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="a0d60-192">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a0d60-193">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="a0d60-193">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="a0d60-194">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d60-194">Int32</span></span>|<span data-ttu-id="a0d60-195">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a0d60-195">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="a0d60-196">енфорцедсофтвареупдатеделайиндайс</span><span class="sxs-lookup"><span data-stu-id="a0d60-196">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="a0d60-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d60-197">Int32</span></span>|<span data-ttu-id="a0d60-198">Дней до отображения обновлений программного обеспечения для устройств с iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="a0d60-198">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="a0d60-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d60-199">Response</span></span>
<span data-ttu-id="a0d60-200">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a0d60-200">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d60-201">Пример</span><span class="sxs-lookup"><span data-stu-id="a0d60-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0d60-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0d60-202">Request</span></span>
<span data-ttu-id="a0d60-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0d60-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0d60-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d60-204">Response</span></span>
<span data-ttu-id="a0d60-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0d60-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






