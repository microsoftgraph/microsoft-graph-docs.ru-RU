---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 029a793172ef2ce7b9d9a279e1b3fcc746631d63
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390940"
---
# <a name="update-devicecategory"></a><span data-ttu-id="1a228-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1a228-103">Update deviceCategory</span></span>

<span data-ttu-id="1a228-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a228-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a228-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a228-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a228-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a228-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a228-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a228-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a228-108">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1a228-108">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a228-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a228-109">Prerequisites</span></span>

<span data-ttu-id="1a228-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a228-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a228-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a228-112">Permission type</span></span>|<span data-ttu-id="1a228-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a228-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a228-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a228-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1a228-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="1a228-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1a228-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a228-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="1a228-117">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="1a228-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1a228-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a228-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a228-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a228-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a228-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a228-120">Not supported.</span></span>|
|<span data-ttu-id="1a228-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1a228-121">Application</span></span>||
| <span data-ttu-id="1a228-122">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="1a228-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1a228-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a228-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="1a228-124">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="1a228-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1a228-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a228-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a228-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a228-126">HTTP Request</span></span>

<span data-ttu-id="1a228-127">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="1a228-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="1a228-128">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="1a228-128">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="1a228-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a228-129">Request headers</span></span>

|<span data-ttu-id="1a228-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a228-130">Header</span></span>|<span data-ttu-id="1a228-131">Значение</span><span class="sxs-lookup"><span data-stu-id="1a228-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a228-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a228-132">Authorization</span></span>|<span data-ttu-id="1a228-133">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a228-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a228-134">Accept</span><span class="sxs-lookup"><span data-stu-id="1a228-134">Accept</span></span>|<span data-ttu-id="1a228-135">application/json</span><span class="sxs-lookup"><span data-stu-id="1a228-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a228-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a228-136">Request body</span></span>

<span data-ttu-id="1a228-137">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a228-137">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="1a228-138">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1a228-138">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="1a228-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a228-139">Property</span></span>|<span data-ttu-id="1a228-140">Тип</span><span class="sxs-lookup"><span data-stu-id="1a228-140">Type</span></span>|<span data-ttu-id="1a228-141">Описание</span><span class="sxs-lookup"><span data-stu-id="1a228-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a228-142">id</span><span class="sxs-lookup"><span data-stu-id="1a228-142">id</span></span>|<span data-ttu-id="1a228-143">String</span><span class="sxs-lookup"><span data-stu-id="1a228-143">String</span></span>|<span data-ttu-id="1a228-144">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="1a228-144">Unique identifier for the device category.</span></span> <span data-ttu-id="1a228-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a228-145">Read-only.</span></span>|
|<span data-ttu-id="1a228-146">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="1a228-146">**Onboarding**</span></span>|
|<span data-ttu-id="1a228-147">description</span><span class="sxs-lookup"><span data-stu-id="1a228-147">description</span></span>|<span data-ttu-id="1a228-148">String</span><span class="sxs-lookup"><span data-stu-id="1a228-148">String</span></span>|<span data-ttu-id="1a228-149">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="1a228-149">Optional description for the device category.</span></span>|
|<span data-ttu-id="1a228-150">displayName</span><span class="sxs-lookup"><span data-stu-id="1a228-150">displayName</span></span>|<span data-ttu-id="1a228-151">Строка</span><span class="sxs-lookup"><span data-stu-id="1a228-151">String</span></span>|<span data-ttu-id="1a228-152">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="1a228-152">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="1a228-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a228-153">Response</span></span>

<span data-ttu-id="1a228-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a228-154">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a228-155">Пример</span><span class="sxs-lookup"><span data-stu-id="1a228-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a228-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a228-156">Request</span></span>

<span data-ttu-id="1a228-157">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="1a228-157">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="1a228-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a228-158">Response</span></span>

<span data-ttu-id="1a228-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a228-159">Here is an example of the response.</span></span> <span data-ttu-id="1a228-160">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1a228-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1a228-161">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="1a228-161">Response properties will vary according to context.</span></span>

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









