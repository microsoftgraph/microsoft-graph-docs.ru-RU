---
title: Обновление Унсуппортеддевицеконфигуратион
description: Обновление свойств объекта Унсуппортеддевицеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72f1320d48c22890fc2b5ee9ff2566132885aa68
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168350"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="39733-103">Обновление Унсуппортеддевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="39733-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="39733-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39733-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39733-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39733-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39733-106">Обновление свойств объекта [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="39733-106">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39733-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39733-107">Prerequisites</span></span>
<span data-ttu-id="39733-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="39733-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39733-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39733-110">Permission type</span></span>|<span data-ttu-id="39733-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39733-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39733-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39733-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39733-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39733-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39733-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39733-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39733-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39733-115">Not supported.</span></span>|
|<span data-ttu-id="39733-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39733-116">Application</span></span>|<span data-ttu-id="39733-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39733-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39733-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39733-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="39733-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39733-119">Request headers</span></span>
|<span data-ttu-id="39733-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39733-120">Header</span></span>|<span data-ttu-id="39733-121">Значение</span><span class="sxs-lookup"><span data-stu-id="39733-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39733-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39733-122">Authorization</span></span>|<span data-ttu-id="39733-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="39733-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39733-124">Accept</span><span class="sxs-lookup"><span data-stu-id="39733-124">Accept</span></span>|<span data-ttu-id="39733-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39733-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39733-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39733-126">Request body</span></span>
<span data-ttu-id="39733-127">В тексте запроса добавьте представление объекта [Унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39733-127">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="39733-128">В следующей таблице приведены свойства, необходимые при создании [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-128">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="39733-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="39733-129">Property</span></span>|<span data-ttu-id="39733-130">Тип</span><span class="sxs-lookup"><span data-stu-id="39733-130">Type</span></span>|<span data-ttu-id="39733-131">Описание</span><span class="sxs-lookup"><span data-stu-id="39733-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39733-132">id</span><span class="sxs-lookup"><span data-stu-id="39733-132">id</span></span>|<span data-ttu-id="39733-133">String</span><span class="sxs-lookup"><span data-stu-id="39733-133">String</span></span>|<span data-ttu-id="39733-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39733-134">Key of the entity.</span></span> <span data-ttu-id="39733-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39733-136">lastModifiedDateTime</span></span>|<span data-ttu-id="39733-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39733-137">DateTimeOffset</span></span>|<span data-ttu-id="39733-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="39733-138">DateTime the object was last modified.</span></span> <span data-ttu-id="39733-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39733-140">roleScopeTagIds</span></span>|<span data-ttu-id="39733-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="39733-141">String collection</span></span>|<span data-ttu-id="39733-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="39733-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39733-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="39733-144">supportsScopeTags</span></span>|<span data-ttu-id="39733-145">Логический</span><span class="sxs-lookup"><span data-stu-id="39733-145">Boolean</span></span>|<span data-ttu-id="39733-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="39733-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39733-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="39733-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39733-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="39733-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39733-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39733-149">This property is read-only.</span></span> <span data-ttu-id="39733-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39733-151">createdDateTime</span></span>|<span data-ttu-id="39733-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39733-152">DateTimeOffset</span></span>|<span data-ttu-id="39733-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="39733-153">DateTime the object was created.</span></span> <span data-ttu-id="39733-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-155">description</span><span class="sxs-lookup"><span data-stu-id="39733-155">description</span></span>|<span data-ttu-id="39733-156">String</span><span class="sxs-lookup"><span data-stu-id="39733-156">String</span></span>|<span data-ttu-id="39733-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39733-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39733-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-159">displayName</span><span class="sxs-lookup"><span data-stu-id="39733-159">displayName</span></span>|<span data-ttu-id="39733-160">String</span><span class="sxs-lookup"><span data-stu-id="39733-160">String</span></span>|<span data-ttu-id="39733-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39733-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39733-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-163">version</span><span class="sxs-lookup"><span data-stu-id="39733-163">version</span></span>|<span data-ttu-id="39733-164">Int32</span><span class="sxs-lookup"><span data-stu-id="39733-164">Int32</span></span>|<span data-ttu-id="39733-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39733-165">Version of the device configuration.</span></span> <span data-ttu-id="39733-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39733-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39733-167">Оригиналентититипенаме</span><span class="sxs-lookup"><span data-stu-id="39733-167">originalEntityTypeName</span></span>|<span data-ttu-id="39733-168">String</span><span class="sxs-lookup"><span data-stu-id="39733-168">String</span></span>|<span data-ttu-id="39733-169">Тип сущности, возвращаемой в противном случае.</span><span class="sxs-lookup"><span data-stu-id="39733-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="39733-170">подробности</span><span class="sxs-lookup"><span data-stu-id="39733-170">details</span></span>|<span data-ttu-id="39733-171">Коллекция [унсуппортеддевицеконфигуратиондетаил](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="39733-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="39733-172">Сведения о том, почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39733-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="39733-173">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="39733-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="39733-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="39733-174">Response</span></span>
<span data-ttu-id="39733-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39733-175">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39733-176">Пример</span><span class="sxs-lookup"><span data-stu-id="39733-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="39733-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="39733-177">Request</span></span>
<span data-ttu-id="39733-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39733-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39733-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="39733-179">Response</span></span>
<span data-ttu-id="39733-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39733-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




