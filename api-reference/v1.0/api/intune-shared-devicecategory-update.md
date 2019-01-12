---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b055f8865592e935aaa32e8a3a541151886d36de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986861"
---
# <a name="update-devicecategory"></a><span data-ttu-id="acd74-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="acd74-103">Update deviceCategory</span></span>

> <span data-ttu-id="acd74-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="acd74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acd74-105">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="acd74-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acd74-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="acd74-106">Prerequisites</span></span>
<span data-ttu-id="acd74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acd74-109">Permission type</span></span>|<span data-ttu-id="acd74-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="acd74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acd74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acd74-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="acd74-112">&nbsp;&nbsp; **Адаптация новых сотрудников** и</span><span class="sxs-lookup"><span data-stu-id="acd74-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="acd74-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="acd74-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="acd74-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acd74-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="acd74-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acd74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acd74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd74-116">Not supported.</span></span>|
|<span data-ttu-id="acd74-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acd74-117">Application</span></span>|<span data-ttu-id="acd74-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd74-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acd74-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acd74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="acd74-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acd74-120">Request headers</span></span>
|<span data-ttu-id="acd74-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acd74-121">Header</span></span>|<span data-ttu-id="acd74-122">Значение</span><span class="sxs-lookup"><span data-stu-id="acd74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acd74-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd74-123">Authorization</span></span>|<span data-ttu-id="acd74-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="acd74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acd74-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acd74-125">Accept</span></span>|<span data-ttu-id="acd74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acd74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd74-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="acd74-127">Request body</span></span>
<span data-ttu-id="acd74-128">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acd74-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="acd74-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="acd74-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="acd74-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="acd74-130">Property</span></span>|<span data-ttu-id="acd74-131">Тип</span><span class="sxs-lookup"><span data-stu-id="acd74-131">Type</span></span>|<span data-ttu-id="acd74-132">Описание</span><span class="sxs-lookup"><span data-stu-id="acd74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acd74-133">id</span><span class="sxs-lookup"><span data-stu-id="acd74-133">id</span></span>|<span data-ttu-id="acd74-134">Строка</span><span class="sxs-lookup"><span data-stu-id="acd74-134">String</span></span>|<span data-ttu-id="acd74-135">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="acd74-135">Unique identifier for the device category.</span></span> <span data-ttu-id="acd74-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="acd74-136">Read-only.</span></span>|
|<span data-ttu-id="acd74-137">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="acd74-137">**Onboarding**</span></span>|
|<span data-ttu-id="acd74-138">displayName</span><span class="sxs-lookup"><span data-stu-id="acd74-138">displayName</span></span>|<span data-ttu-id="acd74-139">String</span><span class="sxs-lookup"><span data-stu-id="acd74-139">String</span></span>|<span data-ttu-id="acd74-140">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="acd74-140">Display name for the device category.</span></span>|
|<span data-ttu-id="acd74-141">описание</span><span class="sxs-lookup"><span data-stu-id="acd74-141">description</span></span>|<span data-ttu-id="acd74-142">String</span><span class="sxs-lookup"><span data-stu-id="acd74-142">String</span></span>|<span data-ttu-id="acd74-143">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="acd74-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="acd74-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd74-144">Response</span></span>
<span data-ttu-id="acd74-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="acd74-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acd74-146">Пример</span><span class="sxs-lookup"><span data-stu-id="acd74-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="acd74-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="acd74-147">Request</span></span>
<span data-ttu-id="acd74-148">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="acd74-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="acd74-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="acd74-149">Response</span></span>
<span data-ttu-id="acd74-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="acd74-150">Here is an example of the response.</span></span> <span data-ttu-id="acd74-151">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="acd74-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="acd74-152">Свойства ответа будет отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="acd74-152">Response properties will vary according to context.</span></span>
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



