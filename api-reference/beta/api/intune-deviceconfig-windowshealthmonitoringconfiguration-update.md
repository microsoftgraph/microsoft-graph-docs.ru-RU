---
title: Обновление Виндовшеалсмониторингконфигуратион
description: Обновление свойств объекта Виндовшеалсмониторингконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e22db8c85d591c770128dc3db3594fa23826836
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917921"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="1e0d6-103">Обновление Виндовшеалсмониторингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1e0d6-103">Update windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="1e0d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e0d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e0d6-106">Обновление свойств объекта [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1e0d6-106">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e0d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1e0d6-107">Prerequisites</span></span>
<span data-ttu-id="1e0d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e0d6-110">Permission type</span></span>|<span data-ttu-id="1e0d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e0d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e0d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e0d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e0d6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e0d6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e0d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e0d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e0d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-115">Not supported.</span></span>|
|<span data-ttu-id="1e0d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e0d6-116">Application</span></span>|<span data-ttu-id="1e0d6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e0d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e0d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1e0d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e0d6-119">Request headers</span></span>
|<span data-ttu-id="1e0d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e0d6-120">Header</span></span>|<span data-ttu-id="1e0d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1e0d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e0d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e0d6-122">Authorization</span></span>|<span data-ttu-id="1e0d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e0d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1e0d6-124">Accept</span></span>|<span data-ttu-id="1e0d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e0d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0d6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1e0d6-126">Request body</span></span>
<span data-ttu-id="1e0d6-127">В тексте запроса добавьте представление объекта [Виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-127">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="1e0d6-128">В следующей таблице приведены свойства, необходимые при создании [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-128">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="1e0d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e0d6-129">Property</span></span>|<span data-ttu-id="1e0d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1e0d6-130">Type</span></span>|<span data-ttu-id="1e0d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0d6-132">id</span><span class="sxs-lookup"><span data-stu-id="1e0d6-132">id</span></span>|<span data-ttu-id="1e0d6-133">String</span><span class="sxs-lookup"><span data-stu-id="1e0d6-133">String</span></span>|<span data-ttu-id="1e0d6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-134">Key of the entity.</span></span> <span data-ttu-id="1e0d6-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e0d6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1e0d6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e0d6-137">DateTimeOffset</span></span>|<span data-ttu-id="1e0d6-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1e0d6-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e0d6-140">roleScopeTagIds</span></span>|<span data-ttu-id="1e0d6-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1e0d6-141">String collection</span></span>|<span data-ttu-id="1e0d6-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1e0d6-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1e0d6-144">supportsScopeTags</span></span>|<span data-ttu-id="1e0d6-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1e0d6-145">Boolean</span></span>|<span data-ttu-id="1e0d6-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1e0d6-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1e0d6-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1e0d6-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-149">This property is read-only.</span></span> <span data-ttu-id="1e0d6-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e0d6-151">createdDateTime</span></span>|<span data-ttu-id="1e0d6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e0d6-152">DateTimeOffset</span></span>|<span data-ttu-id="1e0d6-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-153">DateTime the object was created.</span></span> <span data-ttu-id="1e0d6-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-155">description</span><span class="sxs-lookup"><span data-stu-id="1e0d6-155">description</span></span>|<span data-ttu-id="1e0d6-156">String</span><span class="sxs-lookup"><span data-stu-id="1e0d6-156">String</span></span>|<span data-ttu-id="1e0d6-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e0d6-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1e0d6-159">displayName</span></span>|<span data-ttu-id="1e0d6-160">Строка</span><span class="sxs-lookup"><span data-stu-id="1e0d6-160">String</span></span>|<span data-ttu-id="1e0d6-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e0d6-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-163">version</span><span class="sxs-lookup"><span data-stu-id="1e0d6-163">version</span></span>|<span data-ttu-id="1e0d6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0d6-164">Int32</span></span>|<span data-ttu-id="1e0d6-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-165">Version of the device configuration.</span></span> <span data-ttu-id="1e0d6-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0d6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e0d6-167">Алловдевицехеалсмониторинг</span><span class="sxs-lookup"><span data-stu-id="1e0d6-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="1e0d6-168">Включение</span><span class="sxs-lookup"><span data-stu-id="1e0d6-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1e0d6-169">Включает мониторинг работоспособности устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="1e0d6-170">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1e0d6-171">Конфигдевицехеалсмониторингскопе</span><span class="sxs-lookup"><span data-stu-id="1e0d6-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="1e0d6-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="1e0d6-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="1e0d6-173">Задает набор событий, полученных с устройства, на котором включен мониторинг работоспособности.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-173">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="1e0d6-174">Возможные значения: `undefined`, `healthMonitoring`, `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="1e0d6-175">Конфигдевицехеалсмониторингкустомскопе</span><span class="sxs-lookup"><span data-stu-id="1e0d6-175">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="1e0d6-176">Строка</span><span class="sxs-lookup"><span data-stu-id="1e0d6-176">String</span></span>|<span data-ttu-id="1e0d6-177">Указывает настраиваемый набор событий, собранных с устройства, на котором включен мониторинг работоспособности</span><span class="sxs-lookup"><span data-stu-id="1e0d6-177">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="1e0d6-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e0d6-178">Response</span></span>
<span data-ttu-id="1e0d6-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-179">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e0d6-180">Пример</span><span class="sxs-lookup"><span data-stu-id="1e0d6-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e0d6-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e0d6-181">Request</span></span>
<span data-ttu-id="1e0d6-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 471

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```

### <a name="response"></a><span data-ttu-id="1e0d6-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e0d6-183">Response</span></span>
<span data-ttu-id="1e0d6-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e0d6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 643

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```




