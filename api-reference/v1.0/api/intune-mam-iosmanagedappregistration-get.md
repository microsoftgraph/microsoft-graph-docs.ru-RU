---
title: Get iosManagedAppRegistration
description: Чтение свойств и связей объекта iosManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb843c0915e082bd06f84dbc54ce52fea2208948
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259033"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="4d210-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="4d210-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="4d210-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d210-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d210-105">Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4d210-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d210-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4d210-106">Prerequisites</span></span>
<span data-ttu-id="4d210-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d210-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d210-109">Permission type</span></span>|<span data-ttu-id="4d210-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d210-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d210-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d210-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d210-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d210-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4d210-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d210-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d210-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d210-114">Not supported.</span></span>|
|<span data-ttu-id="4d210-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d210-115">Application</span></span>|<span data-ttu-id="4d210-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d210-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d210-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d210-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d210-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d210-118">Optional query parameters</span></span>
<span data-ttu-id="4d210-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d210-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d210-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d210-120">Request headers</span></span>
|<span data-ttu-id="4d210-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d210-121">Header</span></span>|<span data-ttu-id="4d210-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4d210-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d210-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d210-123">Authorization</span></span>|<span data-ttu-id="4d210-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4d210-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d210-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d210-125">Accept</span></span>|<span data-ttu-id="4d210-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d210-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d210-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d210-127">Request body</span></span>
<span data-ttu-id="4d210-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d210-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d210-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d210-129">Response</span></span>
<span data-ttu-id="4d210-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4d210-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d210-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4d210-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d210-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d210-132">Request</span></span>
<span data-ttu-id="4d210-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d210-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="4d210-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d210-134">Response</span></span>
<span data-ttu-id="4d210-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d210-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



