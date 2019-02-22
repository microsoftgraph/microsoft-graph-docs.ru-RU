---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bccd64c5fc4b102340407ba1967a3b101c0b43e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148974"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="20fbf-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="20fbf-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="20fbf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20fbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20fbf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20fbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20fbf-106">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20fbf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20fbf-107">Prerequisites</span></span>
<span data-ttu-id="20fbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="20fbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20fbf-110">Permission type</span></span>|<span data-ttu-id="20fbf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20fbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20fbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20fbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20fbf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20fbf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20fbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20fbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20fbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20fbf-115">Not supported.</span></span>|
|<span data-ttu-id="20fbf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20fbf-116">Application</span></span>|<span data-ttu-id="20fbf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20fbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20fbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20fbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="20fbf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20fbf-119">Request headers</span></span>
|<span data-ttu-id="20fbf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20fbf-120">Header</span></span>|<span data-ttu-id="20fbf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="20fbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20fbf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20fbf-122">Authorization</span></span>|<span data-ttu-id="20fbf-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20fbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20fbf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="20fbf-124">Accept</span></span>|<span data-ttu-id="20fbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20fbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20fbf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20fbf-126">Request body</span></span>
<span data-ttu-id="20fbf-127">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20fbf-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="20fbf-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="20fbf-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="20fbf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="20fbf-129">Property</span></span>|<span data-ttu-id="20fbf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20fbf-130">Type</span></span>|<span data-ttu-id="20fbf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20fbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20fbf-132">id</span><span class="sxs-lookup"><span data-stu-id="20fbf-132">id</span></span>|<span data-ttu-id="20fbf-133">String</span><span class="sxs-lookup"><span data-stu-id="20fbf-133">String</span></span>|<span data-ttu-id="20fbf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20fbf-134">Key of the entity.</span></span> <span data-ttu-id="20fbf-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20fbf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="20fbf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20fbf-137">DateTimeOffset</span></span>|<span data-ttu-id="20fbf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="20fbf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="20fbf-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20fbf-140">roleScopeTagIds</span></span>|<span data-ttu-id="20fbf-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20fbf-141">String collection</span></span>|<span data-ttu-id="20fbf-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="20fbf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20fbf-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="20fbf-144">supportsScopeTags</span></span>|<span data-ttu-id="20fbf-145">Логический</span><span class="sxs-lookup"><span data-stu-id="20fbf-145">Boolean</span></span>|<span data-ttu-id="20fbf-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="20fbf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20fbf-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="20fbf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20fbf-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="20fbf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20fbf-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20fbf-149">This property is read-only.</span></span> <span data-ttu-id="20fbf-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20fbf-151">createdDateTime</span></span>|<span data-ttu-id="20fbf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20fbf-152">DateTimeOffset</span></span>|<span data-ttu-id="20fbf-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="20fbf-153">DateTime the object was created.</span></span> <span data-ttu-id="20fbf-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-155">description</span><span class="sxs-lookup"><span data-stu-id="20fbf-155">description</span></span>|<span data-ttu-id="20fbf-156">String</span><span class="sxs-lookup"><span data-stu-id="20fbf-156">String</span></span>|<span data-ttu-id="20fbf-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20fbf-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20fbf-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="20fbf-159">displayName</span></span>|<span data-ttu-id="20fbf-160">String</span><span class="sxs-lookup"><span data-stu-id="20fbf-160">String</span></span>|<span data-ttu-id="20fbf-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20fbf-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20fbf-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-163">version</span><span class="sxs-lookup"><span data-stu-id="20fbf-163">version</span></span>|<span data-ttu-id="20fbf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="20fbf-164">Int32</span></span>|<span data-ttu-id="20fbf-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20fbf-165">Version of the device configuration.</span></span> <span data-ttu-id="20fbf-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20fbf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20fbf-167">Аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="20fbf-167">airPrintDestinations</span></span>|<span data-ttu-id="20fbf-168">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="20fbf-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="20fbf-169">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="20fbf-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="20fbf-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="20fbf-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="20fbf-171">НаСледуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="20fbf-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="20fbf-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="20fbf-172">Response</span></span>
<span data-ttu-id="20fbf-173">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20fbf-173">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20fbf-174">Пример</span><span class="sxs-lookup"><span data-stu-id="20fbf-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="20fbf-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="20fbf-175">Request</span></span>
<span data-ttu-id="20fbf-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20fbf-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 500

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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

### <a name="response"></a><span data-ttu-id="20fbf-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="20fbf-177">Response</span></span>
<span data-ttu-id="20fbf-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20fbf-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




