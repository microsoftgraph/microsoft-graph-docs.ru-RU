---
title: Get detectedApp
description: Получение свойств и связей объекта detectedApp.
ms.openlocfilehash: a9b5b06a47b4606cc45ba07315331536fb4267c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024371"
---
# <a name="get-detectedapp"></a><span data-ttu-id="e540e-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="e540e-103">Get detectedApp</span></span>

> <span data-ttu-id="e540e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e540e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e540e-105">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e540e-105">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e540e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e540e-106">Prerequisites</span></span>
<span data-ttu-id="e540e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e540e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e540e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e540e-109">Permission type</span></span>|<span data-ttu-id="e540e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e540e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e540e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e540e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e540e-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e540e-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e540e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e540e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e540e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e540e-114">Not supported.</span></span>|
|<span data-ttu-id="e540e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e540e-115">Application</span></span>|<span data-ttu-id="e540e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e540e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e540e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e540e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e540e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e540e-118">Optional query parameters</span></span>
<span data-ttu-id="e540e-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e540e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e540e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e540e-120">Request headers</span></span>
|<span data-ttu-id="e540e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e540e-121">Header</span></span>|<span data-ttu-id="e540e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e540e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e540e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e540e-123">Authorization</span></span>|<span data-ttu-id="e540e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e540e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e540e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e540e-125">Accept</span></span>|<span data-ttu-id="e540e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e540e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e540e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e540e-127">Request body</span></span>
<span data-ttu-id="e540e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e540e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e540e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e540e-129">Response</span></span>
<span data-ttu-id="e540e-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e540e-130">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e540e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e540e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e540e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e540e-132">Request</span></span>
<span data-ttu-id="e540e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e540e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="e540e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e540e-134">Response</span></span>
<span data-ttu-id="e540e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e540e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11
  }
}
```



