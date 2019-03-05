---
title: Перечисление объектов androidManagedAppRegistration
description: Список свойств и связей объектов androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14169256c0aae4eea6d8190575c9519213dc3293
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254928"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="091d6-103">Перечисление объектов androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="091d6-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="091d6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="091d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="091d6-105">Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="091d6-105">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="091d6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="091d6-106">Prerequisites</span></span>
<span data-ttu-id="091d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="091d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="091d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="091d6-109">Permission type</span></span>|<span data-ttu-id="091d6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="091d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="091d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="091d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="091d6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="091d6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="091d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="091d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="091d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091d6-114">Not supported.</span></span>|
|<span data-ttu-id="091d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="091d6-115">Application</span></span>|<span data-ttu-id="091d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="091d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="091d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="091d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="091d6-118">Request headers</span></span>
|<span data-ttu-id="091d6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="091d6-119">Header</span></span>|<span data-ttu-id="091d6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="091d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="091d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="091d6-121">Authorization</span></span>|<span data-ttu-id="091d6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="091d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="091d6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="091d6-123">Accept</span></span>|<span data-ttu-id="091d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="091d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="091d6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="091d6-125">Request body</span></span>
<span data-ttu-id="091d6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="091d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="091d6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="091d6-127">Response</span></span>
<span data-ttu-id="091d6-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="091d6-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="091d6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="091d6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="091d6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="091d6-130">Request</span></span>
<span data-ttu-id="091d6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="091d6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="091d6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="091d6-132">Response</span></span>
<span data-ttu-id="091d6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="091d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```



