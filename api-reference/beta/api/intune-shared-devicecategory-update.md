---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0312497a4ea6589d89cc0e5dbd64fcb4de44f738
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729014"
---
# <a name="update-devicecategory"></a><span data-ttu-id="a542e-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a542e-103">Update deviceCategory</span></span>

<span data-ttu-id="a542e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a542e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a542e-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a542e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a542e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a542e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a542e-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a542e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a542e-108">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="a542e-108">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a542e-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a542e-109">Prerequisites</span></span>

<span data-ttu-id="a542e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a542e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a542e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a542e-112">Permission type</span></span>|<span data-ttu-id="a542e-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a542e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a542e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a542e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a542e-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="a542e-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a542e-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a542e-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="a542e-117">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="a542e-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a542e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a542e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a542e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a542e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a542e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a542e-120">Not supported.</span></span>|
|<span data-ttu-id="a542e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a542e-121">Application</span></span>||
| <span data-ttu-id="a542e-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="a542e-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a542e-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a542e-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="a542e-124">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="a542e-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a542e-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a542e-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a542e-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a542e-126">HTTP Request</span></span>

<span data-ttu-id="a542e-127">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="a542e-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="a542e-128">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="a542e-128">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a542e-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a542e-129">Request headers</span></span>

|<span data-ttu-id="a542e-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a542e-130">Header</span></span>|<span data-ttu-id="a542e-131">Значение</span><span class="sxs-lookup"><span data-stu-id="a542e-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a542e-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a542e-132">Authorization</span></span>|<span data-ttu-id="a542e-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542e-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a542e-134">Accept</span><span class="sxs-lookup"><span data-stu-id="a542e-134">Accept</span></span>|<span data-ttu-id="a542e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="a542e-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a542e-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a542e-136">Request body</span></span>

<span data-ttu-id="a542e-137">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a542e-137">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="a542e-138">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="a542e-138">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="a542e-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="a542e-139">Property</span></span>|<span data-ttu-id="a542e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="a542e-140">Type</span></span>|<span data-ttu-id="a542e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="a542e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a542e-142">id</span><span class="sxs-lookup"><span data-stu-id="a542e-142">id</span></span>|<span data-ttu-id="a542e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a542e-143">String</span></span>|<span data-ttu-id="a542e-144">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="a542e-144">Unique identifier for the device category.</span></span> <span data-ttu-id="a542e-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a542e-145">Read-only.</span></span>|
|<span data-ttu-id="a542e-146">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="a542e-146">**Onboarding**</span></span>|
|<span data-ttu-id="a542e-147">description</span><span class="sxs-lookup"><span data-stu-id="a542e-147">description</span></span>|<span data-ttu-id="a542e-148">Строка</span><span class="sxs-lookup"><span data-stu-id="a542e-148">String</span></span>|<span data-ttu-id="a542e-149">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="a542e-149">Optional description for the device category.</span></span>|
|<span data-ttu-id="a542e-150">displayName</span><span class="sxs-lookup"><span data-stu-id="a542e-150">displayName</span></span>|<span data-ttu-id="a542e-151">Строка</span><span class="sxs-lookup"><span data-stu-id="a542e-151">String</span></span>|<span data-ttu-id="a542e-152">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="a542e-152">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="a542e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a542e-153">Response</span></span>

<span data-ttu-id="a542e-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a542e-154">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a542e-155">Пример</span><span class="sxs-lookup"><span data-stu-id="a542e-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="a542e-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="a542e-156">Request</span></span>

<span data-ttu-id="a542e-157">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="a542e-157">Here are examples of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="a542e-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="a542e-158">Response</span></span>

<span data-ttu-id="a542e-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a542e-159">Here is an example of the response.</span></span> <span data-ttu-id="a542e-160">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a542e-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a542e-161">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="a542e-161">Response properties will vary according to context.</span></span>

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











