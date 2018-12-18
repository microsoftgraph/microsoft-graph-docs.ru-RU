---
title: Get androidManagedAppRegistration
description: Считывание свойств и связей объекта androidManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: 263ab41446062d97b8b51bcf0c558e91b35c0dbf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345166"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="77332-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="77332-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="77332-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77332-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77332-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77332-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77332-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="77332-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77332-107">Чтение свойств и связей объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="77332-107">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77332-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="77332-108">Prerequisites</span></span>
<span data-ttu-id="77332-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77332-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77332-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77332-111">Permission type</span></span>|<span data-ttu-id="77332-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77332-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77332-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77332-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77332-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77332-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77332-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77332-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77332-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77332-116">Not supported.</span></span>|
|<span data-ttu-id="77332-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77332-117">Application</span></span>|<span data-ttu-id="77332-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77332-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77332-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77332-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77332-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77332-120">Optional query parameters</span></span>
<span data-ttu-id="77332-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77332-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="77332-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77332-122">Request headers</span></span>
|<span data-ttu-id="77332-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77332-123">Header</span></span>|<span data-ttu-id="77332-124">Значение</span><span class="sxs-lookup"><span data-stu-id="77332-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77332-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77332-125">Authorization</span></span>|<span data-ttu-id="77332-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77332-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77332-127">Accept</span><span class="sxs-lookup"><span data-stu-id="77332-127">Accept</span></span>|<span data-ttu-id="77332-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77332-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77332-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77332-129">Request body</span></span>
<span data-ttu-id="77332-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77332-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77332-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="77332-131">Response</span></span>
<span data-ttu-id="77332-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="77332-132">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77332-133">Пример</span><span class="sxs-lookup"><span data-stu-id="77332-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="77332-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="77332-134">Request</span></span>
<span data-ttu-id="77332-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77332-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="77332-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="77332-136">Response</span></span>
<span data-ttu-id="77332-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="77332-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
      "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
      "packageId": "Package Id value"
    },
    "id": "0e064997-4997-0e06-9749-060e9749060e",
    "version": "Version value"
  }
}
```





