---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a158ca444c631e8797ab3f3ce2ec95f525f0f1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512099"
---
# <a name="get-devicecategory"></a><span data-ttu-id="91bb9-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="91bb9-103">Get deviceCategory</span></span>

<span data-ttu-id="91bb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91bb9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91bb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91bb9-106">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="91bb9-106">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91bb9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="91bb9-107">Prerequisites</span></span>
<span data-ttu-id="91bb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91bb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91bb9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91bb9-110">Permission type</span></span>|<span data-ttu-id="91bb9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91bb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91bb9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91bb9-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="91bb9-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="91bb9-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="91bb9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="91bb9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="91bb9-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="91bb9-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="91bb9-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="91bb9-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="91bb9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91bb9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91bb9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bb9-118">Not supported.</span></span>|
|<span data-ttu-id="91bb9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91bb9-119">Application</span></span>|<span data-ttu-id="91bb9-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bb9-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91bb9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91bb9-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91bb9-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91bb9-122">Optional query parameters</span></span>
<span data-ttu-id="91bb9-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91bb9-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91bb9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91bb9-124">Request headers</span></span>
|<span data-ttu-id="91bb9-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91bb9-125">Header</span></span>|<span data-ttu-id="91bb9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="91bb9-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91bb9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="91bb9-127">Authorization</span></span>|<span data-ttu-id="91bb9-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91bb9-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91bb9-129">Accept</span><span class="sxs-lookup"><span data-stu-id="91bb9-129">Accept</span></span>|<span data-ttu-id="91bb9-130">application/json</span><span class="sxs-lookup"><span data-stu-id="91bb9-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91bb9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91bb9-131">Request body</span></span>
<span data-ttu-id="91bb9-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91bb9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91bb9-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="91bb9-133">Response</span></span>
<span data-ttu-id="91bb9-134">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91bb9-134">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91bb9-135">Пример</span><span class="sxs-lookup"><span data-stu-id="91bb9-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="91bb9-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="91bb9-136">Request</span></span>
<span data-ttu-id="91bb9-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91bb9-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="91bb9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="91bb9-138">Response</span></span>
<span data-ttu-id="91bb9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91bb9-139">Here is an example of the response.</span></span> <span data-ttu-id="91bb9-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="91bb9-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="91bb9-141">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="91bb9-141">Properties returned from an actual call vary according to context.</span></span>

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




