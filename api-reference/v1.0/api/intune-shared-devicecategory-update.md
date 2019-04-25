---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 831232fc656ad4aa0968e40aca5ae54b1e13ceef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576967"
---
# <a name="update-devicecategory"></a><span data-ttu-id="15665-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="15665-103">Update deviceCategory</span></span>

> <span data-ttu-id="15665-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15665-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15665-105">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="15665-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15665-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="15665-106">Prerequisites</span></span>
<span data-ttu-id="15665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15665-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15665-109">Permission type</span></span>|<span data-ttu-id="15665-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15665-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15665-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15665-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="15665-112">&nbsp;&nbsp; \*\*\*\* Подключение и</span><span class="sxs-lookup"><span data-stu-id="15665-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="15665-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="15665-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="15665-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15665-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="15665-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15665-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15665-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15665-116">Not supported.</span></span>|
|<span data-ttu-id="15665-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15665-117">Application</span></span>|<span data-ttu-id="15665-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15665-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15665-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15665-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="15665-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15665-120">Request headers</span></span>
|<span data-ttu-id="15665-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15665-121">Header</span></span>|<span data-ttu-id="15665-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15665-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15665-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15665-123">Authorization</span></span>|<span data-ttu-id="15665-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15665-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15665-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15665-125">Accept</span></span>|<span data-ttu-id="15665-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15665-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15665-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15665-127">Request body</span></span>
<span data-ttu-id="15665-128">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15665-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="15665-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="15665-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="15665-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15665-130">Property</span></span>|<span data-ttu-id="15665-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15665-131">Type</span></span>|<span data-ttu-id="15665-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15665-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15665-133">id</span><span class="sxs-lookup"><span data-stu-id="15665-133">id</span></span>|<span data-ttu-id="15665-134">Строка</span><span class="sxs-lookup"><span data-stu-id="15665-134">String</span></span>|<span data-ttu-id="15665-135">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="15665-135">Unique identifier for the device category.</span></span> <span data-ttu-id="15665-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15665-136">Read-only.</span></span>|
|<span data-ttu-id="15665-137">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="15665-137">**Onboarding**</span></span>|
|<span data-ttu-id="15665-138">displayName</span><span class="sxs-lookup"><span data-stu-id="15665-138">displayName</span></span>|<span data-ttu-id="15665-139">String</span><span class="sxs-lookup"><span data-stu-id="15665-139">String</span></span>|<span data-ttu-id="15665-140">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="15665-140">Display name for the device category.</span></span>|
|<span data-ttu-id="15665-141">description</span><span class="sxs-lookup"><span data-stu-id="15665-141">description</span></span>|<span data-ttu-id="15665-142">String</span><span class="sxs-lookup"><span data-stu-id="15665-142">String</span></span>|<span data-ttu-id="15665-143">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="15665-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="15665-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="15665-144">Response</span></span>
<span data-ttu-id="15665-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15665-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15665-146">Пример</span><span class="sxs-lookup"><span data-stu-id="15665-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="15665-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="15665-147">Request</span></span>
<span data-ttu-id="15665-148">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="15665-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15665-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="15665-149">Response</span></span>
<span data-ttu-id="15665-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15665-150">Here is an example of the response.</span></span> <span data-ttu-id="15665-151">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="15665-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="15665-152">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="15665-152">Response properties will vary according to context.</span></span>
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



