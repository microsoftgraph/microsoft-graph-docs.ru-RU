---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfa547c14f49c98d3b1f11e3ae8d3a7bb6427be3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537094"
---
# <a name="get-devicecategory"></a><span data-ttu-id="c67e2-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c67e2-103">Get deviceCategory</span></span>

> <span data-ttu-id="c67e2-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c67e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c67e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c67e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c67e2-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c67e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c67e2-107">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="c67e2-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c67e2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c67e2-108">Prerequisites</span></span>

<span data-ttu-id="c67e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c67e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c67e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c67e2-111">Permission type</span></span>|<span data-ttu-id="c67e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c67e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c67e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c67e2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c67e2-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c67e2-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c67e2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c67e2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="c67e2-116">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c67e2-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c67e2-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c67e2-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c67e2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c67e2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c67e2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c67e2-119">Not supported.</span></span>|
|<span data-ttu-id="c67e2-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="c67e2-120">Application</span></span>||
| <span data-ttu-id="c67e2-121">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c67e2-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c67e2-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c67e2-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="c67e2-123">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c67e2-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c67e2-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c67e2-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c67e2-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c67e2-125">HTTP Request</span></span>

<span data-ttu-id="c67e2-126">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c67e2-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="c67e2-127">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c67e2-127">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c67e2-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c67e2-128">Optional query parameters</span></span>

<span data-ttu-id="c67e2-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c67e2-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c67e2-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c67e2-130">Request headers</span></span>

|<span data-ttu-id="c67e2-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c67e2-131">Header</span></span>|<span data-ttu-id="c67e2-132">Значение</span><span class="sxs-lookup"><span data-stu-id="c67e2-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c67e2-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c67e2-133">Authorization</span></span>|<span data-ttu-id="c67e2-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c67e2-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c67e2-135">Accept</span><span class="sxs-lookup"><span data-stu-id="c67e2-135">Accept</span></span>|<span data-ttu-id="c67e2-136">application/json</span><span class="sxs-lookup"><span data-stu-id="c67e2-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c67e2-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c67e2-137">Request body</span></span>

<span data-ttu-id="c67e2-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c67e2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c67e2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c67e2-139">Response</span></span>

<span data-ttu-id="c67e2-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c67e2-140">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c67e2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c67e2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c67e2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c67e2-142">Request</span></span>

<span data-ttu-id="c67e2-143">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="c67e2-143">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="c67e2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c67e2-144">Response</span></span>

<span data-ttu-id="c67e2-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c67e2-145">Here is an example of the response.</span></span> <span data-ttu-id="c67e2-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c67e2-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c67e2-147">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="c67e2-147">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```









