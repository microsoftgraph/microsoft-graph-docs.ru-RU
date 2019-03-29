---
title: Обновление Унсуппортеддевицеконфигуратион
description: Обновление свойств объекта Унсуппортеддевицеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb329eb11058ae8d1239360f07badd850060ec1f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958426"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="4dad9-103">Обновление Унсуппортеддевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4dad9-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="4dad9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dad9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dad9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dad9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dad9-106">Обновление свойств объекта [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4dad9-106">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dad9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4dad9-107">Prerequisites</span></span>
<span data-ttu-id="4dad9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dad9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dad9-110">Permission type</span></span>|<span data-ttu-id="4dad9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dad9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dad9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dad9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dad9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dad9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dad9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dad9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dad9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dad9-115">Not supported.</span></span>|
|<span data-ttu-id="4dad9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dad9-116">Application</span></span>|<span data-ttu-id="4dad9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dad9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dad9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dad9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4dad9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dad9-119">Request headers</span></span>
|<span data-ttu-id="4dad9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dad9-120">Header</span></span>|<span data-ttu-id="4dad9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4dad9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dad9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dad9-122">Authorization</span></span>|<span data-ttu-id="4dad9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dad9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dad9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4dad9-124">Accept</span></span>|<span data-ttu-id="4dad9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dad9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dad9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dad9-126">Request body</span></span>
<span data-ttu-id="4dad9-127">В тексте запроса добавьте представление объекта [Унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dad9-127">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="4dad9-128">В следующей таблице приведены свойства, необходимые при создании [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-128">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="4dad9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dad9-129">Property</span></span>|<span data-ttu-id="4dad9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4dad9-130">Type</span></span>|<span data-ttu-id="4dad9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4dad9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dad9-132">id</span><span class="sxs-lookup"><span data-stu-id="4dad9-132">id</span></span>|<span data-ttu-id="4dad9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4dad9-133">String</span></span>|<span data-ttu-id="4dad9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4dad9-134">Key of the entity.</span></span> <span data-ttu-id="4dad9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dad9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4dad9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dad9-137">DateTimeOffset</span></span>|<span data-ttu-id="4dad9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4dad9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4dad9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4dad9-140">roleScopeTagIds</span></span>|<span data-ttu-id="4dad9-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4dad9-141">String collection</span></span>|<span data-ttu-id="4dad9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4dad9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4dad9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4dad9-144">supportsScopeTags</span></span>|<span data-ttu-id="4dad9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dad9-145">Boolean</span></span>|<span data-ttu-id="4dad9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4dad9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4dad9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4dad9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4dad9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4dad9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4dad9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dad9-149">This property is read-only.</span></span> <span data-ttu-id="4dad9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4dad9-151">createdDateTime</span></span>|<span data-ttu-id="4dad9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dad9-152">DateTimeOffset</span></span>|<span data-ttu-id="4dad9-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4dad9-153">DateTime the object was created.</span></span> <span data-ttu-id="4dad9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-155">description</span><span class="sxs-lookup"><span data-stu-id="4dad9-155">description</span></span>|<span data-ttu-id="4dad9-156">String</span><span class="sxs-lookup"><span data-stu-id="4dad9-156">String</span></span>|<span data-ttu-id="4dad9-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4dad9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4dad9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4dad9-159">displayName</span></span>|<span data-ttu-id="4dad9-160">String</span><span class="sxs-lookup"><span data-stu-id="4dad9-160">String</span></span>|<span data-ttu-id="4dad9-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4dad9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4dad9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-163">version</span><span class="sxs-lookup"><span data-stu-id="4dad9-163">version</span></span>|<span data-ttu-id="4dad9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4dad9-164">Int32</span></span>|<span data-ttu-id="4dad9-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4dad9-165">Version of the device configuration.</span></span> <span data-ttu-id="4dad9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dad9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dad9-167">Оригиналентититипенаме</span><span class="sxs-lookup"><span data-stu-id="4dad9-167">originalEntityTypeName</span></span>|<span data-ttu-id="4dad9-168">String</span><span class="sxs-lookup"><span data-stu-id="4dad9-168">String</span></span>|<span data-ttu-id="4dad9-169">Тип сущности, возвращаемой в противном случае.</span><span class="sxs-lookup"><span data-stu-id="4dad9-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="4dad9-170">подробности</span><span class="sxs-lookup"><span data-stu-id="4dad9-170">details</span></span>|<span data-ttu-id="4dad9-171">Коллекция [унсуппортеддевицеконфигуратиондетаил](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="4dad9-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="4dad9-172">Сведения о том, почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dad9-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="4dad9-173">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="4dad9-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4dad9-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dad9-174">Response</span></span>
<span data-ttu-id="4dad9-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4dad9-175">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dad9-176">Пример</span><span class="sxs-lookup"><span data-stu-id="4dad9-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dad9-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dad9-177">Request</span></span>
<span data-ttu-id="4dad9-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dad9-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4dad9-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dad9-179">Response</span></span>
<span data-ttu-id="4dad9-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4dad9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```




