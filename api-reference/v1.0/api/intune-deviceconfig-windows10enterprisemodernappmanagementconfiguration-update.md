---
title: Обновление объекта windows10EnterpriseModernAppManagementConfiguration
description: Обновление свойств объекта windows10EnterpriseModernAppManagementConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d856f366573de0c7188c0557765a60c934d7f8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460462"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="74b9f-103">Обновление объекта windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="74b9f-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="74b9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74b9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74b9f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74b9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74b9f-106">Обновление свойств объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74b9f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="74b9f-107">Prerequisites</span></span>
<span data-ttu-id="74b9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74b9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74b9f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74b9f-110">Permission type</span></span>|<span data-ttu-id="74b9f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74b9f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74b9f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74b9f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74b9f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74b9f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74b9f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74b9f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74b9f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74b9f-115">Not supported.</span></span>|
|<span data-ttu-id="74b9f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74b9f-116">Application</span></span>|<span data-ttu-id="74b9f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74b9f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74b9f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74b9f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="74b9f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74b9f-119">Request headers</span></span>
|<span data-ttu-id="74b9f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74b9f-120">Header</span></span>|<span data-ttu-id="74b9f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="74b9f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74b9f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74b9f-122">Authorization</span></span>|<span data-ttu-id="74b9f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74b9f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74b9f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="74b9f-124">Accept</span></span>|<span data-ttu-id="74b9f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74b9f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74b9f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74b9f-126">Request body</span></span>
<span data-ttu-id="74b9f-127">В теле запроса добавьте представление объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74b9f-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="74b9f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="74b9f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="74b9f-129">Property</span></span>|<span data-ttu-id="74b9f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="74b9f-130">Type</span></span>|<span data-ttu-id="74b9f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="74b9f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74b9f-132">id</span><span class="sxs-lookup"><span data-stu-id="74b9f-132">id</span></span>|<span data-ttu-id="74b9f-133">String</span><span class="sxs-lookup"><span data-stu-id="74b9f-133">String</span></span>|<span data-ttu-id="74b9f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="74b9f-134">Key of the entity.</span></span> <span data-ttu-id="74b9f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74b9f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74b9f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="74b9f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74b9f-137">DateTimeOffset</span></span>|<span data-ttu-id="74b9f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="74b9f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="74b9f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74b9f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74b9f-140">createdDateTime</span></span>|<span data-ttu-id="74b9f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74b9f-141">DateTimeOffset</span></span>|<span data-ttu-id="74b9f-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="74b9f-142">DateTime the object was created.</span></span> <span data-ttu-id="74b9f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74b9f-144">description</span><span class="sxs-lookup"><span data-stu-id="74b9f-144">description</span></span>|<span data-ttu-id="74b9f-145">String</span><span class="sxs-lookup"><span data-stu-id="74b9f-145">String</span></span>|<span data-ttu-id="74b9f-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="74b9f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74b9f-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74b9f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="74b9f-148">displayName</span></span>|<span data-ttu-id="74b9f-149">Строка</span><span class="sxs-lookup"><span data-stu-id="74b9f-149">String</span></span>|<span data-ttu-id="74b9f-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="74b9f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74b9f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74b9f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74b9f-152">version</span><span class="sxs-lookup"><span data-stu-id="74b9f-152">version</span></span>|<span data-ttu-id="74b9f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="74b9f-153">Int32</span></span>|<span data-ttu-id="74b9f-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="74b9f-154">Version of the device configuration.</span></span> <span data-ttu-id="74b9f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74b9f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74b9f-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="74b9f-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="74b9f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="74b9f-157">Boolean</span></span>|<span data-ttu-id="74b9f-158">Указывает, следует ли удалить фиксированный список встроенных приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="74b9f-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="74b9f-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b9f-159">Response</span></span>
<span data-ttu-id="74b9f-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="74b9f-160">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74b9f-161">Пример</span><span class="sxs-lookup"><span data-stu-id="74b9f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="74b9f-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="74b9f-162">Request</span></span>
<span data-ttu-id="74b9f-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74b9f-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="74b9f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b9f-164">Response</span></span>
<span data-ttu-id="74b9f-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74b9f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```






