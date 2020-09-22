---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 818a23039bc761072801f83ee1991da25109fca6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019147"
---
# <a name="update-devicecategory"></a><span data-ttu-id="0ed7e-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0ed7e-103">Update deviceCategory</span></span>

<span data-ttu-id="0ed7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ed7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ed7e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ed7e-106">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0ed7e-106">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ed7e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0ed7e-107">Prerequisites</span></span>
<span data-ttu-id="0ed7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ed7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ed7e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ed7e-110">Permission type</span></span>|<span data-ttu-id="0ed7e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ed7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ed7e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ed7e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ed7e-113">&nbsp;Подключение &nbsp; **Onboarding** и</span><span class="sxs-lookup"><span data-stu-id="0ed7e-113">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="0ed7e-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0ed7e-114">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="0ed7e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed7e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ed7e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ed7e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ed7e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-117">Not supported.</span></span>|
|<span data-ttu-id="0ed7e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ed7e-118">Application</span></span>|<span data-ttu-id="0ed7e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ed7e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ed7e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="0ed7e-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ed7e-121">Request headers</span></span>
|<span data-ttu-id="0ed7e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ed7e-122">Header</span></span>|<span data-ttu-id="0ed7e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0ed7e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ed7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ed7e-124">Authorization</span></span>|<span data-ttu-id="0ed7e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ed7e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0ed7e-126">Accept</span></span>|<span data-ttu-id="0ed7e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ed7e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ed7e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ed7e-128">Request body</span></span>
<span data-ttu-id="0ed7e-129">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-129">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="0ed7e-130">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0ed7e-130">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="0ed7e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ed7e-131">Property</span></span>|<span data-ttu-id="0ed7e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0ed7e-132">Type</span></span>|<span data-ttu-id="0ed7e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0ed7e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ed7e-134">id</span><span class="sxs-lookup"><span data-stu-id="0ed7e-134">id</span></span>|<span data-ttu-id="0ed7e-135">String</span><span class="sxs-lookup"><span data-stu-id="0ed7e-135">String</span></span>|<span data-ttu-id="0ed7e-136">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-136">Unique identifier for the device category.</span></span> <span data-ttu-id="0ed7e-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-137">Read-only.</span></span>|
|<span data-ttu-id="0ed7e-138">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="0ed7e-138">**Onboarding**</span></span>|
|<span data-ttu-id="0ed7e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0ed7e-139">displayName</span></span>|<span data-ttu-id="0ed7e-140">String</span><span class="sxs-lookup"><span data-stu-id="0ed7e-140">String</span></span>|<span data-ttu-id="0ed7e-141">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-141">Display name for the device category.</span></span>|
|<span data-ttu-id="0ed7e-142">description</span><span class="sxs-lookup"><span data-stu-id="0ed7e-142">description</span></span>|<span data-ttu-id="0ed7e-143">String</span><span class="sxs-lookup"><span data-stu-id="0ed7e-143">String</span></span>|<span data-ttu-id="0ed7e-144">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-144">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="0ed7e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ed7e-145">Response</span></span>
<span data-ttu-id="0ed7e-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-146">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ed7e-147">Пример</span><span class="sxs-lookup"><span data-stu-id="0ed7e-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ed7e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ed7e-148">Request</span></span>
<span data-ttu-id="0ed7e-149">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-149">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="0ed7e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ed7e-150">Response</span></span>
<span data-ttu-id="0ed7e-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-151">Here is an example of the response.</span></span> <span data-ttu-id="0ed7e-152">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0ed7e-153">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="0ed7e-153">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```









