---
title: Get managedAppRegistration
description: Чтение свойств и связей объекта managedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 732091f588e6371d326ce6264a39e1fb3558b0d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166922"
---
# <a name="get-managedappregistration"></a><span data-ttu-id="94e37-103">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="94e37-103">Get managedAppRegistration</span></span>

> <span data-ttu-id="94e37-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94e37-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94e37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94e37-106">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="94e37-106">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94e37-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="94e37-107">Prerequisites</span></span>
<span data-ttu-id="94e37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="94e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="94e37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94e37-110">Permission type</span></span>|<span data-ttu-id="94e37-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94e37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94e37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94e37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94e37-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e37-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="94e37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94e37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e37-115">Not supported.</span></span>|
|<span data-ttu-id="94e37-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94e37-116">Application</span></span>|<span data-ttu-id="94e37-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94e37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94e37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94e37-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94e37-119">Optional query parameters</span></span>
<span data-ttu-id="94e37-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94e37-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94e37-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94e37-121">Request headers</span></span>
|<span data-ttu-id="94e37-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94e37-122">Header</span></span>|<span data-ttu-id="94e37-123">Значение</span><span class="sxs-lookup"><span data-stu-id="94e37-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94e37-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94e37-124">Authorization</span></span>|<span data-ttu-id="94e37-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="94e37-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94e37-126">Accept</span><span class="sxs-lookup"><span data-stu-id="94e37-126">Accept</span></span>|<span data-ttu-id="94e37-127">application/json</span><span class="sxs-lookup"><span data-stu-id="94e37-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e37-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94e37-128">Request body</span></span>
<span data-ttu-id="94e37-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94e37-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e37-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="94e37-130">Response</span></span>
<span data-ttu-id="94e37-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppRegistration](../resources/intune-mam-managedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="94e37-131">If successful, this method returns a `200 OK` response code and [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e37-132">Пример</span><span class="sxs-lookup"><span data-stu-id="94e37-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="94e37-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="94e37-133">Request</span></span>
<span data-ttu-id="94e37-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94e37-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="94e37-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="94e37-135">Response</span></span>
<span data-ttu-id="94e37-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94e37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 956

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppRegistration",
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
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "5496aa60-aa60-5496-60aa-965460aa9654",
    "version": "Version value"
  }
}
```




