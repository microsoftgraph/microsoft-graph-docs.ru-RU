---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40fecdf307c73c0fed94f10122c40ac268bafa45
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52749167"
---
# <a name="update-devicecategory"></a><span data-ttu-id="812ac-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="812ac-103">Update deviceCategory</span></span>

<span data-ttu-id="812ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="812ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="812ac-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="812ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="812ac-106">Обновление свойств объекта [deviceCategory](../resources/intune-devices-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="812ac-106">Update the properties of a [deviceCategory](../resources/intune-devices-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="812ac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="812ac-107">Prerequisites</span></span>
<span data-ttu-id="812ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="812ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="812ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="812ac-110">Permission type</span></span>|<span data-ttu-id="812ac-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="812ac-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="812ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="812ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="812ac-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="812ac-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="812ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="812ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="812ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="812ac-115">Not supported.</span></span>|
|<span data-ttu-id="812ac-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="812ac-116">Application</span></span>|<span data-ttu-id="812ac-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="812ac-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="812ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="812ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="812ac-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="812ac-119">Request headers</span></span>
|<span data-ttu-id="812ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="812ac-120">Header</span></span>|<span data-ttu-id="812ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="812ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="812ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="812ac-122">Authorization</span></span>|<span data-ttu-id="812ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="812ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="812ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="812ac-124">Accept</span></span>|<span data-ttu-id="812ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="812ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="812ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="812ac-126">Request body</span></span>
<span data-ttu-id="812ac-127">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-devices-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="812ac-127">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-devices-devicecategory.md) object.</span></span>

<span data-ttu-id="812ac-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-devices-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="812ac-128">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-devices-devicecategory.md).</span></span>

|<span data-ttu-id="812ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="812ac-129">Property</span></span>|<span data-ttu-id="812ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="812ac-130">Type</span></span>|<span data-ttu-id="812ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="812ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="812ac-132">id</span><span class="sxs-lookup"><span data-stu-id="812ac-132">id</span></span>|<span data-ttu-id="812ac-133">String</span><span class="sxs-lookup"><span data-stu-id="812ac-133">String</span></span>|<span data-ttu-id="812ac-134">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="812ac-134">Unique identifier for the device category.</span></span> <span data-ttu-id="812ac-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="812ac-135">Read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="812ac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ac-136">Response</span></span>
<span data-ttu-id="812ac-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-devices-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="812ac-137">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-devices-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="812ac-138">Пример</span><span class="sxs-lookup"><span data-stu-id="812ac-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="812ac-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="812ac-139">Request</span></span>
<span data-ttu-id="812ac-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="812ac-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.deviceCategory"
}
```

### <a name="response"></a><span data-ttu-id="812ac-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ac-141">Response</span></span>
<span data-ttu-id="812ac-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="812ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```




