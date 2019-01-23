---
title: Создание unsupportedDeviceConfiguration
description: Создание нового объекта unsupportedDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 098cd2b0cb5f318dba41a1268ebb8e56b752defc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408903"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="3408d-103">Создание unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3408d-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="3408d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3408d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3408d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3408d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3408d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3408d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3408d-107">Создание нового объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3408d-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3408d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3408d-108">Prerequisites</span></span>
<span data-ttu-id="3408d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3408d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3408d-111">Permission type</span></span>|<span data-ttu-id="3408d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3408d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3408d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3408d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3408d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3408d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3408d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3408d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3408d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3408d-116">Not supported.</span></span>|
|<span data-ttu-id="3408d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3408d-117">Application</span></span>|<span data-ttu-id="3408d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3408d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3408d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3408d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3408d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3408d-120">Request headers</span></span>
|<span data-ttu-id="3408d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3408d-121">Header</span></span>|<span data-ttu-id="3408d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3408d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3408d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3408d-123">Authorization</span></span>|<span data-ttu-id="3408d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3408d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3408d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3408d-125">Accept</span></span>|<span data-ttu-id="3408d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3408d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3408d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3408d-127">Request body</span></span>
<span data-ttu-id="3408d-128">В тексте запроса укажите представление JSON для объекта unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3408d-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="3408d-129">В следующей таблице показаны свойства, которые необходимы для создания unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3408d-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="3408d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3408d-130">Property</span></span>|<span data-ttu-id="3408d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3408d-131">Type</span></span>|<span data-ttu-id="3408d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3408d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3408d-133">id</span><span class="sxs-lookup"><span data-stu-id="3408d-133">id</span></span>|<span data-ttu-id="3408d-134">String</span><span class="sxs-lookup"><span data-stu-id="3408d-134">String</span></span>|<span data-ttu-id="3408d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3408d-135">Key of the entity.</span></span> <span data-ttu-id="3408d-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3408d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3408d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3408d-138">DateTimeOffset</span></span>|<span data-ttu-id="3408d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3408d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3408d-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3408d-141">roleScopeTagIds</span></span>|<span data-ttu-id="3408d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3408d-142">String collection</span></span>|<span data-ttu-id="3408d-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3408d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3408d-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3408d-145">supportsScopeTags</span></span>|<span data-ttu-id="3408d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="3408d-146">Boolean</span></span>|<span data-ttu-id="3408d-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="3408d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3408d-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="3408d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3408d-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3408d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3408d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3408d-150">This property is read-only.</span></span> <span data-ttu-id="3408d-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3408d-152">createdDateTime</span></span>|<span data-ttu-id="3408d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3408d-153">DateTimeOffset</span></span>|<span data-ttu-id="3408d-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3408d-154">DateTime the object was created.</span></span> <span data-ttu-id="3408d-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-156">description</span><span class="sxs-lookup"><span data-stu-id="3408d-156">description</span></span>|<span data-ttu-id="3408d-157">String</span><span class="sxs-lookup"><span data-stu-id="3408d-157">String</span></span>|<span data-ttu-id="3408d-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3408d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3408d-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3408d-160">displayName</span></span>|<span data-ttu-id="3408d-161">String</span><span class="sxs-lookup"><span data-stu-id="3408d-161">String</span></span>|<span data-ttu-id="3408d-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3408d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3408d-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-164">version</span><span class="sxs-lookup"><span data-stu-id="3408d-164">version</span></span>|<span data-ttu-id="3408d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3408d-165">Int32</span></span>|<span data-ttu-id="3408d-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3408d-166">Version of the device configuration.</span></span> <span data-ttu-id="3408d-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3408d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3408d-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="3408d-168">originalEntityTypeName</span></span>|<span data-ttu-id="3408d-169">String</span><span class="sxs-lookup"><span data-stu-id="3408d-169">String</span></span>|<span data-ttu-id="3408d-170">Тип сущности, которая в противном случае будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="3408d-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="3408d-171">details</span><span class="sxs-lookup"><span data-stu-id="3408d-171">details</span></span>|<span data-ttu-id="3408d-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3408d-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="3408d-173">Сведения о почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3408d-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="3408d-174">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="3408d-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3408d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="3408d-175">Response</span></span>
<span data-ttu-id="3408d-176">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3408d-176">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3408d-177">Пример</span><span class="sxs-lookup"><span data-stu-id="3408d-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="3408d-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="3408d-178">Request</span></span>
<span data-ttu-id="3408d-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3408d-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3408d-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="3408d-180">Response</span></span>
<span data-ttu-id="3408d-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3408d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




