---
title: Get androidManagedAppRegistration
description: Считывание свойств и связей объекта androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10d277074c929bf5e57472983ca64db9522c5e8a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141393"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="a397a-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a397a-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="a397a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a397a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a397a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a397a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a397a-106">Чтение свойств и связей объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a397a-106">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a397a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a397a-107">Prerequisites</span></span>
<span data-ttu-id="a397a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a397a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a397a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a397a-110">Permission type</span></span>|<span data-ttu-id="a397a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a397a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a397a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a397a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a397a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a397a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a397a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a397a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a397a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a397a-115">Not supported.</span></span>|
|<span data-ttu-id="a397a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a397a-116">Application</span></span>|<span data-ttu-id="a397a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a397a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a397a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a397a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a397a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a397a-119">Optional query parameters</span></span>
<span data-ttu-id="a397a-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a397a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a397a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a397a-121">Request headers</span></span>
|<span data-ttu-id="a397a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a397a-122">Header</span></span>|<span data-ttu-id="a397a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a397a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a397a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a397a-124">Authorization</span></span>|<span data-ttu-id="a397a-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a397a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a397a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a397a-126">Accept</span></span>|<span data-ttu-id="a397a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a397a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a397a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a397a-128">Request body</span></span>
<span data-ttu-id="a397a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a397a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a397a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a397a-130">Response</span></span>
<span data-ttu-id="a397a-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a397a-131">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a397a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a397a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a397a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a397a-133">Request</span></span>
<span data-ttu-id="a397a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a397a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="a397a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a397a-135">Response</span></span>
<span data-ttu-id="a397a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a397a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

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
    "version": "Version value",
    "patchVersion": "Patch Version value"
  }
}
```




