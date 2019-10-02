---
title: Обновление объекта windows10EnterpriseModernAppManagementConfiguration
description: Обновление свойств объекта windows10EnterpriseModernAppManagementConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c75df60caf240825b3f5685424c15d0dbe92960
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365420"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="13e00-103">Обновление объекта windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="13e00-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="13e00-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13e00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13e00-105">Обновление свойств объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-105">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13e00-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13e00-106">Prerequisites</span></span>
<span data-ttu-id="13e00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13e00-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13e00-109">Permission type</span></span>|<span data-ttu-id="13e00-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13e00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13e00-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13e00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13e00-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13e00-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13e00-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13e00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13e00-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13e00-114">Not supported.</span></span>|
|<span data-ttu-id="13e00-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13e00-115">Application</span></span>|<span data-ttu-id="13e00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13e00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13e00-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13e00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="13e00-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13e00-118">Request headers</span></span>
|<span data-ttu-id="13e00-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13e00-119">Header</span></span>|<span data-ttu-id="13e00-120">Значение</span><span class="sxs-lookup"><span data-stu-id="13e00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13e00-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13e00-121">Authorization</span></span>|<span data-ttu-id="13e00-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13e00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13e00-123">Accept</span><span class="sxs-lookup"><span data-stu-id="13e00-123">Accept</span></span>|<span data-ttu-id="13e00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13e00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13e00-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13e00-125">Request body</span></span>
<span data-ttu-id="13e00-126">В теле запроса добавьте представление объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13e00-126">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="13e00-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-127">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="13e00-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="13e00-128">Property</span></span>|<span data-ttu-id="13e00-129">Тип</span><span class="sxs-lookup"><span data-stu-id="13e00-129">Type</span></span>|<span data-ttu-id="13e00-130">Описание</span><span class="sxs-lookup"><span data-stu-id="13e00-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13e00-131">id</span><span class="sxs-lookup"><span data-stu-id="13e00-131">id</span></span>|<span data-ttu-id="13e00-132">String</span><span class="sxs-lookup"><span data-stu-id="13e00-132">String</span></span>|<span data-ttu-id="13e00-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13e00-133">Key of the entity.</span></span> <span data-ttu-id="13e00-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e00-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13e00-135">lastModifiedDateTime</span></span>|<span data-ttu-id="13e00-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e00-136">DateTimeOffset</span></span>|<span data-ttu-id="13e00-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="13e00-137">DateTime the object was last modified.</span></span> <span data-ttu-id="13e00-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e00-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13e00-139">createdDateTime</span></span>|<span data-ttu-id="13e00-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e00-140">DateTimeOffset</span></span>|<span data-ttu-id="13e00-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="13e00-141">DateTime the object was created.</span></span> <span data-ttu-id="13e00-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e00-143">description</span><span class="sxs-lookup"><span data-stu-id="13e00-143">description</span></span>|<span data-ttu-id="13e00-144">String</span><span class="sxs-lookup"><span data-stu-id="13e00-144">String</span></span>|<span data-ttu-id="13e00-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="13e00-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13e00-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e00-147">displayName</span><span class="sxs-lookup"><span data-stu-id="13e00-147">displayName</span></span>|<span data-ttu-id="13e00-148">Строка</span><span class="sxs-lookup"><span data-stu-id="13e00-148">String</span></span>|<span data-ttu-id="13e00-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="13e00-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13e00-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13e00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e00-151">version</span><span class="sxs-lookup"><span data-stu-id="13e00-151">version</span></span>|<span data-ttu-id="13e00-152">Int32</span><span class="sxs-lookup"><span data-stu-id="13e00-152">Int32</span></span>|<span data-ttu-id="13e00-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="13e00-153">Version of the device configuration.</span></span> <span data-ttu-id="13e00-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13e00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13e00-155">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="13e00-155">uninstallBuiltInApps</span></span>|<span data-ttu-id="13e00-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="13e00-156">Boolean</span></span>|<span data-ttu-id="13e00-157">Указывает, следует ли удалить фиксированный список встроенных приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="13e00-157">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="13e00-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e00-158">Response</span></span>
<span data-ttu-id="13e00-159">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13e00-159">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13e00-160">Пример</span><span class="sxs-lookup"><span data-stu-id="13e00-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="13e00-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="13e00-161">Request</span></span>
<span data-ttu-id="13e00-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13e00-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13e00-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e00-163">Response</span></span>
<span data-ttu-id="13e00-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13e00-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




