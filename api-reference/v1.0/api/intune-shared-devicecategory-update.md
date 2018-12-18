---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: tfitzmac
ms.openlocfilehash: 73980aa4c178ff610ce44dc3b832c8c931d72740
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344305"
---
# <a name="update-devicecategory"></a><span data-ttu-id="cccea-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cccea-103">Update deviceCategory</span></span>

> <span data-ttu-id="cccea-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cccea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cccea-105">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="cccea-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cccea-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cccea-106">Prerequisites</span></span>
<span data-ttu-id="cccea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cccea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cccea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cccea-109">Permission type</span></span>|<span data-ttu-id="cccea-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cccea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cccea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cccea-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cccea-112">&nbsp;&nbsp; **Адаптация новых сотрудников** и</span><span class="sxs-lookup"><span data-stu-id="cccea-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="cccea-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="cccea-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="cccea-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cccea-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cccea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cccea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cccea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cccea-116">Not supported.</span></span>|
|<span data-ttu-id="cccea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cccea-117">Application</span></span>|<span data-ttu-id="cccea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cccea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cccea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cccea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="cccea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cccea-120">Request headers</span></span>
|<span data-ttu-id="cccea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cccea-121">Header</span></span>|<span data-ttu-id="cccea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cccea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cccea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cccea-123">Authorization</span></span>|<span data-ttu-id="cccea-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cccea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cccea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cccea-125">Accept</span></span>|<span data-ttu-id="cccea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cccea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cccea-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cccea-127">Request body</span></span>
<span data-ttu-id="cccea-128">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cccea-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="cccea-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="cccea-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="cccea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cccea-130">Property</span></span>|<span data-ttu-id="cccea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cccea-131">Type</span></span>|<span data-ttu-id="cccea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cccea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cccea-133">id</span><span class="sxs-lookup"><span data-stu-id="cccea-133">id</span></span>|<span data-ttu-id="cccea-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cccea-134">String</span></span>|<span data-ttu-id="cccea-135">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="cccea-135">Unique identifier for the device category.</span></span> <span data-ttu-id="cccea-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cccea-136">Read-only.</span></span>|
|<span data-ttu-id="cccea-137">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="cccea-137">**Onboarding**</span></span>|
|<span data-ttu-id="cccea-138">displayName</span><span class="sxs-lookup"><span data-stu-id="cccea-138">displayName</span></span>|<span data-ttu-id="cccea-139">String</span><span class="sxs-lookup"><span data-stu-id="cccea-139">String</span></span>|<span data-ttu-id="cccea-140">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="cccea-140">Display name for the device category.</span></span>|
|<span data-ttu-id="cccea-141">описание</span><span class="sxs-lookup"><span data-stu-id="cccea-141">description</span></span>|<span data-ttu-id="cccea-142">String</span><span class="sxs-lookup"><span data-stu-id="cccea-142">String</span></span>|<span data-ttu-id="cccea-143">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="cccea-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="cccea-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cccea-144">Response</span></span>
<span data-ttu-id="cccea-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cccea-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cccea-146">Пример</span><span class="sxs-lookup"><span data-stu-id="cccea-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="cccea-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="cccea-147">Request</span></span>
<span data-ttu-id="cccea-148">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="cccea-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cccea-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="cccea-149">Response</span></span>
<span data-ttu-id="cccea-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cccea-150">Here is an example of the response.</span></span> <span data-ttu-id="cccea-151">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cccea-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cccea-152">Свойства ответа будет отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="cccea-152">Response properties will vary according to context.</span></span>
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



