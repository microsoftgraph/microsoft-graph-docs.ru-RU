---
title: Get iosManagedAppRegistration
description: Чтение свойств и связей объекта iosManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: 8d0a93b9cddce5c21d923758b783ab7e40d5b27b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354693"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="09362-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="09362-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="09362-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="09362-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09362-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09362-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09362-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09362-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09362-107">Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="09362-107">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09362-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="09362-108">Prerequisites</span></span>
<span data-ttu-id="09362-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09362-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09362-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09362-111">Permission type</span></span>|<span data-ttu-id="09362-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09362-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09362-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09362-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09362-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="09362-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="09362-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09362-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09362-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09362-116">Not supported.</span></span>|
|<span data-ttu-id="09362-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09362-117">Application</span></span>|<span data-ttu-id="09362-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09362-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09362-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09362-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09362-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="09362-120">Optional query parameters</span></span>
<span data-ttu-id="09362-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="09362-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="09362-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09362-122">Request headers</span></span>
|<span data-ttu-id="09362-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09362-123">Header</span></span>|<span data-ttu-id="09362-124">Значение</span><span class="sxs-lookup"><span data-stu-id="09362-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09362-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09362-125">Authorization</span></span>|<span data-ttu-id="09362-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="09362-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09362-127">Accept</span><span class="sxs-lookup"><span data-stu-id="09362-127">Accept</span></span>|<span data-ttu-id="09362-128">application/json</span><span class="sxs-lookup"><span data-stu-id="09362-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09362-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09362-129">Request body</span></span>
<span data-ttu-id="09362-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09362-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09362-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="09362-131">Response</span></span>
<span data-ttu-id="09362-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="09362-132">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09362-133">Пример</span><span class="sxs-lookup"><span data-stu-id="09362-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="09362-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="09362-134">Request</span></span>
<span data-ttu-id="09362-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09362-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="09362-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="09362-136">Response</span></span>
<span data-ttu-id="09362-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="09362-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

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
    "managedDeviceId": "Managed Device Id value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
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





