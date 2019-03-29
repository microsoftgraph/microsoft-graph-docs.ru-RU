---
title: Создание Виндовшеалсмониторингконфигуратион
description: Создание нового объекта Виндовшеалсмониторингконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75ace30116ddf2515f99f8bcdd6a2c9c19f45b58
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972930"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="db3cb-103">Создание Виндовшеалсмониторингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="db3cb-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="db3cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db3cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db3cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db3cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db3cb-106">Создание нового объекта [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db3cb-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db3cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db3cb-107">Prerequisites</span></span>
<span data-ttu-id="db3cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db3cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db3cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db3cb-110">Permission type</span></span>|<span data-ttu-id="db3cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db3cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db3cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db3cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db3cb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3cb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db3cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db3cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db3cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db3cb-115">Not supported.</span></span>|
|<span data-ttu-id="db3cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db3cb-116">Application</span></span>|<span data-ttu-id="db3cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db3cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db3cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db3cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db3cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db3cb-119">Request headers</span></span>
|<span data-ttu-id="db3cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db3cb-120">Header</span></span>|<span data-ttu-id="db3cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="db3cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db3cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db3cb-122">Authorization</span></span>|<span data-ttu-id="db3cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db3cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db3cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="db3cb-124">Accept</span></span>|<span data-ttu-id="db3cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db3cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db3cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db3cb-126">Request body</span></span>
<span data-ttu-id="db3cb-127">В тексте запроса добавьте представление объекта Виндовшеалсмониторингконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db3cb-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="db3cb-128">В следующей таблице приведены свойства, необходимые при создании Виндовшеалсмониторингконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="db3cb-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="db3cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="db3cb-129">Property</span></span>|<span data-ttu-id="db3cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="db3cb-130">Type</span></span>|<span data-ttu-id="db3cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="db3cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db3cb-132">id</span><span class="sxs-lookup"><span data-stu-id="db3cb-132">id</span></span>|<span data-ttu-id="db3cb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="db3cb-133">String</span></span>|<span data-ttu-id="db3cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="db3cb-134">Key of the entity.</span></span> <span data-ttu-id="db3cb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db3cb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="db3cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3cb-137">DateTimeOffset</span></span>|<span data-ttu-id="db3cb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="db3cb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="db3cb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db3cb-140">roleScopeTagIds</span></span>|<span data-ttu-id="db3cb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db3cb-141">String collection</span></span>|<span data-ttu-id="db3cb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="db3cb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db3cb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="db3cb-144">supportsScopeTags</span></span>|<span data-ttu-id="db3cb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="db3cb-145">Boolean</span></span>|<span data-ttu-id="db3cb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="db3cb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db3cb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="db3cb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db3cb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="db3cb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db3cb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3cb-149">This property is read-only.</span></span> <span data-ttu-id="db3cb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db3cb-151">createdDateTime</span></span>|<span data-ttu-id="db3cb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3cb-152">DateTimeOffset</span></span>|<span data-ttu-id="db3cb-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="db3cb-153">DateTime the object was created.</span></span> <span data-ttu-id="db3cb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-155">description</span><span class="sxs-lookup"><span data-stu-id="db3cb-155">description</span></span>|<span data-ttu-id="db3cb-156">String</span><span class="sxs-lookup"><span data-stu-id="db3cb-156">String</span></span>|<span data-ttu-id="db3cb-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="db3cb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db3cb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="db3cb-159">displayName</span></span>|<span data-ttu-id="db3cb-160">String</span><span class="sxs-lookup"><span data-stu-id="db3cb-160">String</span></span>|<span data-ttu-id="db3cb-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="db3cb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db3cb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-163">version</span><span class="sxs-lookup"><span data-stu-id="db3cb-163">version</span></span>|<span data-ttu-id="db3cb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="db3cb-164">Int32</span></span>|<span data-ttu-id="db3cb-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="db3cb-165">Version of the device configuration.</span></span> <span data-ttu-id="db3cb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db3cb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db3cb-167">Алловдевицехеалсмониторинг</span><span class="sxs-lookup"><span data-stu-id="db3cb-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="db3cb-168">Включение</span><span class="sxs-lookup"><span data-stu-id="db3cb-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="db3cb-169">Включает мониторинг работоспособности устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="db3cb-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="db3cb-170">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="db3cb-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="db3cb-171">Конфигдевицехеалсмониторингскопе</span><span class="sxs-lookup"><span data-stu-id="db3cb-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="db3cb-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="db3cb-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="db3cb-173">СепЦифиес набор событий, полученных с устройства, на котором включен мониторинг работоспособности.</span><span class="sxs-lookup"><span data-stu-id="db3cb-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="db3cb-174">Возможные значения: `undefined`, `healthMonitoring`, `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="db3cb-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="db3cb-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="db3cb-175">Response</span></span>
<span data-ttu-id="db3cb-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db3cb-176">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db3cb-177">Пример</span><span class="sxs-lookup"><span data-stu-id="db3cb-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="db3cb-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="db3cb-178">Request</span></span>
<span data-ttu-id="db3cb-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db3cb-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 371

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
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```

### <a name="response"></a><span data-ttu-id="db3cb-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="db3cb-180">Response</span></span>
<span data-ttu-id="db3cb-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db3cb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 543

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
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```




