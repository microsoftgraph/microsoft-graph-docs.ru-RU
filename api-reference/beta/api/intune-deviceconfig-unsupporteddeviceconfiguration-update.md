---
title: Обновление unsupportedDeviceConfiguration
description: Обновление свойства объекта unsupportedDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf4dc0e52b577682ea88a93abaabb561dbb444b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395022"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="847dd-103">Обновление unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="847dd-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="847dd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="847dd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="847dd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="847dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="847dd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="847dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="847dd-107">Обновление свойства объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="847dd-107">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="847dd-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="847dd-108">Prerequisites</span></span>
<span data-ttu-id="847dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="847dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="847dd-111">Permission type</span></span>|<span data-ttu-id="847dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="847dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="847dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="847dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="847dd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="847dd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="847dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="847dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="847dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="847dd-116">Not supported.</span></span>|
|<span data-ttu-id="847dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="847dd-117">Application</span></span>|<span data-ttu-id="847dd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="847dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="847dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="847dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="847dd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="847dd-120">Request headers</span></span>
|<span data-ttu-id="847dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="847dd-121">Header</span></span>|<span data-ttu-id="847dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="847dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="847dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="847dd-123">Authorization</span></span>|<span data-ttu-id="847dd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="847dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="847dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="847dd-125">Accept</span></span>|<span data-ttu-id="847dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="847dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="847dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="847dd-127">Request body</span></span>
<span data-ttu-id="847dd-128">В тексте запроса укажите представление JSON для объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="847dd-128">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="847dd-129">В следующей таблице показаны свойства, которые необходимы для создания [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-129">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="847dd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="847dd-130">Property</span></span>|<span data-ttu-id="847dd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="847dd-131">Type</span></span>|<span data-ttu-id="847dd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="847dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="847dd-133">id</span><span class="sxs-lookup"><span data-stu-id="847dd-133">id</span></span>|<span data-ttu-id="847dd-134">String</span><span class="sxs-lookup"><span data-stu-id="847dd-134">String</span></span>|<span data-ttu-id="847dd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="847dd-135">Key of the entity.</span></span> <span data-ttu-id="847dd-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="847dd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="847dd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="847dd-138">DateTimeOffset</span></span>|<span data-ttu-id="847dd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="847dd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="847dd-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="847dd-141">roleScopeTagIds</span></span>|<span data-ttu-id="847dd-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="847dd-142">String collection</span></span>|<span data-ttu-id="847dd-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="847dd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="847dd-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="847dd-145">supportsScopeTags</span></span>|<span data-ttu-id="847dd-146">Логический</span><span class="sxs-lookup"><span data-stu-id="847dd-146">Boolean</span></span>|<span data-ttu-id="847dd-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="847dd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="847dd-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="847dd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="847dd-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="847dd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="847dd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="847dd-150">This property is read-only.</span></span> <span data-ttu-id="847dd-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="847dd-152">createdDateTime</span></span>|<span data-ttu-id="847dd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="847dd-153">DateTimeOffset</span></span>|<span data-ttu-id="847dd-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="847dd-154">DateTime the object was created.</span></span> <span data-ttu-id="847dd-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-156">description</span><span class="sxs-lookup"><span data-stu-id="847dd-156">description</span></span>|<span data-ttu-id="847dd-157">String</span><span class="sxs-lookup"><span data-stu-id="847dd-157">String</span></span>|<span data-ttu-id="847dd-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="847dd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="847dd-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="847dd-160">displayName</span></span>|<span data-ttu-id="847dd-161">String</span><span class="sxs-lookup"><span data-stu-id="847dd-161">String</span></span>|<span data-ttu-id="847dd-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="847dd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="847dd-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-164">version</span><span class="sxs-lookup"><span data-stu-id="847dd-164">version</span></span>|<span data-ttu-id="847dd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="847dd-165">Int32</span></span>|<span data-ttu-id="847dd-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="847dd-166">Version of the device configuration.</span></span> <span data-ttu-id="847dd-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="847dd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="847dd-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="847dd-168">originalEntityTypeName</span></span>|<span data-ttu-id="847dd-169">String</span><span class="sxs-lookup"><span data-stu-id="847dd-169">String</span></span>|<span data-ttu-id="847dd-170">Тип сущности, которая в противном случае будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="847dd-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="847dd-171">details</span><span class="sxs-lookup"><span data-stu-id="847dd-171">details</span></span>|<span data-ttu-id="847dd-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="847dd-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="847dd-173">Сведения о почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="847dd-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="847dd-174">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="847dd-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="847dd-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="847dd-175">Response</span></span>
<span data-ttu-id="847dd-176">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="847dd-176">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="847dd-177">Пример</span><span class="sxs-lookup"><span data-stu-id="847dd-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="847dd-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="847dd-178">Request</span></span>
<span data-ttu-id="847dd-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="847dd-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="847dd-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="847dd-180">Response</span></span>
<span data-ttu-id="847dd-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="847dd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




