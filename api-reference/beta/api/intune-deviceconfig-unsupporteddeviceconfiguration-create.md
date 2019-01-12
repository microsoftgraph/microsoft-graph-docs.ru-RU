---
title: Создание unsupportedDeviceConfiguration
description: Создание нового объекта unsupportedDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 86babcc56ebf62a7456bce90e0cfd7c7f9748d5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964762"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="5a6e2-103">Создание unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a6e2-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="5a6e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a6e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a6e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a6e2-107">Создание нового объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5a6e2-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a6e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a6e2-108">Prerequisites</span></span>
<span data-ttu-id="5a6e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a6e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6e2-111">Permission type</span></span>|<span data-ttu-id="5a6e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a6e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a6e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a6e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a6e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a6e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a6e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a6e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a6e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-116">Not supported.</span></span>|
|<span data-ttu-id="5a6e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a6e2-117">Application</span></span>|<span data-ttu-id="5a6e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a6e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a6e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a6e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a6e2-120">Request headers</span></span>
|<span data-ttu-id="5a6e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a6e2-121">Header</span></span>|<span data-ttu-id="5a6e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5a6e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a6e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a6e2-123">Authorization</span></span>|<span data-ttu-id="5a6e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5a6e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a6e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5a6e2-125">Accept</span></span>|<span data-ttu-id="5a6e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a6e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a6e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a6e2-127">Request body</span></span>
<span data-ttu-id="5a6e2-128">В тексте запроса укажите представление JSON для объекта unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="5a6e2-129">В следующей таблице показаны свойства, которые необходимы для создания unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="5a6e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a6e2-130">Property</span></span>|<span data-ttu-id="5a6e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5a6e2-131">Type</span></span>|<span data-ttu-id="5a6e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a6e2-133">id</span><span class="sxs-lookup"><span data-stu-id="5a6e2-133">id</span></span>|<span data-ttu-id="5a6e2-134">String</span><span class="sxs-lookup"><span data-stu-id="5a6e2-134">String</span></span>|<span data-ttu-id="5a6e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-135">Key of the entity.</span></span> <span data-ttu-id="5a6e2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a6e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5a6e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a6e2-138">DateTimeOffset</span></span>|<span data-ttu-id="5a6e2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5a6e2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a6e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="5a6e2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5a6e2-142">String collection</span></span>|<span data-ttu-id="5a6e2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5a6e2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5a6e2-145">supportsScopeTags</span></span>|<span data-ttu-id="5a6e2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a6e2-146">Boolean</span></span>|<span data-ttu-id="5a6e2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5a6e2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5a6e2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5a6e2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-150">This property is read-only.</span></span> <span data-ttu-id="5a6e2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a6e2-152">createdDateTime</span></span>|<span data-ttu-id="5a6e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a6e2-153">DateTimeOffset</span></span>|<span data-ttu-id="5a6e2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-154">DateTime the object was created.</span></span> <span data-ttu-id="5a6e2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-156">описание</span><span class="sxs-lookup"><span data-stu-id="5a6e2-156">description</span></span>|<span data-ttu-id="5a6e2-157">String</span><span class="sxs-lookup"><span data-stu-id="5a6e2-157">String</span></span>|<span data-ttu-id="5a6e2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5a6e2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5a6e2-160">displayName</span></span>|<span data-ttu-id="5a6e2-161">String</span><span class="sxs-lookup"><span data-stu-id="5a6e2-161">String</span></span>|<span data-ttu-id="5a6e2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5a6e2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-164">version</span><span class="sxs-lookup"><span data-stu-id="5a6e2-164">version</span></span>|<span data-ttu-id="5a6e2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5a6e2-165">Int32</span></span>|<span data-ttu-id="5a6e2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-166">Version of the device configuration.</span></span> <span data-ttu-id="5a6e2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a6e2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a6e2-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="5a6e2-168">originalEntityTypeName</span></span>|<span data-ttu-id="5a6e2-169">String</span><span class="sxs-lookup"><span data-stu-id="5a6e2-169">String</span></span>|<span data-ttu-id="5a6e2-170">Тип сущности, которая в противном случае будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="5a6e2-171">details</span><span class="sxs-lookup"><span data-stu-id="5a6e2-171">details</span></span>|<span data-ttu-id="5a6e2-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5a6e2-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="5a6e2-173">Сведения о почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="5a6e2-174">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5a6e2-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a6e2-175">Response</span></span>
<span data-ttu-id="5a6e2-176">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-176">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a6e2-177">Пример</span><span class="sxs-lookup"><span data-stu-id="5a6e2-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a6e2-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a6e2-178">Request</span></span>
<span data-ttu-id="5a6e2-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 582

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="5a6e2-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a6e2-180">Response</span></span>
<span data-ttu-id="5a6e2-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5a6e2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





