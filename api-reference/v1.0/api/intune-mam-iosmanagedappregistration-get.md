---
title: Get iosManagedAppRegistration
description: Чтение свойств и связей объекта iosManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bac379de3e185c2ae9f9e2627bafdab0e7c7ce45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844746"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="f15ee-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f15ee-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="f15ee-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f15ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f15ee-105">Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f15ee-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f15ee-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f15ee-106">Prerequisites</span></span>
<span data-ttu-id="f15ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f15ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f15ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f15ee-109">Permission type</span></span>|<span data-ttu-id="f15ee-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f15ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f15ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f15ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f15ee-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f15ee-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f15ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f15ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f15ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15ee-114">Not supported.</span></span>|
|<span data-ttu-id="f15ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f15ee-115">Application</span></span>|<span data-ttu-id="f15ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f15ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f15ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f15ee-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f15ee-118">Optional query parameters</span></span>
<span data-ttu-id="f15ee-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f15ee-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f15ee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f15ee-120">Request headers</span></span>
|<span data-ttu-id="f15ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f15ee-121">Header</span></span>|<span data-ttu-id="f15ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f15ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f15ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f15ee-123">Authorization</span></span>|<span data-ttu-id="f15ee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f15ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f15ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f15ee-125">Accept</span></span>|<span data-ttu-id="f15ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f15ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f15ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f15ee-127">Request body</span></span>
<span data-ttu-id="f15ee-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f15ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f15ee-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f15ee-129">Response</span></span>
<span data-ttu-id="f15ee-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f15ee-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f15ee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f15ee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f15ee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f15ee-132">Request</span></span>
<span data-ttu-id="f15ee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f15ee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="f15ee-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f15ee-134">Response</span></span>
<span data-ttu-id="f15ee-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f15ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 800

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```



