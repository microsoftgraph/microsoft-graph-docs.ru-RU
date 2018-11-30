---
title: Обновление unsupportedDeviceConfiguration
description: Обновление свойства объекта unsupportedDeviceConfiguration.
ms.openlocfilehash: 0f8594642908aef125556f06fdca911c9530db76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076550"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="ee46b-103">Обновление unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee46b-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="ee46b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee46b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee46b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee46b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee46b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee46b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee46b-107">Обновление свойства объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee46b-107">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee46b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee46b-108">Prerequisites</span></span>
<span data-ttu-id="ee46b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee46b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee46b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee46b-111">Permission type</span></span>|<span data-ttu-id="ee46b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee46b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee46b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee46b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee46b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee46b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee46b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee46b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee46b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee46b-116">Not supported.</span></span>|
|<span data-ttu-id="ee46b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee46b-117">Application</span></span>|<span data-ttu-id="ee46b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee46b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee46b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee46b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee46b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee46b-120">Request headers</span></span>
|<span data-ttu-id="ee46b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee46b-121">Header</span></span>|<span data-ttu-id="ee46b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee46b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee46b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee46b-123">Authorization</span></span>|<span data-ttu-id="ee46b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ee46b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee46b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee46b-125">Accept</span></span>|<span data-ttu-id="ee46b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee46b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee46b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee46b-127">Request body</span></span>
<span data-ttu-id="ee46b-128">В тексте запроса укажите представление JSON для объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee46b-128">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ee46b-129">В следующей таблице показаны свойства, которые необходимы для создания [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-129">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="ee46b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee46b-130">Property</span></span>|<span data-ttu-id="ee46b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee46b-131">Type</span></span>|<span data-ttu-id="ee46b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee46b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee46b-133">id</span><span class="sxs-lookup"><span data-stu-id="ee46b-133">id</span></span>|<span data-ttu-id="ee46b-134">String</span><span class="sxs-lookup"><span data-stu-id="ee46b-134">String</span></span>|<span data-ttu-id="ee46b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee46b-135">Key of the entity.</span></span> <span data-ttu-id="ee46b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee46b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ee46b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee46b-138">DateTimeOffset</span></span>|<span data-ttu-id="ee46b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee46b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ee46b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee46b-141">roleScopeTagIds</span></span>|<span data-ttu-id="ee46b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee46b-142">String collection</span></span>|<span data-ttu-id="ee46b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ee46b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee46b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ee46b-145">supportsScopeTags</span></span>|<span data-ttu-id="ee46b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ee46b-146">Boolean</span></span>|<span data-ttu-id="ee46b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ee46b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee46b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ee46b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee46b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ee46b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee46b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee46b-150">This property is read-only.</span></span> <span data-ttu-id="ee46b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee46b-152">createdDateTime</span></span>|<span data-ttu-id="ee46b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee46b-153">DateTimeOffset</span></span>|<span data-ttu-id="ee46b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ee46b-154">DateTime the object was created.</span></span> <span data-ttu-id="ee46b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-156">описание</span><span class="sxs-lookup"><span data-stu-id="ee46b-156">description</span></span>|<span data-ttu-id="ee46b-157">String</span><span class="sxs-lookup"><span data-stu-id="ee46b-157">String</span></span>|<span data-ttu-id="ee46b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee46b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee46b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ee46b-160">displayName</span></span>|<span data-ttu-id="ee46b-161">String</span><span class="sxs-lookup"><span data-stu-id="ee46b-161">String</span></span>|<span data-ttu-id="ee46b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee46b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee46b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-164">version</span><span class="sxs-lookup"><span data-stu-id="ee46b-164">version</span></span>|<span data-ttu-id="ee46b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ee46b-165">Int32</span></span>|<span data-ttu-id="ee46b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee46b-166">Version of the device configuration.</span></span> <span data-ttu-id="ee46b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee46b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee46b-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="ee46b-168">originalEntityTypeName</span></span>|<span data-ttu-id="ee46b-169">String</span><span class="sxs-lookup"><span data-stu-id="ee46b-169">String</span></span>|<span data-ttu-id="ee46b-170">Тип сущности, которая в противном случае будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="ee46b-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="ee46b-171">details</span><span class="sxs-lookup"><span data-stu-id="ee46b-171">details</span></span>|<span data-ttu-id="ee46b-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ee46b-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="ee46b-173">Сведения о почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee46b-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="ee46b-174">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee46b-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ee46b-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee46b-175">Response</span></span>
<span data-ttu-id="ee46b-176">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee46b-176">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee46b-177">Пример</span><span class="sxs-lookup"><span data-stu-id="ee46b-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee46b-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee46b-178">Request</span></span>
<span data-ttu-id="ee46b-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee46b-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 513

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="ee46b-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee46b-180">Response</span></span>
<span data-ttu-id="ee46b-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ee46b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





