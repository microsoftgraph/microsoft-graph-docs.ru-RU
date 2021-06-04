---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8690e7db843c4769a1f3646ec5199240f1e98765
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732721"
---
# <a name="update-devicecategory"></a><span data-ttu-id="8bea4-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8bea4-103">Update deviceCategory</span></span>

<span data-ttu-id="8bea4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bea4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bea4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bea4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bea4-106">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8bea4-106">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bea4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8bea4-107">Prerequisites</span></span>
<span data-ttu-id="8bea4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bea4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bea4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bea4-110">Permission type</span></span>|<span data-ttu-id="8bea4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bea4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bea4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bea4-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8bea4-113">&nbsp;&nbsp; **Бортовая и**</span><span class="sxs-lookup"><span data-stu-id="8bea4-113">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="8bea4-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="8bea4-114">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="8bea4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bea4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8bea4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bea4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bea4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bea4-117">Not supported.</span></span>|
|<span data-ttu-id="8bea4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bea4-118">Application</span></span>|<span data-ttu-id="8bea4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bea4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bea4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bea4-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="8bea4-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8bea4-121">Request headers</span></span>
|<span data-ttu-id="8bea4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bea4-122">Header</span></span>|<span data-ttu-id="8bea4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8bea4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bea4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bea4-124">Authorization</span></span>|<span data-ttu-id="8bea4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bea4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bea4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8bea4-126">Accept</span></span>|<span data-ttu-id="8bea4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8bea4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bea4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bea4-128">Request body</span></span>
<span data-ttu-id="8bea4-129">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bea4-129">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="8bea4-130">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8bea4-130">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="8bea4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bea4-131">Property</span></span>|<span data-ttu-id="8bea4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8bea4-132">Type</span></span>|<span data-ttu-id="8bea4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8bea4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bea4-134">id</span><span class="sxs-lookup"><span data-stu-id="8bea4-134">id</span></span>|<span data-ttu-id="8bea4-135">String</span><span class="sxs-lookup"><span data-stu-id="8bea4-135">String</span></span>|<span data-ttu-id="8bea4-136">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="8bea4-136">Unique identifier for the device category.</span></span> <span data-ttu-id="8bea4-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bea4-137">Read-only.</span></span>|
|<span data-ttu-id="8bea4-138">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="8bea4-138">**Onboarding**</span></span>|
|<span data-ttu-id="8bea4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8bea4-139">displayName</span></span>|<span data-ttu-id="8bea4-140">String</span><span class="sxs-lookup"><span data-stu-id="8bea4-140">String</span></span>|<span data-ttu-id="8bea4-141">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="8bea4-141">Display name for the device category.</span></span>|
|<span data-ttu-id="8bea4-142">description</span><span class="sxs-lookup"><span data-stu-id="8bea4-142">description</span></span>|<span data-ttu-id="8bea4-143">String</span><span class="sxs-lookup"><span data-stu-id="8bea4-143">String</span></span>|<span data-ttu-id="8bea4-144">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="8bea4-144">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="8bea4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bea4-145">Response</span></span>
<span data-ttu-id="8bea4-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8bea4-146">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bea4-147">Пример</span><span class="sxs-lookup"><span data-stu-id="8bea4-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bea4-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bea4-148">Request</span></span>
<span data-ttu-id="8bea4-149">Вот примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="8bea4-149">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="8bea4-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bea4-150">Response</span></span>
<span data-ttu-id="8bea4-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bea4-151">Here is an example of the response.</span></span> <span data-ttu-id="8bea4-152">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8bea4-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8bea4-153">Свойства отклика будут отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="8bea4-153">Response properties will vary according to context.</span></span>
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









