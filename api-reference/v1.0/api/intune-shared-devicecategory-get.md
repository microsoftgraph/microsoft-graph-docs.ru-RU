---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
ms.openlocfilehash: 89b8f46aae22c87ea1462cc70eeb3e28e9bfa230
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027712"
---
# <a name="get-devicecategory"></a><span data-ttu-id="c4870-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c4870-103">Get deviceCategory</span></span>



> <span data-ttu-id="c4870-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4870-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4870-105">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="c4870-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4870-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c4870-106">Prerequisites</span></span>
<span data-ttu-id="c4870-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4870-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4870-109">Permission type</span></span>|<span data-ttu-id="c4870-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4870-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4870-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4870-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c4870-112">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c4870-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c4870-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4870-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="c4870-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="c4870-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c4870-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4870-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c4870-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4870-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4870-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4870-117">Not supported.</span></span>|
|<span data-ttu-id="c4870-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4870-118">Application</span></span>|<span data-ttu-id="c4870-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4870-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4870-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4870-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4870-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4870-121">Optional query parameters</span></span>
<span data-ttu-id="c4870-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4870-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4870-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4870-123">Request headers</span></span>
|<span data-ttu-id="c4870-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4870-124">Header</span></span>|<span data-ttu-id="c4870-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c4870-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4870-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4870-126">Authorization</span></span>|<span data-ttu-id="c4870-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c4870-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4870-128">Accept</span><span class="sxs-lookup"><span data-stu-id="c4870-128">Accept</span></span>|<span data-ttu-id="c4870-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c4870-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4870-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4870-130">Request body</span></span>
<span data-ttu-id="c4870-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4870-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4870-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4870-132">Response</span></span>
<span data-ttu-id="c4870-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4870-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4870-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c4870-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4870-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4870-135">Request</span></span>
<span data-ttu-id="c4870-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4870-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="c4870-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4870-137">Response</span></span>
<span data-ttu-id="c4870-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4870-138">Here is an example of the response.</span></span> <span data-ttu-id="c4870-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c4870-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c4870-140">Свойства, возвращенные фактический вызов различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="c4870-140">Properties returned from an actual call vary according to context.</span></span>

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



