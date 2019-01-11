---
title: Создание unsupportedDeviceConfiguration
description: Создание нового объекта unsupportedDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa776cee2504a3383db862ab4aea59fd19347f1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882784"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="8cc07-103">Создание unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cc07-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="8cc07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cc07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cc07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cc07-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8cc07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cc07-107">Создание нового объекта [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8cc07-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cc07-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8cc07-108">Prerequisites</span></span>
<span data-ttu-id="8cc07-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cc07-111">Permission type</span></span>|<span data-ttu-id="8cc07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cc07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cc07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc07-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc07-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cc07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc07-116">Not supported.</span></span>|
|<span data-ttu-id="8cc07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cc07-117">Application</span></span>|<span data-ttu-id="8cc07-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cc07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8cc07-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cc07-120">Request headers</span></span>
|<span data-ttu-id="8cc07-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cc07-121">Header</span></span>|<span data-ttu-id="8cc07-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8cc07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc07-123">Authorization</span></span>|<span data-ttu-id="8cc07-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8cc07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc07-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cc07-125">Accept</span></span>|<span data-ttu-id="8cc07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc07-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8cc07-127">Request body</span></span>
<span data-ttu-id="8cc07-128">В тексте запроса укажите представление JSON для объекта unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8cc07-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="8cc07-129">В следующей таблице показаны свойства, которые необходимы для создания unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8cc07-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="8cc07-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc07-130">Property</span></span>|<span data-ttu-id="8cc07-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc07-131">Type</span></span>|<span data-ttu-id="8cc07-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc07-133">id</span><span class="sxs-lookup"><span data-stu-id="8cc07-133">id</span></span>|<span data-ttu-id="8cc07-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc07-134">String</span></span>|<span data-ttu-id="8cc07-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8cc07-135">Key of the entity.</span></span> <span data-ttu-id="8cc07-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc07-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc07-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc07-138">DateTimeOffset</span></span>|<span data-ttu-id="8cc07-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8cc07-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8cc07-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cc07-141">roleScopeTagIds</span></span>|<span data-ttu-id="8cc07-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8cc07-142">String collection</span></span>|<span data-ttu-id="8cc07-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8cc07-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8cc07-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8cc07-145">supportsScopeTags</span></span>|<span data-ttu-id="8cc07-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8cc07-146">Boolean</span></span>|<span data-ttu-id="8cc07-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="8cc07-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8cc07-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="8cc07-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8cc07-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8cc07-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8cc07-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cc07-150">This property is read-only.</span></span> <span data-ttu-id="8cc07-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc07-152">createdDateTime</span></span>|<span data-ttu-id="8cc07-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc07-153">DateTimeOffset</span></span>|<span data-ttu-id="8cc07-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8cc07-154">DateTime the object was created.</span></span> <span data-ttu-id="8cc07-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-156">описание</span><span class="sxs-lookup"><span data-stu-id="8cc07-156">description</span></span>|<span data-ttu-id="8cc07-157">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc07-157">String</span></span>|<span data-ttu-id="8cc07-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8cc07-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8cc07-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc07-160">displayName</span></span>|<span data-ttu-id="8cc07-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc07-161">String</span></span>|<span data-ttu-id="8cc07-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8cc07-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8cc07-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-164">version</span><span class="sxs-lookup"><span data-stu-id="8cc07-164">version</span></span>|<span data-ttu-id="8cc07-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc07-165">Int32</span></span>|<span data-ttu-id="8cc07-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8cc07-166">Version of the device configuration.</span></span> <span data-ttu-id="8cc07-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc07-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc07-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="8cc07-168">originalEntityTypeName</span></span>|<span data-ttu-id="8cc07-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc07-169">String</span></span>|<span data-ttu-id="8cc07-170">Тип сущности, которая в противном случае будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="8cc07-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="8cc07-171">details</span><span class="sxs-lookup"><span data-stu-id="8cc07-171">details</span></span>|<span data-ttu-id="8cc07-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8cc07-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="8cc07-173">Сведения о почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc07-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="8cc07-174">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8cc07-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8cc07-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cc07-175">Response</span></span>
<span data-ttu-id="8cc07-176">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8cc07-176">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc07-177">Пример</span><span class="sxs-lookup"><span data-stu-id="8cc07-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cc07-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cc07-178">Request</span></span>
<span data-ttu-id="8cc07-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cc07-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8cc07-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cc07-180">Response</span></span>
<span data-ttu-id="8cc07-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8cc07-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





