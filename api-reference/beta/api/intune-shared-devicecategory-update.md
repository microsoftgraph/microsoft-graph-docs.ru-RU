---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ee489c1cfae88b7a2832f517bafc78131d56b36
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537087"
---
# <a name="update-devicecategory"></a><span data-ttu-id="13148-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="13148-103">Update deviceCategory</span></span>

> <span data-ttu-id="13148-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13148-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13148-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13148-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13148-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13148-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13148-107">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="13148-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13148-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13148-108">Prerequisites</span></span>

<span data-ttu-id="13148-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13148-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13148-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13148-111">Permission type</span></span>|<span data-ttu-id="13148-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13148-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13148-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13148-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="13148-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="13148-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="13148-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13148-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="13148-116">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="13148-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="13148-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13148-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13148-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13148-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13148-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13148-119">Not supported.</span></span>|
|<span data-ttu-id="13148-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="13148-120">Application</span></span>||
| <span data-ttu-id="13148-121">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="13148-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="13148-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13148-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="13148-123">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="13148-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="13148-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13148-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13148-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13148-125">HTTP Request</span></span>

<span data-ttu-id="13148-126">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="13148-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="13148-127">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="13148-127">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="13148-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13148-128">Request headers</span></span>

|<span data-ttu-id="13148-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13148-129">Header</span></span>|<span data-ttu-id="13148-130">Значение</span><span class="sxs-lookup"><span data-stu-id="13148-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13148-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13148-131">Authorization</span></span>|<span data-ttu-id="13148-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13148-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13148-133">Accept</span><span class="sxs-lookup"><span data-stu-id="13148-133">Accept</span></span>|<span data-ttu-id="13148-134">application/json</span><span class="sxs-lookup"><span data-stu-id="13148-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13148-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13148-135">Request body</span></span>

<span data-ttu-id="13148-136">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13148-136">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="13148-137">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="13148-137">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="13148-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="13148-138">Property</span></span>|<span data-ttu-id="13148-139">Тип</span><span class="sxs-lookup"><span data-stu-id="13148-139">Type</span></span>|<span data-ttu-id="13148-140">Описание</span><span class="sxs-lookup"><span data-stu-id="13148-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13148-141">id</span><span class="sxs-lookup"><span data-stu-id="13148-141">id</span></span>|<span data-ttu-id="13148-142">String</span><span class="sxs-lookup"><span data-stu-id="13148-142">String</span></span>|<span data-ttu-id="13148-143">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="13148-143">Unique identifier for the device category.</span></span> <span data-ttu-id="13148-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13148-144">Read-only.</span></span>|
|<span data-ttu-id="13148-145">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="13148-145">**Onboarding**</span></span>|
|<span data-ttu-id="13148-146">description</span><span class="sxs-lookup"><span data-stu-id="13148-146">description</span></span>|<span data-ttu-id="13148-147">String</span><span class="sxs-lookup"><span data-stu-id="13148-147">String</span></span>|<span data-ttu-id="13148-148">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="13148-148">Optional description for the device category.</span></span>|
|<span data-ttu-id="13148-149">displayName</span><span class="sxs-lookup"><span data-stu-id="13148-149">displayName</span></span>|<span data-ttu-id="13148-150">Строка</span><span class="sxs-lookup"><span data-stu-id="13148-150">String</span></span>|<span data-ttu-id="13148-151">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="13148-151">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="13148-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="13148-152">Response</span></span>

<span data-ttu-id="13148-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13148-153">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13148-154">Пример</span><span class="sxs-lookup"><span data-stu-id="13148-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="13148-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="13148-155">Request</span></span>

<span data-ttu-id="13148-156">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="13148-156">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="13148-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="13148-157">Response</span></span>

<span data-ttu-id="13148-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13148-158">Here is an example of the response.</span></span> <span data-ttu-id="13148-159">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="13148-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13148-160">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="13148-160">Response properties will vary according to context.</span></span>

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









