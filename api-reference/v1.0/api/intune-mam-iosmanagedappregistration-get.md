---
title: Get iosManagedAppRegistration
description: Чтение свойств и связей объекта iosManagedAppRegistration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0adb8800b4caabf108f7df2fce728af10ee2cc73
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454156"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="d95c5-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d95c5-103">Get iosManagedAppRegistration</span></span>

<span data-ttu-id="d95c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d95c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d95c5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d95c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d95c5-106">Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="d95c5-106">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d95c5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d95c5-107">Prerequisites</span></span>
<span data-ttu-id="d95c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d95c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d95c5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d95c5-110">Permission type</span></span>|<span data-ttu-id="d95c5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d95c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d95c5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d95c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d95c5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d95c5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d95c5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d95c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d95c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d95c5-115">Not supported.</span></span>|
|<span data-ttu-id="d95c5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d95c5-116">Application</span></span>|<span data-ttu-id="d95c5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d95c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d95c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d95c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d95c5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d95c5-119">Optional query parameters</span></span>
<span data-ttu-id="d95c5-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d95c5-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d95c5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d95c5-121">Request headers</span></span>
|<span data-ttu-id="d95c5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d95c5-122">Header</span></span>|<span data-ttu-id="d95c5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d95c5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d95c5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d95c5-124">Authorization</span></span>|<span data-ttu-id="d95c5-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d95c5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d95c5-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d95c5-126">Accept</span></span>|<span data-ttu-id="d95c5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d95c5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d95c5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d95c5-128">Request body</span></span>
<span data-ttu-id="d95c5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d95c5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d95c5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d95c5-130">Response</span></span>
<span data-ttu-id="d95c5-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d95c5-131">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d95c5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d95c5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d95c5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d95c5-133">Request</span></span>
<span data-ttu-id="d95c5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d95c5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="d95c5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d95c5-135">Response</span></span>
<span data-ttu-id="d95c5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d95c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






