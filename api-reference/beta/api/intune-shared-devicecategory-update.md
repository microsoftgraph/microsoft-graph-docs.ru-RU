---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90f5305e2fb52b5ecd184aad837f2c9d8f6334ef
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395015"
---
# <a name="update-devicecategory"></a><span data-ttu-id="22797-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="22797-103">Update deviceCategory</span></span>

> <span data-ttu-id="22797-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22797-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22797-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22797-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22797-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22797-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22797-107">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="22797-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22797-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="22797-108">Prerequisites</span></span>

<span data-ttu-id="22797-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22797-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22797-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22797-111">Permission type</span></span>|<span data-ttu-id="22797-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22797-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22797-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22797-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="22797-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="22797-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="22797-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22797-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="22797-116">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="22797-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="22797-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22797-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="22797-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22797-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22797-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22797-119">Not supported.</span></span>|
|<span data-ttu-id="22797-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22797-120">Application</span></span>|<span data-ttu-id="22797-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22797-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22797-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22797-122">HTTP Request</span></span>

<span data-ttu-id="22797-123">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="22797-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="22797-124">**На использование доски**</span><span class="sxs-lookup"><span data-stu-id="22797-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="22797-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22797-125">Request headers</span></span>

|<span data-ttu-id="22797-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22797-126">Header</span></span>|<span data-ttu-id="22797-127">Значение</span><span class="sxs-lookup"><span data-stu-id="22797-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22797-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="22797-128">Authorization</span></span>|<span data-ttu-id="22797-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22797-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22797-130">Accept</span><span class="sxs-lookup"><span data-stu-id="22797-130">Accept</span></span>|<span data-ttu-id="22797-131">application/json</span><span class="sxs-lookup"><span data-stu-id="22797-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22797-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22797-132">Request body</span></span>

<span data-ttu-id="22797-133">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22797-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="22797-134">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="22797-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="22797-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="22797-135">Property</span></span>|<span data-ttu-id="22797-136">Тип</span><span class="sxs-lookup"><span data-stu-id="22797-136">Type</span></span>|<span data-ttu-id="22797-137">Описание</span><span class="sxs-lookup"><span data-stu-id="22797-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22797-138">id</span><span class="sxs-lookup"><span data-stu-id="22797-138">id</span></span>|<span data-ttu-id="22797-139">String</span><span class="sxs-lookup"><span data-stu-id="22797-139">String</span></span>|<span data-ttu-id="22797-140">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="22797-140">Unique identifier for the device category.</span></span> <span data-ttu-id="22797-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22797-141">Read-only.</span></span>|
|<span data-ttu-id="22797-142">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="22797-142">**Onboarding**</span></span>|
|<span data-ttu-id="22797-143">description</span><span class="sxs-lookup"><span data-stu-id="22797-143">description</span></span>|<span data-ttu-id="22797-144">String</span><span class="sxs-lookup"><span data-stu-id="22797-144">String</span></span>|<span data-ttu-id="22797-145">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="22797-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="22797-146">displayName</span><span class="sxs-lookup"><span data-stu-id="22797-146">displayName</span></span>|<span data-ttu-id="22797-147">String</span><span class="sxs-lookup"><span data-stu-id="22797-147">String</span></span>|<span data-ttu-id="22797-148">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="22797-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="22797-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="22797-149">Response</span></span>

<span data-ttu-id="22797-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="22797-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22797-151">Пример</span><span class="sxs-lookup"><span data-stu-id="22797-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="22797-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="22797-152">Request</span></span>

<span data-ttu-id="22797-153">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="22797-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="22797-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="22797-154">Response</span></span>

<span data-ttu-id="22797-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22797-155">Here is an example of the response.</span></span> <span data-ttu-id="22797-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="22797-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="22797-157">Свойства ответа будет отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="22797-157">Response properties will vary according to context.</span></span>

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



