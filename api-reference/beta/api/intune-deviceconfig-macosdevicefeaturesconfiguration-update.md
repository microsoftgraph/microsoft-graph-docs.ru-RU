---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
ms.openlocfilehash: c174cd57fc01fce06afeca4365ac3a02ffc410e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080233"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="ab26a-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab26a-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="ab26a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab26a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab26a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab26a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab26a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab26a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab26a-107">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab26a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ab26a-108">Prerequisites</span></span>
<span data-ttu-id="ab26a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab26a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab26a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab26a-111">Permission type</span></span>|<span data-ttu-id="ab26a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab26a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab26a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab26a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab26a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab26a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab26a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab26a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab26a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab26a-116">Not supported.</span></span>|
|<span data-ttu-id="ab26a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab26a-117">Application</span></span>|<span data-ttu-id="ab26a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab26a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab26a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab26a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab26a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab26a-120">Request headers</span></span>
|<span data-ttu-id="ab26a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab26a-121">Header</span></span>|<span data-ttu-id="ab26a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab26a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab26a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab26a-123">Authorization</span></span>|<span data-ttu-id="ab26a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab26a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab26a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab26a-125">Accept</span></span>|<span data-ttu-id="ab26a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab26a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab26a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab26a-127">Request body</span></span>
<span data-ttu-id="ab26a-128">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab26a-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="ab26a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="ab26a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab26a-130">Property</span></span>|<span data-ttu-id="ab26a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab26a-131">Type</span></span>|<span data-ttu-id="ab26a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab26a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab26a-133">id</span><span class="sxs-lookup"><span data-stu-id="ab26a-133">id</span></span>|<span data-ttu-id="ab26a-134">String</span><span class="sxs-lookup"><span data-stu-id="ab26a-134">String</span></span>|<span data-ttu-id="ab26a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab26a-135">Key of the entity.</span></span> <span data-ttu-id="ab26a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab26a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ab26a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab26a-138">DateTimeOffset</span></span>|<span data-ttu-id="ab26a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab26a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ab26a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab26a-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab26a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab26a-142">String collection</span></span>|<span data-ttu-id="ab26a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ab26a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab26a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ab26a-145">supportsScopeTags</span></span>|<span data-ttu-id="ab26a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ab26a-146">Boolean</span></span>|<span data-ttu-id="ab26a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ab26a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab26a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ab26a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab26a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ab26a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab26a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab26a-150">This property is read-only.</span></span> <span data-ttu-id="ab26a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab26a-152">createdDateTime</span></span>|<span data-ttu-id="ab26a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab26a-153">DateTimeOffset</span></span>|<span data-ttu-id="ab26a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ab26a-154">DateTime the object was created.</span></span> <span data-ttu-id="ab26a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-156">описание</span><span class="sxs-lookup"><span data-stu-id="ab26a-156">description</span></span>|<span data-ttu-id="ab26a-157">String</span><span class="sxs-lookup"><span data-stu-id="ab26a-157">String</span></span>|<span data-ttu-id="ab26a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab26a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab26a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ab26a-160">displayName</span></span>|<span data-ttu-id="ab26a-161">String</span><span class="sxs-lookup"><span data-stu-id="ab26a-161">String</span></span>|<span data-ttu-id="ab26a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab26a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab26a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-164">version</span><span class="sxs-lookup"><span data-stu-id="ab26a-164">version</span></span>|<span data-ttu-id="ab26a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ab26a-165">Int32</span></span>|<span data-ttu-id="ab26a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab26a-166">Version of the device configuration.</span></span> <span data-ttu-id="ab26a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab26a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab26a-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="ab26a-168">airPrintDestinations</span></span>|<span data-ttu-id="ab26a-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ab26a-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="ab26a-170">Массив AirPrint принтеров, которые всегда должны быть отображены.</span><span class="sxs-lookup"><span data-stu-id="ab26a-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="ab26a-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ab26a-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ab26a-172">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="ab26a-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ab26a-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab26a-173">Response</span></span>
<span data-ttu-id="ab26a-174">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ab26a-174">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab26a-175">Пример</span><span class="sxs-lookup"><span data-stu-id="ab26a-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab26a-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab26a-176">Request</span></span>
<span data-ttu-id="ab26a-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab26a-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 493

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ab26a-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab26a-178">Response</span></span>
<span data-ttu-id="ab26a-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ab26a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 672

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```





