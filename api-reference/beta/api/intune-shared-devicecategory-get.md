---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d3383f3237a47542c80c834467689a93c20ee6d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350904"
---
# <a name="get-devicecategory"></a><span data-ttu-id="e6438-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="e6438-103">Get deviceCategory</span></span>

> <span data-ttu-id="e6438-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6438-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6438-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6438-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6438-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6438-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6438-107">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="e6438-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6438-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e6438-108">Prerequisites</span></span>

<span data-ttu-id="e6438-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6438-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6438-111">Permission type</span></span>|<span data-ttu-id="e6438-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6438-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6438-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6438-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e6438-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e6438-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e6438-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6438-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="e6438-116">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="e6438-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e6438-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6438-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e6438-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6438-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6438-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6438-119">Not supported.</span></span>|
|<span data-ttu-id="e6438-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6438-120">Application</span></span>|<span data-ttu-id="e6438-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6438-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6438-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6438-122">HTTP Request</span></span>

<span data-ttu-id="e6438-123">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e6438-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="e6438-124">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="e6438-124">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6438-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6438-125">Optional query parameters</span></span>

<span data-ttu-id="e6438-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6438-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6438-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6438-127">Request headers</span></span>

|<span data-ttu-id="e6438-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6438-128">Header</span></span>|<span data-ttu-id="e6438-129">Значение</span><span class="sxs-lookup"><span data-stu-id="e6438-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6438-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6438-130">Authorization</span></span>|<span data-ttu-id="e6438-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6438-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6438-132">Accept</span><span class="sxs-lookup"><span data-stu-id="e6438-132">Accept</span></span>|<span data-ttu-id="e6438-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e6438-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6438-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6438-134">Request body</span></span>

<span data-ttu-id="e6438-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6438-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6438-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6438-136">Response</span></span>

<span data-ttu-id="e6438-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e6438-137">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6438-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e6438-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6438-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6438-139">Request</span></span>

<span data-ttu-id="e6438-140">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="e6438-140">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="e6438-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6438-141">Response</span></span>

<span data-ttu-id="e6438-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6438-142">Here is an example of the response.</span></span> <span data-ttu-id="e6438-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e6438-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e6438-144">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="e6438-144">Properties returned from an actual call vary according to context.</span></span>

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






