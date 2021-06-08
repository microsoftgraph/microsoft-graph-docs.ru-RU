---
title: Обновление объекта windows10EnterpriseModernAppManagementConfiguration
description: Обновление свойств объекта windows10EnterpriseModernAppManagementConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d452a0c355302e9423663b0154c16c0044cb7cbe
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760526"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="42c1b-103">Обновление объекта windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="42c1b-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="42c1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42c1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42c1b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42c1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42c1b-106">Обновление свойств объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42c1b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="42c1b-107">Prerequisites</span></span>
<span data-ttu-id="42c1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42c1b-110">Permission type</span></span>|<span data-ttu-id="42c1b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42c1b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42c1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42c1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42c1b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42c1b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42c1b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42c1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42c1b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c1b-115">Not supported.</span></span>|
|<span data-ttu-id="42c1b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="42c1b-116">Application</span></span>|<span data-ttu-id="42c1b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42c1b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42c1b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42c1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42c1b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42c1b-119">Request headers</span></span>
|<span data-ttu-id="42c1b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42c1b-120">Header</span></span>|<span data-ttu-id="42c1b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42c1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42c1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42c1b-122">Authorization</span></span>|<span data-ttu-id="42c1b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42c1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42c1b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42c1b-124">Accept</span></span>|<span data-ttu-id="42c1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42c1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42c1b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42c1b-126">Request body</span></span>
<span data-ttu-id="42c1b-127">В теле запроса добавьте представление объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42c1b-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="42c1b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="42c1b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="42c1b-129">Property</span></span>|<span data-ttu-id="42c1b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42c1b-130">Type</span></span>|<span data-ttu-id="42c1b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42c1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42c1b-132">id</span><span class="sxs-lookup"><span data-stu-id="42c1b-132">id</span></span>|<span data-ttu-id="42c1b-133">String</span><span class="sxs-lookup"><span data-stu-id="42c1b-133">String</span></span>|<span data-ttu-id="42c1b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42c1b-134">Key of the entity.</span></span> <span data-ttu-id="42c1b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42c1b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42c1b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="42c1b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42c1b-137">DateTimeOffset</span></span>|<span data-ttu-id="42c1b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="42c1b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="42c1b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42c1b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42c1b-140">createdDateTime</span></span>|<span data-ttu-id="42c1b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42c1b-141">DateTimeOffset</span></span>|<span data-ttu-id="42c1b-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="42c1b-142">DateTime the object was created.</span></span> <span data-ttu-id="42c1b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42c1b-144">description</span><span class="sxs-lookup"><span data-stu-id="42c1b-144">description</span></span>|<span data-ttu-id="42c1b-145">String</span><span class="sxs-lookup"><span data-stu-id="42c1b-145">String</span></span>|<span data-ttu-id="42c1b-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42c1b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42c1b-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42c1b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="42c1b-148">displayName</span></span>|<span data-ttu-id="42c1b-149">String</span><span class="sxs-lookup"><span data-stu-id="42c1b-149">String</span></span>|<span data-ttu-id="42c1b-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42c1b-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42c1b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42c1b-152">version</span><span class="sxs-lookup"><span data-stu-id="42c1b-152">version</span></span>|<span data-ttu-id="42c1b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="42c1b-153">Int32</span></span>|<span data-ttu-id="42c1b-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42c1b-154">Version of the device configuration.</span></span> <span data-ttu-id="42c1b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42c1b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42c1b-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="42c1b-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="42c1b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="42c1b-157">Boolean</span></span>|<span data-ttu-id="42c1b-158">Указывает, следует ли удалить фиксированный список встроенных приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="42c1b-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="42c1b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="42c1b-159">Response</span></span>
<span data-ttu-id="42c1b-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42c1b-160">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c1b-161">Пример</span><span class="sxs-lookup"><span data-stu-id="42c1b-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="42c1b-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="42c1b-162">Request</span></span>
<span data-ttu-id="42c1b-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42c1b-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42c1b-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="42c1b-164">Response</span></span>
<span data-ttu-id="42c1b-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42c1b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




