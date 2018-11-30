---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
ms.openlocfilehash: 5bd8bda5b019fee81a50c117218264975883461a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077129"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="3ec7f-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="3ec7f-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="3ec7f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ec7f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ec7f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ec7f-107">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ec7f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3ec7f-108">Prerequisites</span></span>
<span data-ttu-id="3ec7f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec7f-111">Permission type</span></span>|<span data-ttu-id="3ec7f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ec7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ec7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ec7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ec7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ec7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ec7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ec7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-116">Not supported.</span></span>|
|<span data-ttu-id="3ec7f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ec7f-117">Application</span></span>|<span data-ttu-id="3ec7f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ec7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ec7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3ec7f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ec7f-120">Request headers</span></span>
|<span data-ttu-id="3ec7f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ec7f-121">Header</span></span>|<span data-ttu-id="3ec7f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ec7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ec7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec7f-123">Authorization</span></span>|<span data-ttu-id="3ec7f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3ec7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ec7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ec7f-125">Accept</span></span>|<span data-ttu-id="3ec7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ec7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec7f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ec7f-127">Request body</span></span>
<span data-ttu-id="3ec7f-128">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="3ec7f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="3ec7f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ec7f-130">Property</span></span>|<span data-ttu-id="3ec7f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3ec7f-131">Type</span></span>|<span data-ttu-id="3ec7f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ec7f-133">id</span><span class="sxs-lookup"><span data-stu-id="3ec7f-133">id</span></span>|<span data-ttu-id="3ec7f-134">String</span><span class="sxs-lookup"><span data-stu-id="3ec7f-134">String</span></span>|<span data-ttu-id="3ec7f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-135">Key of the entity.</span></span> <span data-ttu-id="3ec7f-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ec7f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3ec7f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ec7f-138">DateTimeOffset</span></span>|<span data-ttu-id="3ec7f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3ec7f-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3ec7f-141">roleScopeTagIds</span></span>|<span data-ttu-id="3ec7f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ec7f-142">String collection</span></span>|<span data-ttu-id="3ec7f-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3ec7f-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3ec7f-145">supportsScopeTags</span></span>|<span data-ttu-id="3ec7f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="3ec7f-146">Boolean</span></span>|<span data-ttu-id="3ec7f-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3ec7f-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3ec7f-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3ec7f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-150">This property is read-only.</span></span> <span data-ttu-id="3ec7f-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ec7f-152">createdDateTime</span></span>|<span data-ttu-id="3ec7f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ec7f-153">DateTimeOffset</span></span>|<span data-ttu-id="3ec7f-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-154">DateTime the object was created.</span></span> <span data-ttu-id="3ec7f-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-156">описание</span><span class="sxs-lookup"><span data-stu-id="3ec7f-156">description</span></span>|<span data-ttu-id="3ec7f-157">String</span><span class="sxs-lookup"><span data-stu-id="3ec7f-157">String</span></span>|<span data-ttu-id="3ec7f-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3ec7f-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3ec7f-160">displayName</span></span>|<span data-ttu-id="3ec7f-161">String</span><span class="sxs-lookup"><span data-stu-id="3ec7f-161">String</span></span>|<span data-ttu-id="3ec7f-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3ec7f-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-164">version</span><span class="sxs-lookup"><span data-stu-id="3ec7f-164">version</span></span>|<span data-ttu-id="3ec7f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec7f-165">Int32</span></span>|<span data-ttu-id="3ec7f-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-166">Version of the device configuration.</span></span> <span data-ttu-id="3ec7f-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ec7f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ec7f-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="3ec7f-168">airPrintDestinations</span></span>|<span data-ttu-id="3ec7f-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3ec7f-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="3ec7f-170">Массив AirPrint принтеров, которые всегда должны быть отображены.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="3ec7f-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3ec7f-172">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="3ec7f-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3ec7f-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec7f-173">Response</span></span>
<span data-ttu-id="3ec7f-174">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-174">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec7f-175">Пример</span><span class="sxs-lookup"><span data-stu-id="3ec7f-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ec7f-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec7f-176">Request</span></span>
<span data-ttu-id="3ec7f-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ec7f-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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

### <a name="response"></a><span data-ttu-id="3ec7f-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ec7f-178">Response</span></span>
<span data-ttu-id="3ec7f-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3ec7f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





